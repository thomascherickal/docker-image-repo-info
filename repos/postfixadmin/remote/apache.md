## `postfixadmin:apache`

```console
$ docker pull postfixadmin@sha256:578faf0cd2dcd496b22ee1687de01ca9287345712e6d2cf2f3daffdfd3c18fe0
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

### `postfixadmin:apache` - linux; amd64

```console
$ docker pull postfixadmin@sha256:6a5b9306d05710e7f65038b206e397c971bbaa7775dc914f836c2ea0490f6344
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.2 MB (171167820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d40cd21fa67acdcc31c61f1e308f33ac6b5f0f938b6af8a9bb3f7f8fece62de7`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:38:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 04:38:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 04:38:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:38:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 04:38:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 04:45:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 04:45:06 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 04:45:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 04:45:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 19:36:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:36:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:36:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 23:04:42 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 14 Oct 2021 23:04:42 GMT
ENV PHP_VERSION=7.4.24
# Thu, 14 Oct 2021 23:04:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 14 Oct 2021 23:04:43 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 14 Oct 2021 23:05:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 23:05:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 23:11:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 23:11:14 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 14 Oct 2021 23:11:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 23:11:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 23:11:16 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 Oct 2021 23:11:17 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 Oct 2021 23:11:17 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 23:11:18 GMT
EXPOSE 80
# Thu, 14 Oct 2021 23:11:18 GMT
CMD ["apache2-foreground"]
# Thu, 21 Oct 2021 19:58:43 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 21 Oct 2021 19:58:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 19:59:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 19:59:17 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 19:59:17 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 19:59:18 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 19:59:18 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 19:59:18 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 21 Oct 2021 19:59:19 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 21 Oct 2021 19:59:21 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 21 Oct 2021 19:59:21 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 21 Oct 2021 19:59:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Oct 2021 19:59:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b15dfd3cfa205395e33cb9ea4155c38a2a83a7acee7cb46fb9c169fcbe7411`  
		Last Modified: Tue, 12 Oct 2021 09:03:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64625c2e355fe69d0228e8a97fd6a1eb71879d7abe06240beec04e919e259c02`  
		Last Modified: Tue, 12 Oct 2021 09:04:08 GMT  
		Size: 91.6 MB (91605096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275a8dd8f3587f8c1fe7fc1f672f2e0757e95d18a018a5378cca93b98312415d`  
		Last Modified: Tue, 12 Oct 2021 09:03:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1c8ccc797aa9ff6819e95d6b867b2696860e31d2cac35e904316766ac9b44d`  
		Last Modified: Tue, 12 Oct 2021 09:04:43 GMT  
		Size: 19.2 MB (19235736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf98f0c33af1f7822072ae2d18f8296d65b117192dbef2026b4bca3737656d`  
		Last Modified: Tue, 12 Oct 2021 09:04:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e7c544c3e3203131f005689418e38d82298c3bc2bce4db3efe927345f6e34e`  
		Last Modified: Tue, 12 Oct 2021 09:04:39 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dfe78542d6b123eab61e038bf0f6814b587ca7ed09ace3e6e8101dc7f5fe59`  
		Last Modified: Fri, 15 Oct 2021 02:34:39 GMT  
		Size: 10.7 MB (10713081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f4b5ff9f72e79cc2968db9eb7f79faf26329af5d234ac6c9af924e1b36cc41`  
		Last Modified: Fri, 15 Oct 2021 02:34:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41327333801beca95ea8e010e189e40c172a280862b4fa301879cd4611ef2824`  
		Last Modified: Fri, 15 Oct 2021 02:34:41 GMT  
		Size: 13.9 MB (13906369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d061bb1ce0785cf349a98382b485e5fe022c0eac4fc1c4f473929ed58f7fad5`  
		Last Modified: Fri, 15 Oct 2021 02:34:35 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18874285db3bb1009b8eefa7797f045d63d5fadfd50bdde4d9d5fd2e8c9f1218`  
		Last Modified: Fri, 15 Oct 2021 02:34:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7eef711e76b3a5268ae63199da631481c7ef72ed3df28b6e4d328be352dc89`  
		Last Modified: Fri, 15 Oct 2021 02:34:35 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e20a2c2045309856d6945ea23ea03c071b9f534efca1d1c336f5fbf74a0cc`  
		Last Modified: Thu, 21 Oct 2021 20:01:02 GMT  
		Size: 1.3 MB (1284013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6e65c700899a2f0aae553c5d528cd1fed00b614b586e8f5a15bd5c87be052b`  
		Last Modified: Thu, 21 Oct 2021 20:01:02 GMT  
		Size: 1.2 MB (1186154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de388a18714e824382250fe4eef3a4ac8c8d6f9113cdcaa24a51ca2b51ec4a71`  
		Last Modified: Thu, 21 Oct 2021 20:01:02 GMT  
		Size: 8.2 KB (8220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5743eabef8dc279863c4fd16c9a22aa5a0ad5a10855d288f12bbcebdf42d096e`  
		Last Modified: Thu, 21 Oct 2021 20:01:03 GMT  
		Size: 1.9 MB (1864815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49bf0e1db154f7daf09880b2c392c0bf4367c78544b0c6a9aad38db850e682f1`  
		Last Modified: Thu, 21 Oct 2021 20:01:02 GMT  
		Size: 1.6 KB (1598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; arm variant v5

```console
$ docker pull postfixadmin@sha256:ad4e4491a7e6c8cfc4d38c673ec368e89da80b35162f08dd18146d25c060559f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (149040678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c15084279852d75a33a93cb810aa489487457d29a5aeb4d72c46bbb776c3e4`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:30 GMT
ADD file:fb1afabdc1f93b4866b4c4d696f272b4888519cb5bf35eb7ed1a4c021d1a04c8 in / 
# Tue, 12 Oct 2021 00:50:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 07:37:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 07:37:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 07:37:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 07:37:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 07:37:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 07:43:28 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 07:43:29 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 07:43:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 07:43:55 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 07:43:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 20:45:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 20:45:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 20:45:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 22:18:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 14 Oct 2021 22:18:36 GMT
ENV PHP_VERSION=7.4.24
# Thu, 14 Oct 2021 22:18:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 14 Oct 2021 22:18:37 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 14 Oct 2021 22:19:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 22:19:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:23:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 22:23:23 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:23:25 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 22:23:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 22:23:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 Oct 2021 22:23:26 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:23:27 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 22:23:27 GMT
EXPOSE 80
# Thu, 14 Oct 2021 22:23:28 GMT
CMD ["apache2-foreground"]
# Thu, 21 Oct 2021 21:26:08 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 21 Oct 2021 21:26:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 21:28:11 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 21:28:12 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 21:28:12 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 21:28:13 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 21:28:13 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 21:28:14 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 21 Oct 2021 21:28:16 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 21 Oct 2021 21:28:19 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 21 Oct 2021 21:28:20 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 21 Oct 2021 21:28:21 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Oct 2021 21:28:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5c9bab66abc5c53391435f6fd66e0ff3571295d568f45ac7d2dc480bcbfd56e8`  
		Last Modified: Tue, 12 Oct 2021 01:06:07 GMT  
		Size: 28.9 MB (28899715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569af31a3f546449c97619c10ce4bf50f7b5b53264865389d304aac632e1a590`  
		Last Modified: Tue, 12 Oct 2021 10:53:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa45e316719e67a0a4586c32f9f5226e0c60cc548199b5b6a4da1ef6ff38799`  
		Last Modified: Tue, 12 Oct 2021 10:54:22 GMT  
		Size: 73.7 MB (73684492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be2abc1db535bad2c3b042ee74207b681476c834f649b7f8435aebd6e2e76c8`  
		Last Modified: Tue, 12 Oct 2021 10:53:46 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4273f5c9ea07a27eb93a031e207cfaa52ddb62a6854f5c4895ec96fbcb049915`  
		Last Modified: Tue, 12 Oct 2021 10:55:13 GMT  
		Size: 18.5 MB (18525831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf2d473f376456fa9bbb3ac6543042b9d8e6690e10e9f0c0dfb504d2cfd89f4`  
		Last Modified: Tue, 12 Oct 2021 10:55:02 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd3b22adc21293942029cb70d452ee01d91e7eab707e2ac5bddd1ef4d5e586c`  
		Last Modified: Tue, 12 Oct 2021 10:55:03 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a7926084ff4960edf830696973608c8e9476d4476c60a792e10b9882e17035`  
		Last Modified: Fri, 15 Oct 2021 00:45:28 GMT  
		Size: 10.7 MB (10711475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0cd2c3a1ea9edca6c0acd436f4dc8bf1adc12e459a7a594a5952db35268405`  
		Last Modified: Fri, 15 Oct 2021 00:45:24 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc214847248b69206923209a4c501196b171f455c05a58a12ad0d5dfe6fd315`  
		Last Modified: Fri, 15 Oct 2021 00:45:33 GMT  
		Size: 13.0 MB (12979618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787a37fca3a0a1756720aebe65c7379f6a8599f888462b52226aa1cd3317ab02`  
		Last Modified: Fri, 15 Oct 2021 00:45:24 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27787eb4cf92ab2bb4942cc18c9513ee292b03770e7cd077075f08bec1c13aa5`  
		Last Modified: Fri, 15 Oct 2021 00:45:24 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28750079abb92f3d2a44c944f665e165b30f0ed8c0cdc1c69a44441c769293ac`  
		Last Modified: Fri, 15 Oct 2021 00:45:24 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395ba3f5d8163d2a02275ff1e5e3f718cb2959f0108b17ff59f47c45e846a4ec`  
		Last Modified: Thu, 21 Oct 2021 21:31:57 GMT  
		Size: 1.2 MB (1229986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6509c5f8a96fd95d04570ced9ee2c3c911bc0a2d0cfc099550ea58d56904193e`  
		Last Modified: Thu, 21 Oct 2021 21:31:57 GMT  
		Size: 1.1 MB (1129475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8d7443352bb904dbd812b7f9035e9732d83e7b2cc3592adf97cf22c2741ef3`  
		Last Modified: Thu, 21 Oct 2021 21:31:56 GMT  
		Size: 8.2 KB (8224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0610fb183582d08ccf2386a9905533ab665cbccec3423609c66ca55da55921f0`  
		Last Modified: Thu, 21 Oct 2021 21:31:58 GMT  
		Size: 1.9 MB (1864819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bffc1f436b5f5d36ba58b2fc2fa47f0c4177931512dde19f7df650dcd90a177`  
		Last Modified: Thu, 21 Oct 2021 21:31:56 GMT  
		Size: 1.6 KB (1599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:47b4db3dbea53e1feba447ca46d26bd28b75b874b6031e2e651320269ed57dc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.0 MB (141035951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ecdef073ebb8333f567e9f9567333a4d4201c13122c9114ee0a4a7d6a37a03f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 10:11:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 10:11:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 10:12:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 10:12:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 10:12:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 10:17:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 10:17:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 10:18:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 10:18:19 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 10:18:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 19:13:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:13:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:13:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 21:18:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 14 Oct 2021 21:18:37 GMT
ENV PHP_VERSION=7.4.24
# Thu, 14 Oct 2021 21:18:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 14 Oct 2021 21:18:38 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 14 Oct 2021 21:19:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 21:19:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 21:23:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 21:23:11 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 14 Oct 2021 21:23:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 21:23:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 21:23:13 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 Oct 2021 21:23:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 Oct 2021 21:23:14 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 21:23:15 GMT
EXPOSE 80
# Thu, 14 Oct 2021 21:23:15 GMT
CMD ["apache2-foreground"]
# Fri, 22 Oct 2021 01:57:33 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 22 Oct 2021 01:57:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 01:59:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 01:59:26 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Fri, 22 Oct 2021 01:59:27 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 22 Oct 2021 01:59:27 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Fri, 22 Oct 2021 01:59:27 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 22 Oct 2021 01:59:28 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Fri, 22 Oct 2021 01:59:29 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Fri, 22 Oct 2021 01:59:33 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 22 Oct 2021 01:59:33 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Fri, 22 Oct 2021 01:59:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 01:59:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd9f480a07dd663124a4fa2dd037ecfa121fb7f48c5611ad0bfdcc1a8620a95`  
		Last Modified: Tue, 12 Oct 2021 13:25:43 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541b04bc4262d66b1debf2bdfc8f9af3aaaf35857a5129ef875c83b66d9ca381`  
		Last Modified: Tue, 12 Oct 2021 13:26:25 GMT  
		Size: 69.3 MB (69314813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0c01531f1abfd9002da0136f1c5f9d7f1dded1e9c635594a2416f9b2592b57`  
		Last Modified: Tue, 12 Oct 2021 13:25:43 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46f326eb4d7df5b1062f7cf9febcde80dff286e3c58467e4b0bb4fe994e1c49`  
		Last Modified: Tue, 12 Oct 2021 13:27:16 GMT  
		Size: 18.0 MB (17987465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90b5a512593f340cfcf524a288c914574af941f7ba1ca3407b4c8810ef9f2f9`  
		Last Modified: Tue, 12 Oct 2021 13:27:06 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5ae29d359a60994986ddf2bc5eeffe6ec88d873499473e034fd5633404c155`  
		Last Modified: Tue, 12 Oct 2021 13:27:06 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a5dd55a4f93c66a707288490f7446af08210e00d23e4ae214faeaa8ae9f101`  
		Last Modified: Fri, 15 Oct 2021 00:49:14 GMT  
		Size: 10.7 MB (10711379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:799ec2f4ed47eddeea1f84eb3ccd244723336619b51ad8eaa4cff965ce14d7f4`  
		Last Modified: Fri, 15 Oct 2021 00:49:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fea13f870fc4ca75943e25f3cdaf7be611d1fde21ae5dcb964540ebf12a920`  
		Last Modified: Fri, 15 Oct 2021 00:49:12 GMT  
		Size: 12.3 MB (12277051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5da544db8cd1dd5fb19369d3dc6d24cd78447d2e2652359e0066d69b58f8c54`  
		Last Modified: Fri, 15 Oct 2021 00:49:04 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044cdd4b4f54e78e2c335b47f55556e54c882403d3b241bea2f347eb27c34b5a`  
		Last Modified: Fri, 15 Oct 2021 00:49:04 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16111c7aab1cfc4a8825d5713da24bf004dd1c5fddd6d5b73303a654ac990b3d`  
		Last Modified: Fri, 15 Oct 2021 00:49:04 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b151150e9c6ee5b2d8df3acdbbf8e2563389d464794ff0a4a9dc56685f6b9a`  
		Last Modified: Fri, 22 Oct 2021 02:05:11 GMT  
		Size: 1.2 MB (1224365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647c7003f320df5a8c0b1bb373c1526997f33a8ce3d9158609fd2d80d98d5f86`  
		Last Modified: Fri, 22 Oct 2021 02:05:11 GMT  
		Size: 1.1 MB (1079731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c09082ea62b80d5a6d31fed1c1e120b3e601183975ad5fa3c22b55efee4e2b`  
		Last Modified: Fri, 22 Oct 2021 02:05:10 GMT  
		Size: 8.2 KB (8223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cfbf2530a14ec01df5493a6c47089bb67ce30801cadbacac26790574c46c2e`  
		Last Modified: Fri, 22 Oct 2021 02:05:12 GMT  
		Size: 1.9 MB (1864821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d3a9489b99186056403e0a4827803430c06532ed68e1b0dddc14e26a9a67b`  
		Last Modified: Fri, 22 Oct 2021 02:05:10 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:4186062f2604df831da593dd4f1a9c0fc78a0e81a50d89a69a697a523d670181
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.9 MB (163881623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60c5697420ac2ae7c0e54cdf525d899f60738c61403010231dcb801ce0b7b2ef`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:18 GMT
ADD file:d84144ad575672cd6cc8a00c8e5a88ab0545348f040fc249ea5fcf8193b2bce6 in / 
# Tue, 12 Oct 2021 01:41:18 GMT
CMD ["bash"]
# Thu, 14 Oct 2021 20:01:06 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 Oct 2021 20:01:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 Oct 2021 20:01:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 Oct 2021 20:01:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 Oct 2021 20:01:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 Oct 2021 20:06:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 Oct 2021 20:06:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 Oct 2021 20:06:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 Oct 2021 20:06:13 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 Oct 2021 20:06:14 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 20:06:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 20:06:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 20:06:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 21:40:43 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 14 Oct 2021 21:40:44 GMT
ENV PHP_VERSION=7.4.24
# Thu, 14 Oct 2021 21:40:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 14 Oct 2021 21:40:46 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 14 Oct 2021 21:41:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 21:41:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 21:42:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 21:42:59 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 14 Oct 2021 21:42:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 21:43:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 21:43:01 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 Oct 2021 21:43:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 Oct 2021 21:43:03 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 21:43:04 GMT
EXPOSE 80
# Thu, 14 Oct 2021 21:43:05 GMT
CMD ["apache2-foreground"]
# Thu, 21 Oct 2021 19:36:26 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 21 Oct 2021 19:36:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 19:37:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 19:37:05 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 19:37:06 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 19:37:07 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 19:37:08 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 19:37:09 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 21 Oct 2021 19:37:10 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 21 Oct 2021 19:37:13 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 21 Oct 2021 19:37:14 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 21 Oct 2021 19:37:14 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Oct 2021 19:37:15 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a9eb63951c1c2ee8efcc12b696928fee3741a2d4eae76f2da3e161a5d90548bf`  
		Last Modified: Tue, 12 Oct 2021 01:48:13 GMT  
		Size: 30.0 MB (30043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e8dc602726d99b28b5686afda874ade5e865d91b658bc68dff4a02c3062f7a`  
		Last Modified: Thu, 14 Oct 2021 23:07:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0f1ee1d0d511e2f20f2114a9991e2f3cf25a91cae9d6662a65cf2b4f53dc01`  
		Last Modified: Thu, 14 Oct 2021 23:07:30 GMT  
		Size: 86.9 MB (86920409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7a167ae8f3a912487645dcb4aef47f14d63f29d7a1c2ea4ae26bdd531f2f8f`  
		Last Modified: Thu, 14 Oct 2021 23:07:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566731d744b22af202f1c1f1cb5af9f295596e83869b10e07397c7bd085908ae`  
		Last Modified: Thu, 14 Oct 2021 23:08:04 GMT  
		Size: 18.9 MB (18939819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512a0e300c292015b8f6716bc5d9f3469fa6a7f958a487a002ab1da01938573c`  
		Last Modified: Thu, 14 Oct 2021 23:08:01 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe39677b5f5deed457115099f2a19558013a51d7679a6c702d90b9cc72b0d4b1`  
		Last Modified: Thu, 14 Oct 2021 23:08:01 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa42ed0ea8a66488a49b29dd374d741bc49a3c09ac79310616c3c01fae78b04`  
		Last Modified: Thu, 14 Oct 2021 23:19:23 GMT  
		Size: 10.5 MB (10497235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592150534f5669317c8b9779cf10e56a1d9470428740a4e1c68b38838fd02ba0`  
		Last Modified: Thu, 14 Oct 2021 23:19:19 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1effaf8fba1fc2ae353aa6e9d6733e8ace4b1c946dd9a2df6d8987b3e384719c`  
		Last Modified: Thu, 14 Oct 2021 23:19:22 GMT  
		Size: 13.6 MB (13647724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8da9c3c8cb90f8e5c5288065107aa087b3fb9daed8139cc7841f23751374798`  
		Last Modified: Thu, 14 Oct 2021 23:19:19 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f4d1f04aa53d9b9cc82888c810c2a0340aca9dca2e3b075d67a21839baab10`  
		Last Modified: Thu, 14 Oct 2021 23:19:19 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609e8edb16730211afee3f1c83110ba95361bd3b29af9bed4890281ecbcd410c`  
		Last Modified: Thu, 14 Oct 2021 23:19:19 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105c2b06befe2dc7e3e59608c5ddc9c635d07c3c5ff6bb94da5b5945b8c65af0`  
		Last Modified: Thu, 21 Oct 2021 19:39:40 GMT  
		Size: 991.4 KB (991438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c755dd5678e3aadbd4ce7cdc2b7fc7982783c595ace2a9bf759a8ea5afb2c040`  
		Last Modified: Thu, 21 Oct 2021 19:39:40 GMT  
		Size: 961.3 KB (961272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c0398614acaa9e854c710eb65c0586b702df85b40279d918ecd0a96f351406`  
		Last Modified: Thu, 21 Oct 2021 19:39:39 GMT  
		Size: 8.2 KB (8220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8bb34f9cd11054103d5a47d98a6be26d6b9f0ccd5a698c139aab0141fe4b95`  
		Last Modified: Thu, 21 Oct 2021 19:39:40 GMT  
		Size: 1.9 MB (1864693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd165f8a417888d622823f732bd40950211a04bc8b85f90d1b2b1603ce0b903`  
		Last Modified: Thu, 21 Oct 2021 19:39:39 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; 386

```console
$ docker pull postfixadmin@sha256:4efc0587c6cb4b20966e573604bc3acc58d37aeca98f76121f565b178dc23d60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.1 MB (174070281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c52ba28a96b0cf3729211dda1d24d07fc0e3fbf48da407295b49959daa357b`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:47 GMT
ADD file:42196ffa4c70af8d9f1e7b74edb3bb92d47296acf989adf615e8208230f8bd0c in / 
# Tue, 12 Oct 2021 01:39:47 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:16:01 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 18:16:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 18:16:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:16:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 18:16:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 18:23:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 18:23:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 18:23:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 18:23:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 18:23:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 19:56:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:56:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:56:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 23:39:30 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 14 Oct 2021 23:39:31 GMT
ENV PHP_VERSION=7.4.24
# Thu, 14 Oct 2021 23:39:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 14 Oct 2021 23:39:32 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 14 Oct 2021 23:40:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 23:40:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 23:44:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 23:44:14 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 14 Oct 2021 23:44:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 23:44:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 23:44:16 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 Oct 2021 23:44:16 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 Oct 2021 23:44:16 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 23:44:17 GMT
EXPOSE 80
# Thu, 14 Oct 2021 23:44:17 GMT
CMD ["apache2-foreground"]
# Fri, 15 Oct 2021 07:30:05 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 15 Oct 2021 07:30:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 Oct 2021 07:30:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 Oct 2021 07:30:46 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Fri, 15 Oct 2021 07:30:46 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 15 Oct 2021 07:30:46 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Fri, 15 Oct 2021 07:30:47 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 15 Oct 2021 07:30:47 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Fri, 15 Oct 2021 07:30:48 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Fri, 15 Oct 2021 07:30:49 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 15 Oct 2021 07:30:50 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Fri, 15 Oct 2021 07:30:50 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 15 Oct 2021 07:30:50 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:87318d165b5c0fdf05c8ccf97d83084f56b4608075a3335b1a46c76295b82753`  
		Last Modified: Tue, 12 Oct 2021 01:47:39 GMT  
		Size: 32.4 MB (32370344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d7b55744f495c4538bc35e1935df5ce5a3ac7584169b9dadb5641beaa08fc6`  
		Last Modified: Tue, 12 Oct 2021 22:06:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55f1f83e7520231f01d19a9decf9941bac0dc2290dbc514216b787edacfb1f8`  
		Last Modified: Tue, 12 Oct 2021 22:06:55 GMT  
		Size: 92.7 MB (92716556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff493eb0e3106a89b7c5f55740e05ffe39bde5673df81dea4f0a8609627c220a`  
		Last Modified: Tue, 12 Oct 2021 22:06:16 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae05156eebdd94107900118e3da52a91e1b61ce12bcd59c1e08419517ed5ed90`  
		Last Modified: Tue, 12 Oct 2021 22:07:49 GMT  
		Size: 19.7 MB (19713810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df85d9bc98416a8f2cf28362008d41b0704f55c78064c00824a48889ca88f620`  
		Last Modified: Tue, 12 Oct 2021 22:07:39 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c77e1860324939b5cb12581995bd0f576c4290473ab64d2d7d8f695aac3821`  
		Last Modified: Tue, 12 Oct 2021 22:07:39 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3420c0565407e0e8bcdace4b249a5d36a9849231596d3d001de2265e9fa39f3c`  
		Last Modified: Fri, 15 Oct 2021 03:15:56 GMT  
		Size: 10.7 MB (10712296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24a6ce4cdc49983f99efa0c03579c786ac12bc10e7f7f3438a2ec6f35f09fc4`  
		Last Modified: Fri, 15 Oct 2021 03:15:52 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c898e1a9cdf34e4ed522e241697485303841153538866f73ec889750a2610620`  
		Last Modified: Fri, 15 Oct 2021 03:15:56 GMT  
		Size: 14.2 MB (14230502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e6b825f859eccd41152cbb7bd3c40167d7a7907a1a0a5a0df923b73f972f5d`  
		Last Modified: Fri, 15 Oct 2021 03:15:52 GMT  
		Size: 2.3 KB (2317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072ec6552778a68045d33a96891895ce717f1f0bbce0040e1a587bc513834e05`  
		Last Modified: Fri, 15 Oct 2021 03:15:52 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03dba78f9d2c4dbc18ca32e92bdf90e6e3eaa310f0c1e36bce59d0391387eeac`  
		Last Modified: Fri, 15 Oct 2021 03:15:52 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcb038b143e8f20a9745832f9aa208de715ebb11bc9060f6a392a17c03db4cb`  
		Last Modified: Fri, 15 Oct 2021 07:33:07 GMT  
		Size: 1.2 MB (1243236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e95b36961a5f120b09290b907868852f8cdc466014df156f86e31e923e6b62e`  
		Last Modified: Fri, 15 Oct 2021 07:33:07 GMT  
		Size: 1.2 MB (1203475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d176a1f0939eece0bc0b110e9d1f3124b92debdcab11d46f0c7c1500c73a548f`  
		Last Modified: Fri, 15 Oct 2021 07:33:06 GMT  
		Size: 8.2 KB (8221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbd3cc74fc4eaa0159ef7653ab74f9057b10e994b99d135d6615774c9fe89d5`  
		Last Modified: Fri, 15 Oct 2021 07:33:07 GMT  
		Size: 1.9 MB (1864814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3eba70215f6ba991a80cef018ddac61d3c38ec632b4b5a35f21fb57cbeaeb25`  
		Last Modified: Fri, 15 Oct 2021 07:33:06 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; mips64le

```console
$ docker pull postfixadmin@sha256:2220747c8618ef84c1ee81c2018723db191b59e764a6807fa443e87ef0c50a0f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148871709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4e7d5736d8f455c5cb1aedef6f7104fb847856e27d5b3e785289abec737d971`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:11:15 GMT
ADD file:f90ca8957172106f42a9096c9a21082d51f3201aa78e6f64621a73117e2b7b6a in / 
# Tue, 12 Oct 2021 01:11:16 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:09:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 18:09:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 18:10:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:10:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 18:10:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 18:24:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 18:24:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 18:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 18:24:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 18:24:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 19:23:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:23:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:23:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 22:46:30 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 14 Oct 2021 22:46:30 GMT
ENV PHP_VERSION=7.4.24
# Thu, 14 Oct 2021 22:46:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 14 Oct 2021 22:46:31 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 14 Oct 2021 22:46:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 22:46:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:54:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 22:54:42 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:54:44 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 22:54:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 22:54:45 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 Oct 2021 22:54:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:54:46 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 22:54:46 GMT
EXPOSE 80
# Thu, 14 Oct 2021 22:54:46 GMT
CMD ["apache2-foreground"]
# Thu, 21 Oct 2021 19:48:22 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 21 Oct 2021 19:48:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 19:50:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Oct 2021 19:50:24 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 19:50:24 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 19:50:24 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 19:50:25 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 19:50:25 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Thu, 21 Oct 2021 19:50:27 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Thu, 21 Oct 2021 19:50:31 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 21 Oct 2021 19:50:31 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Thu, 21 Oct 2021 19:50:32 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Oct 2021 19:50:32 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:59ddca50ce05605e6234c1e7213c39cdedabc48ef11637e12156b7bd69afe161`  
		Last Modified: Tue, 12 Oct 2021 01:20:03 GMT  
		Size: 29.6 MB (29618732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff87c2332509770737b3726a7edbc9070eb8965e3168af4e323e11735f2c92`  
		Last Modified: Wed, 13 Oct 2021 00:47:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb84497951b93c12a62afde8f02ebbea1b6bc7408856d226297b5a3be0a7c92`  
		Last Modified: Wed, 13 Oct 2021 00:48:33 GMT  
		Size: 72.0 MB (72014027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d4e4615e6fe3d8e364eacce72f7ccce515209e2da18447ca24da978c31e38c`  
		Last Modified: Wed, 13 Oct 2021 00:47:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4922634a24fcda8d05a799ce9a76bad0bc77f74e6183b0c01c24561c5fcdf50a`  
		Last Modified: Wed, 13 Oct 2021 00:49:17 GMT  
		Size: 19.1 MB (19143667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727d7b8f91bd9e80b3890e0309546b7201a45d40c6c45c35efca82a3c5fe40ff`  
		Last Modified: Wed, 13 Oct 2021 00:49:04 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d4efcc601a141d1be58474d763f5f131619fdfdcc0d3d3bee16bfb8e7241e7`  
		Last Modified: Wed, 13 Oct 2021 00:49:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e04d7c6580baec7aff1ca88f51b75d72f0da2294db1228c542488150be685ff`  
		Last Modified: Fri, 15 Oct 2021 01:28:23 GMT  
		Size: 10.7 MB (10710433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616ac43e76a3409ee973fb9515e06fb5cbb28266f51cdb8bff139c3bbaf12667`  
		Last Modified: Fri, 15 Oct 2021 01:28:18 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b5295d421c463fd747678a24b7d32b71d19e011f2b55d5f9c098d1ad333c20`  
		Last Modified: Fri, 15 Oct 2021 01:28:29 GMT  
		Size: 13.2 MB (13191642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e998102b3a9121b289542f585cc896dd82bef268145fe4b883b054d0e0322f`  
		Last Modified: Fri, 15 Oct 2021 01:28:18 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233ea2041e8f9ad3de870a3b4300814106d9d6730b2f2231a3db585c69acd25a`  
		Last Modified: Fri, 15 Oct 2021 01:28:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6969e59c42140b3df0397352e5eccb4c4f5ed710c5f3f465d919ef69ff9171e6`  
		Last Modified: Fri, 15 Oct 2021 01:28:18 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42482c81dc2dc342e2a54e09ff5297286ee6d9a5eaf24accc1f3aa915a0827c`  
		Last Modified: Thu, 21 Oct 2021 19:53:03 GMT  
		Size: 1.2 MB (1160220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb7d4dd77b58ee3fda27f888f913afbb9c95f9878e7c8374ff0662fab24f55`  
		Last Modified: Thu, 21 Oct 2021 19:53:03 GMT  
		Size: 1.2 MB (1153058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c3d57bdd16be8bdd851e9f383e578f891aef36c8d205d94a0b207401403e60`  
		Last Modified: Thu, 21 Oct 2021 19:53:02 GMT  
		Size: 8.2 KB (8223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f8feaad5b091290ba95d526e6c70c81263cd45d30bb41c8f9fbaa66fd93508`  
		Last Modified: Thu, 21 Oct 2021 19:53:04 GMT  
		Size: 1.9 MB (1864791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385c338380645b18296749d20402dd25d27c1f0822f1ee562cb936baf00298c0`  
		Last Modified: Thu, 21 Oct 2021 19:53:02 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:1d3f719c1e3af7a4c55ec196ffab4dfd0f1cc83179a37ea608d50e8e181d5cc5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.3 MB (172349351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2897449b9523f9d9a64a6bcdb0fde7d54ca74236a96cc05ca37a0f1c0d51e932`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:25:45 GMT
ADD file:d8794fadf16c9948c3574ba28740d08393eca57766340333ad91f9c2a33eb719 in / 
# Tue, 12 Oct 2021 01:25:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 10:23:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 10:23:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 10:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 10:26:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 10:26:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 10:33:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 10:33:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 10:34:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 10:34:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 10:34:47 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 19:29:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:29:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:29:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 21:55:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 14 Oct 2021 21:55:27 GMT
ENV PHP_VERSION=7.4.24
# Thu, 14 Oct 2021 21:55:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 14 Oct 2021 21:55:33 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 14 Oct 2021 21:56:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 21:56:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:01:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 22:01:41 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:01:53 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 22:01:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 22:02:04 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 Oct 2021 22:02:06 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:02:08 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 22:02:10 GMT
EXPOSE 80
# Thu, 14 Oct 2021 22:02:14 GMT
CMD ["apache2-foreground"]
# Fri, 22 Oct 2021 01:45:45 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 22 Oct 2021 01:46:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 01:48:45 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 01:48:48 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Fri, 22 Oct 2021 01:48:52 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 22 Oct 2021 01:48:54 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Fri, 22 Oct 2021 01:48:57 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 22 Oct 2021 01:48:59 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Fri, 22 Oct 2021 01:49:14 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Fri, 22 Oct 2021 01:49:33 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 22 Oct 2021 01:49:40 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Fri, 22 Oct 2021 01:49:47 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 01:49:53 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6c28c1405c677dd809094d06190225b38cee3d24f18da38d287ef5bcc67884d6`  
		Last Modified: Tue, 12 Oct 2021 01:37:00 GMT  
		Size: 35.3 MB (35258729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007cbc0c1bbccf469e9d9fc6e98e3d4ad1e4469d5f23cc0d263aa3bdc8f9c5`  
		Last Modified: Tue, 12 Oct 2021 14:32:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6750fd2121e14e6e55c726ed712f7b485e03363824dd42e9fa37ca714848f4c6`  
		Last Modified: Tue, 12 Oct 2021 14:33:23 GMT  
		Size: 86.6 MB (86624771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6280509c1db590ff214716adca9daabd1ac3c060c29e70cf6ed8dc17061d64db`  
		Last Modified: Tue, 12 Oct 2021 14:32:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dfb045a88eef5b0550b8548fbf2106468aac82881db516e679b9d5811ab750`  
		Last Modified: Tue, 12 Oct 2021 14:34:14 GMT  
		Size: 20.4 MB (20441245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b153f7d4d58c38f56768aadaefa599fdeb615c6c4940ce33f129d7df3c44d8a`  
		Last Modified: Tue, 12 Oct 2021 14:33:57 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed81b8cad279c736a63388220d89e0dc436c6f8586239e6e9c3b975efaf6c1f`  
		Last Modified: Tue, 12 Oct 2021 14:33:57 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea636c835b9c90a27d664a0b935da46eaec8b944bb0c664269b8a4f50e5dc2b`  
		Last Modified: Fri, 15 Oct 2021 00:52:38 GMT  
		Size: 10.7 MB (10713323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33018f04e235ad2cb38d254de419c077cb6c79213b21dcc861dc11d6557f2f4d`  
		Last Modified: Fri, 15 Oct 2021 00:52:29 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0e5cbab4298bb806436d13f65156f97e561bbcc3933dc11ba74df44a193c8d`  
		Last Modified: Fri, 15 Oct 2021 00:52:49 GMT  
		Size: 14.9 MB (14923605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61f7f3b72d7f4b6e83b316433aaa57d4b98055f8c5fd47e329253f473b8de04`  
		Last Modified: Fri, 15 Oct 2021 00:52:30 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6660d34b68515de0b2f1dd9f85c4dfc49cf24b2c1289db802573571e1dcd7cb5`  
		Last Modified: Fri, 15 Oct 2021 00:52:29 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885eb351959e59f4d8352a5381ff5c419fb84cc3ffb891474768117cb6c0af05`  
		Last Modified: Fri, 15 Oct 2021 00:52:29 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cdd609756a326b89ef63336930b6ff875b6b848ddaa08f31dc912536fa2c4c`  
		Last Modified: Fri, 22 Oct 2021 01:56:38 GMT  
		Size: 1.2 MB (1186487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e5f424299dcb182f3c0ae49e2cc23dfab7fee5b965a59e40f4cc614a909607`  
		Last Modified: Fri, 22 Oct 2021 01:56:38 GMT  
		Size: 1.3 MB (1321112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb9b6a3f3b5236c87b6a0a6aa0b4233016811102731b38c2cc1cbf9ce26f171`  
		Last Modified: Fri, 22 Oct 2021 01:56:37 GMT  
		Size: 8.2 KB (8224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0f868634e5d6ff4b5587d7ff3cc4a0d93e7657a34e59c3767c70e7c1211b2`  
		Last Modified: Fri, 22 Oct 2021 01:56:38 GMT  
		Size: 1.9 MB (1864819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0a577deeacc9fc491a368f239dc0613f6cac37b61f137d182d07b255cd5ac5`  
		Last Modified: Fri, 22 Oct 2021 01:56:37 GMT  
		Size: 1.6 KB (1597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:apache` - linux; s390x

```console
$ docker pull postfixadmin@sha256:59d5141990f6510b2522944acebff12800356217a2509855bc74c6036eb55637
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.5 MB (148472281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7036fc405fcb3742618179393cb50a38b7577792d7d86bb19aa9373f4fd31be0`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:27 GMT
ADD file:6038dd6db57fb05c3d39c02c3379667ccd2989e7667ff773a8020fe6a69a760c in / 
# Tue, 12 Oct 2021 00:42:29 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:42:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 01:42:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 01:42:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 01:42:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 01:46:53 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 01:46:53 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 01:47:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 01:47:11 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 01:47:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 19:49:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:49:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:49:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 20:50:28 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 14 Oct 2021 20:50:28 GMT
ENV PHP_VERSION=7.4.24
# Thu, 14 Oct 2021 20:50:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 14 Oct 2021 20:50:28 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 14 Oct 2021 20:50:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 Oct 2021 20:50:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 20:51:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 20:51:58 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 14 Oct 2021 20:51:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 20:51:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 20:51:59 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 Oct 2021 20:51:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 Oct 2021 20:51:59 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 20:51:59 GMT
EXPOSE 80
# Thu, 14 Oct 2021 20:52:00 GMT
CMD ["apache2-foreground"]
# Fri, 15 Oct 2021 00:01:53 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 15 Oct 2021 00:01:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		gosu 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 Oct 2021 00:02:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 	libc-client2007e-dev 	libkrb5-dev 	libpq-dev 	libsqlite3-dev 	; 		docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 		docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 		ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 			apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 Oct 2021 00:02:17 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Fri, 15 Oct 2021 00:02:17 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 15 Oct 2021 00:02:17 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Fri, 15 Oct 2021 00:02:17 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 15 Oct 2021 00:02:17 GMT
ENV APACHE_DOCUMENT_ROOT=/var/www/html/public
# Fri, 15 Oct 2021 00:02:18 GMT
RUN set -eu; sed -ri -e 's!/var/www/html!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/sites-available/*.conf; 	sed -ri -e 's!/var/www/!${APACHE_DOCUMENT_ROOT}!g' /etc/apache2/apache2.conf /etc/apache2/conf-available/*.conf
# Fri, 15 Oct 2021 00:02:19 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 15 Oct 2021 00:02:20 GMT
COPY file:c9d831137af59b25a21b91306762892f72362178f6096a24bafecc047bbe6d37 in /usr/local/bin/ 
# Fri, 15 Oct 2021 00:02:20 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 15 Oct 2021 00:02:20 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ded751c48f72503973be01be2794cc039490f22b039b8ac106e9f17de4980742`  
		Last Modified: Tue, 12 Oct 2021 00:48:05 GMT  
		Size: 29.6 MB (29641215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e93f54c1a4ac2c0a445018626dbf2035ae9fff49f85693b56f619e876603022`  
		Last Modified: Tue, 12 Oct 2021 03:44:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a448f945ae4e9abe53c27b72c40f075c61a2ff21977f7b57567f443ad7dee68b`  
		Last Modified: Tue, 12 Oct 2021 03:44:34 GMT  
		Size: 71.6 MB (71618360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3bf3e5f5ecd4bafce85def29ee5490f29b810e95829c3702cc4157280350e6`  
		Last Modified: Tue, 12 Oct 2021 03:44:24 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fa8915dfded42c17fc2ad80a47a873711c8d6200aebee325a829c59c4f6d62`  
		Last Modified: Tue, 12 Oct 2021 03:44:55 GMT  
		Size: 19.1 MB (19052069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed0ccfb17f6bd74cac8f31177eeda092942c5553a73e2168a9dd660804dce37`  
		Last Modified: Tue, 12 Oct 2021 03:44:53 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25b2206fa558b0b5f7444116a8a5f096797010e47f17c377157fdbcd748edab`  
		Last Modified: Tue, 12 Oct 2021 03:44:53 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e81ad5901e98e81a976545c50eaf84bf56027dc2e1628997d59bed202ee732`  
		Last Modified: Thu, 14 Oct 2021 22:15:17 GMT  
		Size: 10.7 MB (10711680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ffceefee4f05b073a7cb9598fff13c3d1e074de1fa4ec736c852a2d75a8a07`  
		Last Modified: Thu, 14 Oct 2021 22:15:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edad02b9f260d1bf0f0d246ed8f837a49e22f2e0cfba4af6a5331789b2e95210`  
		Last Modified: Thu, 14 Oct 2021 22:15:17 GMT  
		Size: 13.1 MB (13142247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8691f9365d649cdbafccc10f718c3414448bf2ffc6174afc8907b159a73e154`  
		Last Modified: Thu, 14 Oct 2021 22:15:15 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262bfa9a1fc5a16f6ab385855a5940074d7ddea03bd94d5e18af56c13bececcd`  
		Last Modified: Thu, 14 Oct 2021 22:15:15 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e80ebfea5e7d9db73851dce6431dabc793767f4c0fbcd3b1db43c879ba268b`  
		Last Modified: Thu, 14 Oct 2021 22:15:15 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f0cb77c3c3a16cf0e8f2f4c6de4e7300528da4181beaca5ad4da5fc6304ba4`  
		Last Modified: Fri, 15 Oct 2021 00:04:09 GMT  
		Size: 1.2 MB (1245359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0d8ee76ea869896a22bee838cb2f03fbb17e1b193a7133a2fef08973329dfc`  
		Last Modified: Fri, 15 Oct 2021 00:04:08 GMT  
		Size: 1.2 MB (1181284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c2aff88502262f4dc6504b44f3795c5ae34de135c6f0989c78507627fa9588`  
		Last Modified: Fri, 15 Oct 2021 00:04:08 GMT  
		Size: 8.2 KB (8225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780f5abd92707077053d78bd98098a1ac436094fc2e4ff025ba2e07d3a0b8981`  
		Last Modified: Fri, 15 Oct 2021 00:04:08 GMT  
		Size: 1.9 MB (1864816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a611da486aae38c8ea6d557f9cc0651bdcd2dd57ecaf2e52e80e01e4566c4f70`  
		Last Modified: Fri, 15 Oct 2021 00:04:08 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
