## `yourls:apache`

```console
$ docker pull yourls@sha256:17e08a89e57e371a21f9bb56da82bf82999d3e84d434cf040c62eef8cb7e9097
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

### `yourls:apache` - linux; amd64

```console
$ docker pull yourls@sha256:bbbdc7302480ffcee7b4c30815ab38a9df0bddd24b9c7189b64ad6cef65e65c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.3 MB (170311188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac64d829654e48a29b273808594d7b89c5f26ce8e6698bf45d232684ea8e814a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:35:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 07:35:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 07:36:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:36:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 07:36:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 07:39:35 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 07:39:35 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 07:39:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 07:39:45 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 07:39:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 07:39:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 07:39:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 07:39:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 08:06:40 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:13:29 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:13:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Tue, 14 Feb 2023 21:13:29 GMT
ENV PHP_SHA256=7108b7347981ad6e610aaf3b3fb0f6444019ab6f59a872c1b55a29bc753eba93
# Tue, 14 Feb 2023 21:13:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 14 Feb 2023 21:13:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:16:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 21:16:42 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:16:43 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 21:16:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 21:16:43 GMT
STOPSIGNAL SIGWINCH
# Tue, 14 Feb 2023 21:16:43 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:16:43 GMT
WORKDIR /var/www/html
# Tue, 14 Feb 2023 21:16:43 GMT
EXPOSE 80
# Tue, 14 Feb 2023 21:16:43 GMT
CMD ["apache2-foreground"]
# Wed, 15 Feb 2023 00:55:12 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 15 Feb 2023 00:55:12 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 15 Feb 2023 00:55:12 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 15 Feb 2023 00:55:13 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 15 Feb 2023 00:55:13 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 15 Feb 2023 00:55:13 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 15 Feb 2023 00:55:13 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 15 Feb 2023 00:55:13 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 15 Feb 2023 00:55:54 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 15 Feb 2023 00:55:55 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 15 Feb 2023 00:55:55 GMT
RUN a2enmod rewrite expires
# Wed, 15 Feb 2023 00:55:55 GMT
ARG YOURLS_VERSION=1.9.1
# Wed, 15 Feb 2023 00:55:55 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 15 Feb 2023 00:55:56 GMT
LABEL org.opencontainers.image.version=1.9.1
# Wed, 15 Feb 2023 00:55:56 GMT
ENV YOURLS_VERSION=1.9.1
# Wed, 15 Feb 2023 00:55:56 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 15 Feb 2023 00:55:58 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 15 Feb 2023 00:55:58 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 15 Feb 2023 00:55:58 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 15 Feb 2023 00:55:58 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 15 Feb 2023 00:55:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Feb 2023 00:55:58 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0825793cba86d855da45c20858c3c3bd7121ac697fb1741bc38a779e261ab82e`  
		Last Modified: Thu, 09 Feb 2023 08:57:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3c011d207b2fa9b335817876040ab36845c702e712599e055c5613c0e23154`  
		Last Modified: Thu, 09 Feb 2023 08:57:49 GMT  
		Size: 91.6 MB (91636221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3c5bd9650e8a316cedc37895a14fb3c7555d183f74eabe3888ff504558f8c5`  
		Last Modified: Thu, 09 Feb 2023 08:57:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c3827232f74438f8883d98e1c582ac82c5daf0eed1ad78c404b1679b6f43fc`  
		Last Modified: Thu, 09 Feb 2023 08:58:32 GMT  
		Size: 19.2 MB (19244718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fdaec51865231cd0c095d584d05b75723060bd1a11e587ec77b41c409ffe44b`  
		Last Modified: Thu, 09 Feb 2023 08:58:29 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfea1d79d41c2cf0e150c6bf6635559028c824a2443695a77975048c237da2e`  
		Last Modified: Thu, 09 Feb 2023 08:58:29 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1778f4862f0b1f28277bc18a6c133cbafb3adbcf01f989003acfe01bfd305a1`  
		Last Modified: Tue, 14 Feb 2023 22:47:11 GMT  
		Size: 12.5 MB (12539649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e371c51a394ef101dcd25a9f39b18eaabde7484588032848a3ca529355ffc90`  
		Last Modified: Tue, 14 Feb 2023 22:47:08 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9226298947b7c2e28230ee5de7498eb68e5c376986733e5f366e3192d267cc9e`  
		Last Modified: Tue, 14 Feb 2023 22:47:10 GMT  
		Size: 11.0 MB (11049811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a2f63bce1933060b3ba2bf51ee8e8c40b1479d2e00c835be4b7ffedb846106`  
		Last Modified: Tue, 14 Feb 2023 22:47:08 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73a16e45a0f3a0ea2d174c68923eb3c01ed95d4011c9a812cf790c4fd3479dd5`  
		Last Modified: Tue, 14 Feb 2023 22:47:08 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d6575f672732341d21542bef0dd159f02bfb9b52b566c3405e6303a3ad2112b`  
		Last Modified: Tue, 14 Feb 2023 22:47:08 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb53e88d55fcb7847ac1769afc864a0511ed6413ea074e6dd7088eb417461c8`  
		Last Modified: Wed, 15 Feb 2023 00:58:07 GMT  
		Size: 515.2 KB (515238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70ed6c14956764c53fc0fb279aea1867dd8baccddabd3734ca3f91bce2e5f092`  
		Last Modified: Wed, 15 Feb 2023 00:58:06 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed1efd9b823aa1190d1414c985546c533c1c04b3a14800ad56ff7425a7f45ed`  
		Last Modified: Wed, 15 Feb 2023 00:58:04 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936dc951df1cf42ee0b1a30c4be194cdc5bd6d88530f452f1586f983659ab71e`  
		Last Modified: Wed, 15 Feb 2023 00:58:05 GMT  
		Size: 3.9 MB (3903534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e51fea25675f38ce0974b36bdc580052e2691eb83fbdeb2cdcde51fe97a18201`  
		Last Modified: Wed, 15 Feb 2023 00:58:04 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c3869b94361a22a0c663742d4641d851fb67a0c64d4115391e90b128af3495`  
		Last Modified: Wed, 15 Feb 2023 00:58:05 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c86a84db07247f73d3cefccbc86177194be77af51fd9d8a40da88816ac868`  
		Last Modified: Wed, 15 Feb 2023 00:58:04 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; arm variant v5

```console
$ docker pull yourls@sha256:d0a7399d491547caa504c472fa54317f28f57d634cd06ef684f543704957e4ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.8 MB (147825350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0dbe3a3231d9937b9c09e74d475a5b4e79391fd79b489d6a7ea7c82e07957d4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:32 GMT
ADD file:fcf4deede0eb98d96d8657dfb1b0918a2c3d35f16d4858dd9e75c843edeff166 in / 
# Thu, 09 Feb 2023 02:00:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:41:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 09:41:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 09:42:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:42:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 09:42:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 09:45:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 09:45:46 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 09:46:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 09:46:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 09:46:02 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 09:46:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 09:46:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 09:46:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 10:02:24 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 20:19:23 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 20:19:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Tue, 14 Feb 2023 20:19:23 GMT
ENV PHP_SHA256=7108b7347981ad6e610aaf3b3fb0f6444019ab6f59a872c1b55a29bc753eba93
# Tue, 14 Feb 2023 20:19:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 14 Feb 2023 20:19:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 20:24:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 20:24:04 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 14 Feb 2023 20:24:05 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 20:24:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 20:24:05 GMT
STOPSIGNAL SIGWINCH
# Tue, 14 Feb 2023 20:24:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 14 Feb 2023 20:24:05 GMT
WORKDIR /var/www/html
# Tue, 14 Feb 2023 20:24:05 GMT
EXPOSE 80
# Tue, 14 Feb 2023 20:24:06 GMT
CMD ["apache2-foreground"]
# Tue, 14 Feb 2023 23:29:19 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 14 Feb 2023 23:29:19 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 14 Feb 2023 23:29:19 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 14 Feb 2023 23:29:19 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 14 Feb 2023 23:29:19 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 14 Feb 2023 23:29:19 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 14 Feb 2023 23:29:20 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 14 Feb 2023 23:29:20 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 14 Feb 2023 23:29:56 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 14 Feb 2023 23:29:57 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 14 Feb 2023 23:29:57 GMT
RUN a2enmod rewrite expires
# Tue, 14 Feb 2023 23:29:58 GMT
ARG YOURLS_VERSION=1.9.1
# Tue, 14 Feb 2023 23:29:58 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 14 Feb 2023 23:29:58 GMT
LABEL org.opencontainers.image.version=1.9.1
# Tue, 14 Feb 2023 23:29:58 GMT
ENV YOURLS_VERSION=1.9.1
# Tue, 14 Feb 2023 23:29:58 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Tue, 14 Feb 2023 23:30:01 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 14 Feb 2023 23:30:01 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 14 Feb 2023 23:30:01 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 14 Feb 2023 23:30:02 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Tue, 14 Feb 2023 23:30:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Feb 2023 23:30:02 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:886a7482403a267f98b84e4a9f9ede516bac1fe7eb82ff570dabbb0b297d5b53`  
		Last Modified: Thu, 09 Feb 2023 02:05:42 GMT  
		Size: 28.9 MB (28916292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef01cc1baaf987e58ae2d4a64f117fe5666d6401388e74ded3219ee74d224b`  
		Last Modified: Thu, 09 Feb 2023 10:28:32 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550531f8ce72e1c3563629992c0eb48a41e389e248d119c6095fdb1d3700cfd1`  
		Last Modified: Thu, 09 Feb 2023 10:28:46 GMT  
		Size: 73.7 MB (73685604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598749bf70fc39c7a04d81520b000d32e64c62a1a0da866eb3155bccb1f9bdf1`  
		Last Modified: Thu, 09 Feb 2023 10:28:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dec2a390aa615bbeccf6ea0fa182763528d6f63dd033fc88c061ce3b3a104d`  
		Last Modified: Thu, 09 Feb 2023 10:29:49 GMT  
		Size: 18.6 MB (18554331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a115b83b8cb93becb81faeca7b96c26de27f7b2268e78e1339a9a90080d36f30`  
		Last Modified: Thu, 09 Feb 2023 10:29:45 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0040ed7dfbdfee4a72e6b3938e39a2359baf268b638943f06a2e8a81ef7ca812`  
		Last Modified: Thu, 09 Feb 2023 10:29:45 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00bc6becd14133907db6e2043ac3118a066c39d1a0b21222f43dc0013e6735e`  
		Last Modified: Tue, 14 Feb 2023 20:56:44 GMT  
		Size: 12.5 MB (12538235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b7261072626daff0a7896b545cc67aa39ac3c21899918a44a1f3550b5b9ae7`  
		Last Modified: Tue, 14 Feb 2023 20:56:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b0a722938be400fa485e623df741cf9c7c3a449e58e94cbe48cc689c6cd816`  
		Last Modified: Tue, 14 Feb 2023 20:56:43 GMT  
		Size: 10.1 MB (10066545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d08bcff2aec58754c9ea47474bedf896e81eaac57fe269033dd4abc38203c30`  
		Last Modified: Tue, 14 Feb 2023 20:56:41 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6bddf40c3ba1c0096109588750048e6cff22cf6ceb6eff84a7b01f183fc012`  
		Last Modified: Tue, 14 Feb 2023 20:56:41 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4159e979f1c688d395fdaed95ace82537dae2811aa24e6948d4f52b3d4a854d0`  
		Last Modified: Tue, 14 Feb 2023 20:56:41 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48a42a051a214d066c1cd069a7def610ba36bc3ebb97cd80e20a47d5af632ce`  
		Last Modified: Tue, 14 Feb 2023 23:31:30 GMT  
		Size: 150.7 KB (150730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c37bb3807a6f153a998f28d38daee1247ae1e404fb97f5df2cff2be238f4ec8`  
		Last Modified: Tue, 14 Feb 2023 23:31:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbc15059f1f320b92730d70ab52cd1a4cd9c6e5326f58aeab6cd26aa60d9234`  
		Last Modified: Tue, 14 Feb 2023 23:31:28 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e580904190c7db849000f34ff67ac8a19f0c42e90b3e6ae2909daa21dfef15`  
		Last Modified: Tue, 14 Feb 2023 23:31:29 GMT  
		Size: 3.9 MB (3903530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1395bcc87a96a4a8cb3b8162ec7f2ed6ad2a1d71f6aab44f859f5b051430856c`  
		Last Modified: Tue, 14 Feb 2023 23:31:28 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eab323d54626cff6802c0777e6ea9e8b9bf13d3f08c86131adc6d408cfd13c`  
		Last Modified: Tue, 14 Feb 2023 23:31:28 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e21d58fa10cde3ba67de43b3f6ecd494955572755c3cda0d3ec7422d95442c`  
		Last Modified: Tue, 14 Feb 2023 23:31:28 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; arm variant v7

```console
$ docker pull yourls@sha256:c8afe589907d231498c488fb7230653c6f278a886b6f48a2e05805aedd8c17e6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139640653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0df88a642740fdaeb96648b70fbb87ba55628cfdd367cb551a05961c499a2064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:47:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 08:47:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 08:47:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 08:47:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 08:47:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 08:51:36 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 08:51:36 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 08:51:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 08:51:47 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 08:51:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 08:51:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 08:51:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 08:51:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 09:19:17 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 09 Feb 2023 09:19:18 GMT
ENV PHP_VERSION=8.1.15
# Thu, 09 Feb 2023 09:19:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Thu, 09 Feb 2023 09:19:18 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Thu, 09 Feb 2023 09:19:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Feb 2023 09:19:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Feb 2023 09:22:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Feb 2023 09:22:14 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Feb 2023 09:22:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Feb 2023 09:22:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Feb 2023 09:22:14 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Feb 2023 09:22:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Feb 2023 09:22:15 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 09:22:15 GMT
EXPOSE 80
# Thu, 09 Feb 2023 09:22:15 GMT
CMD ["apache2-foreground"]
# Thu, 09 Feb 2023 20:09:33 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 09 Feb 2023 20:09:33 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 09 Feb 2023 20:09:33 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 09 Feb 2023 20:09:34 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 09 Feb 2023 20:09:34 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 09 Feb 2023 20:09:34 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 09 Feb 2023 20:09:34 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 09 Feb 2023 20:09:34 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 09 Feb 2023 20:09:54 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 09 Feb 2023 20:09:54 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 09 Feb 2023 20:09:55 GMT
RUN a2enmod rewrite expires
# Thu, 09 Feb 2023 20:09:55 GMT
ARG YOURLS_VERSION=1.9.1
# Thu, 09 Feb 2023 20:09:55 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 09 Feb 2023 20:09:55 GMT
LABEL org.opencontainers.image.version=1.9.1
# Thu, 09 Feb 2023 20:09:55 GMT
ENV YOURLS_VERSION=1.9.1
# Thu, 09 Feb 2023 20:09:55 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 09 Feb 2023 20:09:57 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 09 Feb 2023 20:09:57 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 09 Feb 2023 20:09:57 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 09 Feb 2023 20:09:58 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 09 Feb 2023 20:09:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 20:09:58 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62799bf19ad9233ac3078e8cc582836e83b92de17042cedcf5dc1da7a98f23a`  
		Last Modified: Thu, 09 Feb 2023 10:17:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6564f926ab623011cf9b95ae4137b43cb32a02e52377138cd1ec6e9683597`  
		Last Modified: Thu, 09 Feb 2023 10:17:42 GMT  
		Size: 69.3 MB (69321683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8102ba0459df46db99ce3cd44312aa557923b4610cc04cddec86c41075105d69`  
		Last Modified: Thu, 09 Feb 2023 10:17:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcbe745ec014b053fb8fd558cfde42215939adae6b881d143e170158a025a6d1`  
		Last Modified: Thu, 09 Feb 2023 10:18:46 GMT  
		Size: 18.0 MB (17997699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46e898255cee1efe198dd646991396eca07d684f76272d8da6d2a8ad1ed1ebc`  
		Last Modified: Thu, 09 Feb 2023 10:18:42 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153eb903be4f793435dc74527c652d3736cc5b45b739f049c039ea29d00e609f`  
		Last Modified: Thu, 09 Feb 2023 10:18:42 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b14a24e3173b2792d99fbc3bebf5bbd91602a6caf297738f4837067f7df41b3`  
		Last Modified: Thu, 09 Feb 2023 10:23:50 GMT  
		Size: 12.2 MB (12153048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abf9b8920518f75dc149630c351b05836dcf6e53c04626aec316aafc784a37c`  
		Last Modified: Thu, 09 Feb 2023 10:23:47 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5481b8ced1560d661532049bd4de59edb65064b0c53b78b6270a694e2df5944`  
		Last Modified: Thu, 09 Feb 2023 10:23:49 GMT  
		Size: 9.5 MB (9538563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d02f589e02c4161febc0732294f55fa539d11d52bc1b96361c420e33cbdafb`  
		Last Modified: Thu, 09 Feb 2023 10:23:47 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c76e7db84822bbc32a16fc5b251ec424be2a33bf8aeb6c81848a530ff37c00`  
		Last Modified: Thu, 09 Feb 2023 10:23:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c49d9c7daa96ec75800f961628589908a0f432bf7f4ec9fd576a4622ce81b8`  
		Last Modified: Thu, 09 Feb 2023 10:23:47 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b76da7c7c16e4bd86d3bd7b3586821caeee54aed6faabeb5206b75f5613144`  
		Last Modified: Thu, 09 Feb 2023 20:11:26 GMT  
		Size: 138.4 KB (138385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b966d7beccfeafb41b40791aec3e0e6b09b7846c6a44e1ec4e5d6a627972655e`  
		Last Modified: Thu, 09 Feb 2023 20:11:26 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab445935e80aab05dd4b207b0ac51a27d6e86014267cb2af9080e9f10d100fa`  
		Last Modified: Thu, 09 Feb 2023 20:11:23 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8993b56fc078d7580e1101364411cff561525cafada2c56e0281296820127d`  
		Last Modified: Thu, 09 Feb 2023 20:11:24 GMT  
		Size: 3.9 MB (3903534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef247a21e267aff551772620f1ce40cf6759fd3534b15ae2723e87f1cf3f2059`  
		Last Modified: Thu, 09 Feb 2023 20:11:23 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1ffa30397256af3e45052d199b870e634e9383459c5c3a6acfa4ba4aac0c7e`  
		Last Modified: Thu, 09 Feb 2023 20:11:23 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5d7da52b4852d9ca81b68cdd41994cc2b446af4957fadf0c5bd50ed8eac80f`  
		Last Modified: Thu, 09 Feb 2023 20:11:23 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:f55ed74bd21545f56c5e004971ac770de87cc6a4a8dd5df8c9ff29925ef31260
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.5 MB (164517299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c855d958e4feb87c52932e919894ca88714f85d9e272b0c4d036f387a362119`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 05:27:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 05:27:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 05:27:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 05:27:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 05:27:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 05:30:33 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 05:30:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 05:30:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 05:30:40 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 05:30:41 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 05:30:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:30:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:30:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 05:55:32 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:37:32 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:37:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Tue, 14 Feb 2023 21:37:32 GMT
ENV PHP_SHA256=7108b7347981ad6e610aaf3b3fb0f6444019ab6f59a872c1b55a29bc753eba93
# Tue, 14 Feb 2023 21:37:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 14 Feb 2023 21:37:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:40:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 21:40:30 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:40:31 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 21:40:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 21:40:31 GMT
STOPSIGNAL SIGWINCH
# Tue, 14 Feb 2023 21:40:31 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:40:31 GMT
WORKDIR /var/www/html
# Tue, 14 Feb 2023 21:40:31 GMT
EXPOSE 80
# Tue, 14 Feb 2023 21:40:31 GMT
CMD ["apache2-foreground"]
# Wed, 15 Feb 2023 02:13:05 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 15 Feb 2023 02:13:05 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 15 Feb 2023 02:13:05 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 15 Feb 2023 02:13:06 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 15 Feb 2023 02:13:06 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 15 Feb 2023 02:13:06 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 15 Feb 2023 02:13:06 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 15 Feb 2023 02:13:06 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 15 Feb 2023 02:13:59 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 15 Feb 2023 02:14:00 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 15 Feb 2023 02:14:00 GMT
RUN a2enmod rewrite expires
# Wed, 15 Feb 2023 02:14:01 GMT
ARG YOURLS_VERSION=1.9.1
# Wed, 15 Feb 2023 02:14:01 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 15 Feb 2023 02:14:01 GMT
LABEL org.opencontainers.image.version=1.9.1
# Wed, 15 Feb 2023 02:14:01 GMT
ENV YOURLS_VERSION=1.9.1
# Wed, 15 Feb 2023 02:14:01 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 15 Feb 2023 02:14:03 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 15 Feb 2023 02:14:03 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 15 Feb 2023 02:14:03 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 15 Feb 2023 02:14:03 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 15 Feb 2023 02:14:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Feb 2023 02:14:03 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbb2734b4952adc9c052061ffab6144238949bcbf2bf5234b71bba52f01e330`  
		Last Modified: Thu, 09 Feb 2023 06:37:24 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea02c4abdd5e6e36a734a5f78a3688e52b8c01015ef8a12ea244607e82fcba02`  
		Last Modified: Thu, 09 Feb 2023 06:37:35 GMT  
		Size: 86.9 MB (86928495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155431a8265f1bc742a122e275f209cbf6bdd3d1cdfcd423ca23920f97e07692`  
		Last Modified: Thu, 09 Feb 2023 06:37:24 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4401994bce70edbeb8d86c6961f64e28ab1dd5049c63f3cbc09a18459b4a6e27`  
		Last Modified: Thu, 09 Feb 2023 06:38:20 GMT  
		Size: 19.2 MB (19166292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783039378940c2f3342c2c4818a6a0b98502ea55870557e699d119417d6ad5e4`  
		Last Modified: Thu, 09 Feb 2023 06:38:18 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b408a32a67e7c8012d2420c99d5faebd3b6b1496b9cdabb7c3ab9bc3ffb964dc`  
		Last Modified: Thu, 09 Feb 2023 06:38:18 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ab904b620952ab6f8b508b8901e2adba3afd810d76b9476bc627300980f789`  
		Last Modified: Tue, 14 Feb 2023 22:58:20 GMT  
		Size: 12.5 MB (12538936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13968607eb4c4df3d575cfab07c336783748aadbb1cb0831f8d672e984dd0756`  
		Last Modified: Tue, 14 Feb 2023 22:58:17 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c77181103f9f5bd01e672348a0b5f49a72dbb4b9bfb654dce7bc1fa9f3513e`  
		Last Modified: Tue, 14 Feb 2023 22:58:19 GMT  
		Size: 11.1 MB (11114050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cfe6faa09554da5fa7eb43f291fdea7edd551f55108315ec5d210f973d9046f`  
		Last Modified: Tue, 14 Feb 2023 22:58:17 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d54a66caa9e6ad6329ceecd93e9693f9cc5e5876f08dc3ec13bb08f79f533e9`  
		Last Modified: Tue, 14 Feb 2023 22:58:17 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5748eeb5dc48ed6ee2339a23806b6a478718aef987af4b46122d695636742ed4`  
		Last Modified: Tue, 14 Feb 2023 22:58:17 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8da1ddff5bc8d1552ed7d8932e90398b01d3d27def7876426284bf6ed99e2d`  
		Last Modified: Wed, 15 Feb 2023 02:17:08 GMT  
		Size: 793.3 KB (793288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5fd1b5bb29e700b8bed344c3e4d07e27833321b449145c33516c8e95543b85`  
		Last Modified: Wed, 15 Feb 2023 02:17:08 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c5b5168796350030b235b027d72d1dad283072831e7f8e3ae039f1a17f41a3`  
		Last Modified: Wed, 15 Feb 2023 02:17:06 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314d5e241843ded587c505c29f1dc8eb72fa93051c3cabb66b302037020caa9e`  
		Last Modified: Wed, 15 Feb 2023 02:17:07 GMT  
		Size: 3.9 MB (3903533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012028f6ea111a41c8ecd1d1c043b12b80dacc93a3d4c0459d087e9c1362924d`  
		Last Modified: Wed, 15 Feb 2023 02:17:06 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d6d50e2e1a8e3198d9478799013e0da23c52ddbf3918129208f3c44115aa86`  
		Last Modified: Wed, 15 Feb 2023 02:17:06 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcff9125ad57efb34cbefe374638dc4857036395531f5419336a25693fe9f1aa`  
		Last Modified: Wed, 15 Feb 2023 02:17:06 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; 386

```console
$ docker pull yourls@sha256:677eefad7687463e68db7939aac9211ac4b755e5e0061519369f007d1f7259d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.1 MB (172050392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bb7cbe5365ca32dc3483413ee0c56fbe3adf4718a5907f854e6b994f2c5273c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:35:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 06:35:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 06:35:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:35:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 06:35:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 06:38:50 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 06:38:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 06:39:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 06:39:02 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 06:39:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 06:39:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 06:39:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 06:39:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 07:05:22 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 09 Feb 2023 07:05:22 GMT
ENV PHP_VERSION=8.1.15
# Thu, 09 Feb 2023 07:05:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Thu, 09 Feb 2023 07:05:24 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Thu, 09 Feb 2023 07:05:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Feb 2023 07:05:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:08:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Feb 2023 07:08:25 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:08:25 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Feb 2023 07:08:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Feb 2023 07:08:27 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Feb 2023 07:08:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Feb 2023 07:08:29 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 07:08:30 GMT
EXPOSE 80
# Thu, 09 Feb 2023 07:08:31 GMT
CMD ["apache2-foreground"]
# Thu, 09 Feb 2023 20:07:37 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 09 Feb 2023 20:07:37 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 09 Feb 2023 20:07:38 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 09 Feb 2023 20:07:39 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 09 Feb 2023 20:07:40 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 09 Feb 2023 20:07:41 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 09 Feb 2023 20:07:42 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 09 Feb 2023 20:07:43 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 09 Feb 2023 20:08:20 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 09 Feb 2023 20:08:21 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 09 Feb 2023 20:08:22 GMT
RUN a2enmod rewrite expires
# Thu, 09 Feb 2023 20:08:23 GMT
ARG YOURLS_VERSION=1.9.1
# Thu, 09 Feb 2023 20:08:24 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 09 Feb 2023 20:08:25 GMT
LABEL org.opencontainers.image.version=1.9.1
# Thu, 09 Feb 2023 20:08:26 GMT
ENV YOURLS_VERSION=1.9.1
# Thu, 09 Feb 2023 20:08:27 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 09 Feb 2023 20:08:30 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 09 Feb 2023 20:08:31 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 09 Feb 2023 20:08:32 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 09 Feb 2023 20:08:33 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 09 Feb 2023 20:08:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 09 Feb 2023 20:08:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d813867a2f676dc535176f61e52aa3a440060fe71341c0ecca003ff22f1e52`  
		Last Modified: Thu, 09 Feb 2023 07:58:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d0c09cb272ba4eef1c58df4e5b9432ea523cfe1a0ccd5b746fcbb378affe7e`  
		Last Modified: Thu, 09 Feb 2023 07:58:41 GMT  
		Size: 92.5 MB (92510382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3105d7eab02cfecefb73c028462dbe22304a988e6668a5d2cb50dd6cb7309bc`  
		Last Modified: Thu, 09 Feb 2023 07:58:28 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08f8c23fb90df65a0c19e725e1b757a8502e1184754f9c3879d380c84e472c4`  
		Last Modified: Thu, 09 Feb 2023 07:59:37 GMT  
		Size: 19.5 MB (19515912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d5cf4926133f0a7d660ef193a654eb59ac640961472b3d9b78a40b5cae326f`  
		Last Modified: Thu, 09 Feb 2023 07:59:34 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d84a4bf50c27a4ac50195b93b27833d5b0ac38e383199a8a3e41af9f2b89a6`  
		Last Modified: Thu, 09 Feb 2023 07:59:34 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92fb05863305abd51d8bffbd4dd060a2d5c02b29d0fe8b77e38060ceb46f6dc`  
		Last Modified: Thu, 09 Feb 2023 08:04:14 GMT  
		Size: 11.9 MB (11939257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34376fe8b61f9d00b54b40d69fa9c06f1ec84bbf166ddb22075bd79f129307b7`  
		Last Modified: Thu, 09 Feb 2023 08:04:10 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7a92c83ff59e2950223777fb002e59ac2173b63f0ed29ffb7a452c6df97ee2`  
		Last Modified: Thu, 09 Feb 2023 08:04:12 GMT  
		Size: 11.3 MB (11279557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386bf1aca35f4e3c7d574596683addfb8402a4ff17b9c6e531547dc85b9ae242`  
		Last Modified: Thu, 09 Feb 2023 08:04:11 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf1ffacd4159b2361d790091446aa14778edb5224633aadaf2840f76a053365`  
		Last Modified: Thu, 09 Feb 2023 08:04:10 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e6bf857489be07ad61a97b52b5e67a82f28efd2a519c2c2cc131bda7f10787`  
		Last Modified: Thu, 09 Feb 2023 08:04:10 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280500e42cab72d4496613f38583039ad04ffd8bddff4fb87908e5e86879f11d`  
		Last Modified: Thu, 09 Feb 2023 20:10:29 GMT  
		Size: 494.9 KB (494920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42ec325a36481eeee0974d6b205f2f12ea913c4daffdd6d6dbb78acee43258f`  
		Last Modified: Thu, 09 Feb 2023 20:10:28 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e3f97df37e4d27b2ea3e8e5fef7dd24ef0f0ccbae85c59ab14831f92c88373`  
		Last Modified: Thu, 09 Feb 2023 20:10:27 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa76db03ecbf6254b9b35c2428b223c49b3e81588250b1bb0bd975b08cb41de1`  
		Last Modified: Thu, 09 Feb 2023 20:10:27 GMT  
		Size: 3.9 MB (3903427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20ac835f7f1e6e2c8502b49d48ba913312cb05974906890b8be6d9a79e6ba73`  
		Last Modified: Thu, 09 Feb 2023 20:10:26 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d726f647cf2edfc5b7646e2fc470cfe7f9d6e560426e39dac7b7bdeaa8659a25`  
		Last Modified: Thu, 09 Feb 2023 20:10:26 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280efa23c2ac59400111ff39ccbb91e0151bb946eb2147b4265784bcc0c958a4`  
		Last Modified: Thu, 09 Feb 2023 20:10:26 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; mips64le

```console
$ docker pull yourls@sha256:7d06ba04e522accde1aae454fb17d30516f333592a4111c29eadfbbe53fd89b8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.6 MB (146586304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb26f9cf98664d57f97f75940a94a51d4cf15db0053ed0373cf79a8468c1997c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 02:45:21 GMT
ADD file:68e11645a37c49c8f8f9d79ba579d0d192aaab78bb28059f07d69d56aa5ace71 in / 
# Thu, 09 Feb 2023 02:45:25 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 16:47:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 16:47:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 16:48:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 16:49:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 16:49:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 17:03:45 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 17:03:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 17:04:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 17:04:49 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 17:04:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 17:04:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 17:05:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 17:05:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 18:02:21 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 09 Feb 2023 18:02:25 GMT
ENV PHP_VERSION=8.1.15
# Thu, 09 Feb 2023 18:02:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.15.tar.xz.asc
# Thu, 09 Feb 2023 18:02:32 GMT
ENV PHP_SHA256=cd450fb4ee50488c5bf5f08851f514e5a1cac18c9512234d9e16c3a1d35781a6
# Thu, 09 Feb 2023 18:03:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Feb 2023 18:03:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Feb 2023 18:16:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Feb 2023 18:16:58 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Feb 2023 18:17:03 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Feb 2023 18:17:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Feb 2023 18:17:10 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Feb 2023 18:17:13 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Feb 2023 18:17:16 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 18:17:20 GMT
EXPOSE 80
# Thu, 09 Feb 2023 18:17:23 GMT
CMD ["apache2-foreground"]
# Fri, 10 Feb 2023 07:39:53 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 10 Feb 2023 07:39:57 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 10 Feb 2023 07:40:00 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 10 Feb 2023 07:40:04 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 10 Feb 2023 07:40:07 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 10 Feb 2023 07:40:11 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 10 Feb 2023 07:40:14 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 10 Feb 2023 07:40:18 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Fri, 10 Feb 2023 07:41:23 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 10 Feb 2023 07:41:29 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Feb 2023 07:41:35 GMT
RUN a2enmod rewrite expires
# Fri, 10 Feb 2023 07:41:39 GMT
ARG YOURLS_VERSION=1.9.1
# Fri, 10 Feb 2023 07:41:42 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 10 Feb 2023 07:41:46 GMT
LABEL org.opencontainers.image.version=1.9.1
# Fri, 10 Feb 2023 07:41:50 GMT
ENV YOURLS_VERSION=1.9.1
# Fri, 10 Feb 2023 07:41:53 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Fri, 10 Feb 2023 07:42:02 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 10 Feb 2023 07:42:06 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 10 Feb 2023 07:42:09 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 10 Feb 2023 07:42:12 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 10 Feb 2023 07:42:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 07:42:19 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1b5516936229d6629ab88588210eb90edc2613c94e5952fd1caf9200284f298a`  
		Last Modified: Thu, 09 Feb 2023 02:53:48 GMT  
		Size: 29.6 MB (29634449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cadf458950d68867a313d27047074490e6171bb745a965ecd2270a62a6934fe`  
		Last Modified: Thu, 09 Feb 2023 19:40:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02e1e2a67f8dc04dd6155300edf3d8403e5bfd3243879a434ac158b8245e25d`  
		Last Modified: Thu, 09 Feb 2023 19:41:36 GMT  
		Size: 71.8 MB (71814207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fdb53a8ae5f57cf6956c9c7d61c643b363e8bf124074dc3f947417f88179a5`  
		Last Modified: Thu, 09 Feb 2023 19:40:43 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec3be553467c6abeb517848cfbf09f534836a4df0eeb83578c93f70cdc0cf99`  
		Last Modified: Thu, 09 Feb 2023 19:42:34 GMT  
		Size: 18.9 MB (18940133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d6b705ab88191ed5bdcb4df3a783d8271e2d3551ec73b6be94124f022d4517`  
		Last Modified: Thu, 09 Feb 2023 19:42:21 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a981839164a03991185f134706096ac5759f76c64058b9147ecedfc64dd9430`  
		Last Modified: Thu, 09 Feb 2023 19:42:21 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92568e4d4d16773eeefccb05e05a8472a71ef51f7546309f63271787c748d828`  
		Last Modified: Thu, 09 Feb 2023 19:45:14 GMT  
		Size: 11.9 MB (11938162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a041b34aa724c2e57b0af2ea999e2ada6f8aa0a2c3fcd6168b4ed46b45b8f9`  
		Last Modified: Thu, 09 Feb 2023 19:45:08 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27274202991c680607f4a2a5fd47a6ce6a2c1e378a11cd4b0c46cc6308ca804d`  
		Last Modified: Thu, 09 Feb 2023 19:45:17 GMT  
		Size: 10.2 MB (10196849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f992f52b151df9dfe629e6a75336eae215f4db4a680dd1addfa239a1904b8a8`  
		Last Modified: Thu, 09 Feb 2023 19:45:08 GMT  
		Size: 2.5 KB (2464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f620b3be1f4c7c9a9a9b483a12bec6ec4e803e6b6c78f07a34fa48531588b0`  
		Last Modified: Thu, 09 Feb 2023 19:45:08 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12dc73e02279e6d1f2fcf227477fc2a2e92cb6ea209e835eede1d415ee484de3`  
		Last Modified: Thu, 09 Feb 2023 19:45:09 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac636e42518da4d625916bd0f2f9382f57cda2a21432ca4cb939a323f4cd0cb`  
		Last Modified: Fri, 10 Feb 2023 07:45:16 GMT  
		Size: 149.0 KB (148975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbc59f9f886c4079a5d9c1a11387d8e438dd2edf3e50cbe7fd43100a38583bd`  
		Last Modified: Fri, 10 Feb 2023 07:45:16 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52aa4da941fb9fdc8df2185eabe3991d5618c83f8e2607e5fff98fafd8ac1a9b`  
		Last Modified: Fri, 10 Feb 2023 07:45:13 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f04441fd60f6f074ac58881d791f7e39528628d07edb98501e696c73320aac0e`  
		Last Modified: Fri, 10 Feb 2023 07:45:17 GMT  
		Size: 3.9 MB (3903427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a282735521e732c32e92c8874510366b3d3c2ec87ebb6cef1abc141be73313`  
		Last Modified: Fri, 10 Feb 2023 07:45:13 GMT  
		Size: 2.1 KB (2057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525326da3ba66d962cbf208723fcf63f7bdc2cc921fb15acb2af7ffd29a7155c`  
		Last Modified: Fri, 10 Feb 2023 07:45:14 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2df03fa7d1939e2c4ecae975602e185c8bce3295e78436e052199faf7d83d8`  
		Last Modified: Fri, 10 Feb 2023 07:45:13 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; ppc64le

```console
$ docker pull yourls@sha256:66c95f966029daf3b2068f7017525a65c49c19563daf4f631108eecc87d18a37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.5 MB (170470703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42e4c0f35fb61fd0c272ba1a15e656d380aa2329b6f1fe899c29f3bc397d84cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:19:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 10:19:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 10:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:20:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 10:20:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 10:25:21 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 10:25:21 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 10:25:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 10:25:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 10:25:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 10:25:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 10:25:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 10:25:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 10:44:01 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:09:06 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:09:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Tue, 14 Feb 2023 21:09:07 GMT
ENV PHP_SHA256=7108b7347981ad6e610aaf3b3fb0f6444019ab6f59a872c1b55a29bc753eba93
# Tue, 14 Feb 2023 21:09:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 14 Feb 2023 21:09:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:13:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 21:13:52 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:13:53 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 21:13:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 21:13:54 GMT
STOPSIGNAL SIGWINCH
# Tue, 14 Feb 2023 21:13:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:13:55 GMT
WORKDIR /var/www/html
# Tue, 14 Feb 2023 21:13:55 GMT
EXPOSE 80
# Tue, 14 Feb 2023 21:13:56 GMT
CMD ["apache2-foreground"]
# Wed, 15 Feb 2023 01:41:50 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 15 Feb 2023 01:41:51 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 15 Feb 2023 01:41:51 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 15 Feb 2023 01:41:52 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 15 Feb 2023 01:41:52 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 15 Feb 2023 01:41:53 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 15 Feb 2023 01:41:53 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 15 Feb 2023 01:41:54 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 15 Feb 2023 01:42:32 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 15 Feb 2023 01:42:34 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 15 Feb 2023 01:42:36 GMT
RUN a2enmod rewrite expires
# Wed, 15 Feb 2023 01:42:36 GMT
ARG YOURLS_VERSION=1.9.1
# Wed, 15 Feb 2023 01:42:37 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 15 Feb 2023 01:42:38 GMT
LABEL org.opencontainers.image.version=1.9.1
# Wed, 15 Feb 2023 01:42:40 GMT
ENV YOURLS_VERSION=1.9.1
# Wed, 15 Feb 2023 01:42:40 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 15 Feb 2023 01:42:45 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 15 Feb 2023 01:42:46 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 15 Feb 2023 01:42:47 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 15 Feb 2023 01:42:47 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 15 Feb 2023 01:42:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Feb 2023 01:42:49 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43232fc55c8ccbdec23837fdbabf8a55f62e81b11637630eb5c442a99b423f4c`  
		Last Modified: Thu, 09 Feb 2023 11:19:20 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878184cd9e854f6d9186e01d93ec972e9536692520fdcf2fcaf34c63b608a9a3`  
		Last Modified: Thu, 09 Feb 2023 11:19:44 GMT  
		Size: 86.6 MB (86632950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939821d7ebd845237190718862054b702fa19155bf8e8a7adb0a6f6e0f5f2b05`  
		Last Modified: Thu, 09 Feb 2023 11:19:20 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7a5569e8426ebb50945fd299464662c8f6adbecf2c4f8ef832213db148e501`  
		Last Modified: Thu, 09 Feb 2023 11:20:47 GMT  
		Size: 20.5 MB (20464261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4c25ec3e4a74374c161176fdbb8910da748fa93eb591d056795427d835ef1d`  
		Last Modified: Thu, 09 Feb 2023 11:20:42 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cda695f67a14b99a7baa06d0458a1e729e550a93626a80af8acd5afcc52d61`  
		Last Modified: Thu, 09 Feb 2023 11:20:42 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a39ed6226f0403d6a518fd77a2834d3dae8906ea92b1e0aa13bc72a7f302a3`  
		Last Modified: Tue, 14 Feb 2023 22:36:23 GMT  
		Size: 12.5 MB (12539593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85e842997f4d7d7e02b38ebe8e34ef56b5e81b9a2b53fcda0c7a4580b30217a`  
		Last Modified: Tue, 14 Feb 2023 22:36:19 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6509e946390d6e2f51f6be000492b29f18c43672a2a1090708f08efcec47f3ce`  
		Last Modified: Tue, 14 Feb 2023 22:36:23 GMT  
		Size: 11.4 MB (11447074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eaa76a414b1d3ba041248880d027e9294f43d7b37db8b7a78be18738648ed2`  
		Last Modified: Tue, 14 Feb 2023 22:36:19 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bbaef89a052b2bc96000c5f67b6adeb7426bf6fd288e69d8012dcdb0bc978b`  
		Last Modified: Tue, 14 Feb 2023 22:36:19 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532606be9959274abe1d31a47f16ae414bc1c0fe85f9b9dfb88e54c21145f4b1`  
		Last Modified: Tue, 14 Feb 2023 22:36:19 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f093ed742ecd91b84e316d58765dae602c1c4e37bdc3ec5bbf1fc21827c54a09`  
		Last Modified: Wed, 15 Feb 2023 01:45:55 GMT  
		Size: 183.8 KB (183832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee047438151229d559b27f52f0d5028cba654c6cd32b0c0432f7b8b444c46ed`  
		Last Modified: Wed, 15 Feb 2023 01:45:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5bbb160ee3d4742b5afb74860e88aa95857e7ae37a30fd6dccc9a96b2f90fe`  
		Last Modified: Wed, 15 Feb 2023 01:45:52 GMT  
		Size: 350.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245f661a174f9ac9ee5628ea75c8e0bd920b622b4413d9fe1c8880e7aec0de11`  
		Last Modified: Wed, 15 Feb 2023 01:45:53 GMT  
		Size: 3.9 MB (3903532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c729147a5ba38e80e03508229f8fb07cb54807dfb85d7cffe6ffcc895ed7ab7c`  
		Last Modified: Wed, 15 Feb 2023 01:45:52 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e948ef5ba5c89019a66fa93b552bba839dd85f16760695e98a5fd8bab6b7861d`  
		Last Modified: Wed, 15 Feb 2023 01:45:52 GMT  
		Size: 1.6 KB (1560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9d92b9791d90158e576564ca2c26fad9c61667ddd3a82137b25cc720d6e92d`  
		Last Modified: Wed, 15 Feb 2023 01:45:52 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; s390x

```console
$ docker pull yourls@sha256:b6cf319dbb1e0aae3436e788443d4cb5aed0b65e3891a67dff3daa461f0d91d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.1 MB (147143910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694b6e56de704233bb8ede213d4be32fdad9466e1c110eb33bc544925bdc43a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:45 GMT
ADD file:dc3c16b50baeac5b9644e607c8df9606e9583f8598e3ba34bcdd69c669a5904c in / 
# Thu, 09 Feb 2023 02:41:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 05:19:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 05:19:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 05:20:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 05:20:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 05:20:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 05:25:31 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 05:25:31 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 05:25:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 05:25:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 05:25:47 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 05:25:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:25:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:25:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 05:45:05 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:27:08 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:27:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Tue, 14 Feb 2023 21:27:08 GMT
ENV PHP_SHA256=7108b7347981ad6e610aaf3b3fb0f6444019ab6f59a872c1b55a29bc753eba93
# Tue, 14 Feb 2023 21:27:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 14 Feb 2023 21:27:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:29:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 21:29:22 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:29:23 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 21:29:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 21:29:23 GMT
STOPSIGNAL SIGWINCH
# Tue, 14 Feb 2023 21:29:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 14 Feb 2023 21:29:24 GMT
WORKDIR /var/www/html
# Tue, 14 Feb 2023 21:29:24 GMT
EXPOSE 80
# Tue, 14 Feb 2023 21:29:24 GMT
CMD ["apache2-foreground"]
# Wed, 15 Feb 2023 01:06:41 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 15 Feb 2023 01:06:41 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 15 Feb 2023 01:06:41 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 15 Feb 2023 01:06:41 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 15 Feb 2023 01:06:42 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 15 Feb 2023 01:06:42 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 15 Feb 2023 01:06:42 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 15 Feb 2023 01:06:42 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 15 Feb 2023 01:06:55 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 15 Feb 2023 01:06:55 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 15 Feb 2023 01:06:56 GMT
RUN a2enmod rewrite expires
# Wed, 15 Feb 2023 01:06:56 GMT
ARG YOURLS_VERSION=1.9.1
# Wed, 15 Feb 2023 01:06:56 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 15 Feb 2023 01:06:56 GMT
LABEL org.opencontainers.image.version=1.9.1
# Wed, 15 Feb 2023 01:06:56 GMT
ENV YOURLS_VERSION=1.9.1
# Wed, 15 Feb 2023 01:06:56 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 15 Feb 2023 01:06:58 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 15 Feb 2023 01:06:58 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 15 Feb 2023 01:06:58 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 15 Feb 2023 01:06:59 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 15 Feb 2023 01:06:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Feb 2023 01:06:59 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c2f78940fdfbfc5ce5d1d3cff3c27a319451aeb3ec12ff2473073516907fbce9`  
		Last Modified: Thu, 09 Feb 2023 02:46:06 GMT  
		Size: 29.6 MB (29647513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3df263a1c9e1be6bb9ae8d3128a5b370055484fccdb14fb616c797eb10b605`  
		Last Modified: Thu, 09 Feb 2023 06:13:38 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12a22024ac2b88388a15678ebf2257c430a770dbc92181a3d46ee4a6e7925c2`  
		Last Modified: Thu, 09 Feb 2023 06:13:48 GMT  
		Size: 71.6 MB (71628890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d91b6fd48d29a549f5f9e77d78578b0a170890a62eaf70107d6f4a80126cba0`  
		Last Modified: Thu, 09 Feb 2023 06:13:38 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46ec046fc8903c85a12c9c8c61db044bb40931eb7405e5f31266b87ef480922`  
		Last Modified: Thu, 09 Feb 2023 06:14:23 GMT  
		Size: 19.1 MB (19072273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a3cccefc82c4ed82bb1808bdbbe8937b84723ddc35929d41b619ad61b8912dc`  
		Last Modified: Thu, 09 Feb 2023 06:14:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e10114ab4dab1689ab15f5c09c932fc512030217b27d6999d48ec1e6a2b4e86`  
		Last Modified: Thu, 09 Feb 2023 06:14:20 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc479b5eca471df7d1af798d75de395c84f8108d40f0b0c5c114269807c7421`  
		Last Modified: Tue, 14 Feb 2023 22:20:41 GMT  
		Size: 12.5 MB (12538762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a2a677c592ea3a6cc2e43f8ba150d130e2ae305172b4fa8d09d828e7c531e06`  
		Last Modified: Tue, 14 Feb 2023 22:20:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca896e6df8b8038f916492a7eec0a2560b0ca848e0473911b8cb1ca85b5f67c4`  
		Last Modified: Tue, 14 Feb 2023 22:20:41 GMT  
		Size: 10.2 MB (10184545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d236806aedb3c622337ad9d0da6d69ceacce746cb28799d01fa5c8f8c8129d08`  
		Last Modified: Tue, 14 Feb 2023 22:20:40 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c35ec202e9e110c7a8d3b8092531777aaace30bde291d21e286d8292d757c8f`  
		Last Modified: Tue, 14 Feb 2023 22:20:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d75e09960985be770e3a8990cb1ca3046fc89d0da4200fc2bfe54b47dac388`  
		Last Modified: Tue, 14 Feb 2023 22:20:40 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59486bf4c4718b3ecd1f59c6a9db9d22609f667d0019b26663f8df8bf3968ca`  
		Last Modified: Wed, 15 Feb 2023 01:08:29 GMT  
		Size: 158.2 KB (158201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3505b569fba601a546cabefd0df7fdd9019c5bd7c80772671cbb171b83ce8f`  
		Last Modified: Wed, 15 Feb 2023 01:08:29 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eb80db5c71bd128b0dbd28bb49cc051f59d7fee611ad3b86ceaa607810c52b`  
		Last Modified: Wed, 15 Feb 2023 01:08:28 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7af35d2b6925448ceb2274e9c63ea56851492ba6b4738d4d99e3c251e3fe1f6`  
		Last Modified: Wed, 15 Feb 2023 01:08:29 GMT  
		Size: 3.9 MB (3903534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62e5460c856ca9e97fb574e7b9ed58ac7678294c8d785b32217157e752d09c6`  
		Last Modified: Wed, 15 Feb 2023 01:08:28 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7770a94fc3f5224be7f343e133c8484da9c1b89827ca136ab2846249aeaa96`  
		Last Modified: Wed, 15 Feb 2023 01:08:28 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb379a0b359e9c4e222af61397871fa1eb323d74d2deffc04965ec664b6070e`  
		Last Modified: Wed, 15 Feb 2023 01:08:28 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
