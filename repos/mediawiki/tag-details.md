<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mediawiki`

-	[`mediawiki:1.31`](#mediawiki131)
-	[`mediawiki:1.31.6`](#mediawiki1316)
-	[`mediawiki:1.33`](#mediawiki133)
-	[`mediawiki:1.33.2`](#mediawiki1332)
-	[`mediawiki:1.34`](#mediawiki134)
-	[`mediawiki:1.34.0`](#mediawiki1340)
-	[`mediawiki:latest`](#mediawikilatest)
-	[`mediawiki:legacy`](#mediawikilegacy)
-	[`mediawiki:legacylts`](#mediawikilegacylts)
-	[`mediawiki:lts`](#mediawikilts)
-	[`mediawiki:stable`](#mediawikistable)

## `mediawiki:1.31`

```console
$ docker pull mediawiki@sha256:278a7d86fe664da12a21711f79f4401e9235557819bc5d4ef52d24f8455b8b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:1.31` - linux; amd64

```console
$ docker pull mediawiki@sha256:7a285ff0cb3d9a847790c653dfae7a2261d474a490c2c3bbde421c8c3dac6302
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251838718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db4ad228621f89c7f104fcb980cf662e52e302f8bde9fc52ee9231c9858d0263`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 22:06:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 22:06:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 22:06:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 22:10:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:56 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 22:10:56 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 22:10:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 22:10:57 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 22:10:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:57 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 22:10:57 GMT
EXPOSE 80
# Sat, 28 Dec 2019 22:10:58 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 11:00:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:58 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 11:01:59 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 11:02:00 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 11:02:07 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616effb632b1d9a229db46a4895f96ef822ed289120d5820f528d4e6d0196b04`  
		Last Modified: Sat, 28 Dec 2019 22:57:09 GMT  
		Size: 12.6 MB (12647459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20683410f309796015435a6c488b34d56f15a42751e53182ff36f9589a697aec`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39e604a3ca40968baa97b55862347eba6db9604fb7009f3b140a5b8a63a48f7`  
		Last Modified: Sat, 28 Dec 2019 22:57:11 GMT  
		Size: 13.8 MB (13840313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc05a4fae7428f9a56c576785244bc2c23c2cd11adec6c8d2a3e4446982b166`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e1a9337fe9acff76d7b3f49a9a55510ef7fa6af7ffa212294bf246d536d62`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1dfa87b2cec32d510224acaaa0ed06f71454e729937f1fb8c17d220fc5476`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b1c9144c1bfcaa8ce4f98f8f98a494041cce5252a5fb21132bb08f4a558e93`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb7894808376d3aa265e25e2dd498af7ded4951ad942b6579cb032969a17010`  
		Last Modified: Sun, 29 Dec 2019 11:02:49 GMT  
		Size: 64.4 MB (64382372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10650c299fdf015820f54960323b5705dce3208624414e83e10dda51b30d2b1d`  
		Last Modified: Sun, 29 Dec 2019 11:02:36 GMT  
		Size: 2.8 MB (2785348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a64e01650d7f7a990f91940bbfd797f1541260aff0abef13e3be9fe44aea78`  
		Last Modified: Sun, 29 Dec 2019 11:02:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa9e447661c47b37ea813400d2e10760cfcead04dc663add54ab05a39062be4`  
		Last Modified: Sun, 29 Dec 2019 11:02:54 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630b2092e36ecf8f916fb0f1c29cb172d732cdabd1586f9f7f9acfe560742b1`  
		Last Modified: Sun, 29 Dec 2019 11:03:03 GMT  
		Size: 35.8 MB (35757718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:ef0bf6ae642cc2cba899051e324e6e51676eea40090ec0b3f8c8f6565aeb9304
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226409915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f411c12b250e4e3b6702aee343d48d59a7f6e47b6737edc97b8bd31d5cbd0f64`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:45:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Jan 2020 21:28:17 GMT
ENV PHP_VERSION=7.2.27
# Thu, 23 Jan 2020 21:28:18 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 21:28:19 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Thu, 23 Jan 2020 21:28:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 21:28:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 21:31:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 21:31:59 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 21:31:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 21:32:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 21:32:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:32:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 21:32:02 GMT
EXPOSE 80
# Thu, 23 Jan 2020 21:32:03 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:56:50 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:58:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:59:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:59:31 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:59:31 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 24 Jan 2020 00:59:32 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 24 Jan 2020 00:59:32 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Fri, 24 Jan 2020 00:59:33 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Fri, 24 Jan 2020 00:59:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2617be9432165f4ff50def4500ca5fcf541952391f0a5d4df67701bc394d2`  
		Last Modified: Thu, 23 Jan 2020 22:08:58 GMT  
		Size: 12.6 MB (12643254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8551c3f5356bf3cfa0a66e3855a0efe8066fe7e70afa47dff31910b97c986848`  
		Last Modified: Thu, 23 Jan 2020 22:08:46 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e729b7434145feec1c3d5e04f80e1c1e86d9e3e52bf329654c9e522b77de3e3b`  
		Last Modified: Thu, 23 Jan 2020 22:08:55 GMT  
		Size: 12.9 MB (12916666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b334636761919b50da4d1829bfaa0354494d1b74a4685041f786014c80cbf5`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3b4973e24f949da38cb81cd021c43453b3836f4745a762576934f89f0eedf4`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b9ab9698f568ba92711f2374a519a4b890fd3eada0b0094b4d69ab1e53891`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b083b324bc21fe14166b4df6df5698a848059740fab4c17079e43447727cc`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88798ca1063ce18ba0743649b0557aa3680d5d097f1ae254b83e3eafafc3c35`  
		Last Modified: Fri, 24 Jan 2020 01:01:57 GMT  
		Size: 60.7 MB (60727513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc48db92f8f0104e85ad6ea21e7710bd9a7011e5a6d84d7a1aee9190902329c`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 2.7 MB (2704392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fe0e9e4680176545f247126ad0874b5caa1fb9598ac33d4f5a19b6d236baf4`  
		Last Modified: Fri, 24 Jan 2020 01:02:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a5fd1a384f029c77fc234ced03fc82fe78dfae93c51a90cfa2ea26e1b3d362`  
		Last Modified: Fri, 24 Jan 2020 01:02:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eef34bca5469eb41f587ac2208ac25134c6030dbe0ece02ecb20f66967db849`  
		Last Modified: Fri, 24 Jan 2020 01:02:52 GMT  
		Size: 35.8 MB (35758727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:902cdc9160421f7b67b42c5be34c59301ae0b40bac222f4a7036eb227b0c592f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.9 MB (219940488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cdf48b416a0015037cfeb85136efa5366b8820d4c57c4124ebec232ebe2c3a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:39:38 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 16:39:39 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 16:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:39:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:42:54 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:59 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:43:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:43:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:43:06 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:43:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:43:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:43:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:43:12 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:09:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:11:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:12:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:12:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:12:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 05:12:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 05:12:13 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 05:12:14 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 05:12:31 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3334f18cf3c9b09c2bb03110d24b806ceed4445b5da5e355e03e723c2b1614`  
		Last Modified: Sat, 28 Dec 2019 17:15:13 GMT  
		Size: 12.6 MB (12645461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eae1e83fddba25d3172b588bce688c3a310608a4bfe25de808e0eb566a04ebf`  
		Last Modified: Sat, 28 Dec 2019 17:15:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fbe17d996b2504cdc42ee40f7d649eca4aaa5be19429a4e539b3329ceb2148`  
		Last Modified: Sat, 28 Dec 2019 17:15:17 GMT  
		Size: 12.2 MB (12186080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2220d9961faeb5bedaefe8a20906c5f3c4539d6f03db8fb786855229732a4c`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc727f308c74cad30c947c8f15188cd2421c2acc731fe9c241b40c6feb1d00`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b81aa860ae65f310e7d52b99ebbd6e7444918b85929de2baa85b188c3863bdb`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128b3062692808ff44cfdd5411ee2739d2edda2e2dcd26883380e709464a2c4d`  
		Last Modified: Sat, 28 Dec 2019 17:15:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0deac41ba566db06f7dc310d07c83a525c13c2e98ea39414561b700d4ce4a66`  
		Last Modified: Sun, 29 Dec 2019 05:13:44 GMT  
		Size: 57.0 MB (57012633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8b99ec8846b071347e924fa2af35fa376c29870cb54fbd15d2a78ca96dd5df`  
		Last Modified: Sun, 29 Dec 2019 05:13:27 GMT  
		Size: 2.6 MB (2649286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c685626d5598b1e85347ad70b3993ba7cacb66f55f75a24ece771374630566`  
		Last Modified: Sun, 29 Dec 2019 05:13:56 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c353924db4c4df5a6902974ed493d1fbc76a399e2136bae23e262b83d17288a`  
		Last Modified: Sun, 29 Dec 2019 05:13:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977796e01e72d35f2a9eb6ca1a2d3ff55cb3908220f961b7ad2e7c94b8f8249a`  
		Last Modified: Sun, 29 Dec 2019 05:14:14 GMT  
		Size: 35.8 MB (35758447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:8c85b7c7625e41de58299cdf2769a58db7dc942f1e73123f4186ab55c7500fca
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241651986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc428c097ace6e52051d6c653b9b13c9722609ca10ff30f732502eebb3f3622`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 15:33:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 15:33:35 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 15:33:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 15:33:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:37:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:13 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:37:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:37:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:37:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:37:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:21 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:37:22 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:37:23 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:23:20 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:26:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:26:09 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:26:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 06:26:17 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 06:26:19 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 06:26:21 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 06:26:38 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef55e879c10bb0bfe58b0e87d612c419ea5bd7503872b20b4f204c4ff29fc529`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 12.6 MB (12646118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f6952b67823bbc1f9d02a4c84126ee319f7453c8b50ba5c15d230f582a24cb`  
		Last Modified: Sat, 28 Dec 2019 16:12:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1409df52b683c197e2f155c5fff7655f3685cba677ed3cd88500b5c50a0b322e`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 13.5 MB (13537744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a0571861c31f3e3e66ef375bed45e5baf9b06264b2c21f16c281c14a6e425a`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5f5ab5fff422d4c5851f79af8e8bcd99629a1d824101f26afe878f49641733`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd643e176f0541609f1cc882c4c2bf40a168ea1a2774bbba5dddea14492e4c14`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266f7b1f11a53b6b15316c0eefecf0d4b8647f2672c42d0b8a7f745bb9939ae3`  
		Last Modified: Sat, 28 Dec 2019 16:12:19 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293f6ae45064ffc9bead71caf085d167b46041ea02c548d0a5051becaf93b138`  
		Last Modified: Sun, 29 Dec 2019 06:27:48 GMT  
		Size: 62.2 MB (62181447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4189a9c54e310f0ed59abeeb288b039c62fbea382ad7b6d2fa91460e2d444d95`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 2.8 MB (2758645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4e636ddcf984e5af604a377da8959f89ef3ebbf5e3f750d2e2720fa3e7fc4d`  
		Last Modified: Sun, 29 Dec 2019 06:27:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3672476e195cbe2f6a8e973fccb19d0ea4613bc6516b73bd2d85c598c659099`  
		Last Modified: Sun, 29 Dec 2019 06:27:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb9b160cbe9a80bf9b013df22a8204bdce4024a6e235bbc549a65b32249516c`  
		Last Modified: Sun, 29 Dec 2019 06:28:15 GMT  
		Size: 35.8 MB (35758354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31` - linux; 386

```console
$ docker pull mediawiki@sha256:6fbf0ace16a8122ea07b7f118f488890f81ffcbbe745196d8bad530354c9f3cf
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.7 MB (259742492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f4ef9d2378f4b8e23256d6601c7abb1673361047d70c77f15ac01be6db2c24`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:36:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 18:36:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:36:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:41:53 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:41:54 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:41:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:41:55 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:41:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:55 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:41:55 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:41:55 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:52:44 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:54:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:55:17 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:55:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 01:55:37 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7cf80bc7d8085b8ce0a31e3a98f5693961c49434a02d4140d3c71a07ca565`  
		Last Modified: Sat, 28 Dec 2019 19:37:07 GMT  
		Size: 12.6 MB (12646713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a2cb9f569f09db2f619aa046f4b6508bf2a6734586800e94606e2cd6d4c56d`  
		Last Modified: Sat, 28 Dec 2019 19:37:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59eac3b46370851360f3dd6921cd777da75f7e064a3f2b86bca60969d4f11e3`  
		Last Modified: Sat, 28 Dec 2019 19:37:11 GMT  
		Size: 14.2 MB (14165526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365a0af4c7ee6ef2bf0e01e4dd3aa80cdf65b41072447cd02e375d3da249dcb`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ffa88e5eec5d45da757fb19b139ff9468309d797987ffc10120d9538947db2`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec1aab950c8691b268d3ee910c230ebe39a8c86cd15872a46d482d9d919987`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8735cfcf9ac1f26b597e58e0dc46c495468cb03cb7bef0c4400da5e8fdbd7cca`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70d0681d2078e2326a14831637f16c3b57fe8f03a55b3f90fc6fb689aba645`  
		Last Modified: Sun, 29 Dec 2019 01:57:23 GMT  
		Size: 66.3 MB (66332499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a47642cce4d2c51efea83292928b49c8938d7cfcc64b60d49387d9e5fa0466`  
		Last Modified: Sun, 29 Dec 2019 01:56:48 GMT  
		Size: 2.8 MB (2775897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8aea51ae0228a216cb72d951e5c80aaa98a02d29c5d2217f7bdcaa95b1bbf65`  
		Last Modified: Sun, 29 Dec 2019 01:57:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59100766a49da5cc2fae5f62cdc492305df96a29f1b4fc106424ceb4aa643c17`  
		Last Modified: Sun, 29 Dec 2019 01:57:30 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3182a6bb97203a909bd4acfd36db720708ca6dd5392407da551710e4b2faf874`  
		Last Modified: Sun, 29 Dec 2019 01:57:50 GMT  
		Size: 35.8 MB (35757566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:aa640970accbfb523f7db66d932a3b49a49b59dd5736a3c37bd75778990e1a98
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.9 MB (269939370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a94f92cfe74abdaeaef6b273e3ea467fefaf086f07e2af64297280d00380ad`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 19:27:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 19:27:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 19:27:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 19:27:39 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 19:28:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 19:28:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 19:33:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:08 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 19:33:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 19:33:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 19:33:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 19:33:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:25 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 19:33:28 GMT
EXPOSE 80
# Sat, 28 Dec 2019 19:33:32 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:49:09 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:50:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:51:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:51:33 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:51:36 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 04:51:39 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 04:51:41 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 04:51:45 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 04:52:05 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed447e92ed09c9a464d9a1193550b84f1554bb96dd375ae2518965c4acc5e7`  
		Last Modified: Sat, 28 Dec 2019 20:19:48 GMT  
		Size: 12.6 MB (12647171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98bdd73f274ddf4d613631b79831e24954ed7bdcbc3001a970ab2673c90191`  
		Last Modified: Sat, 28 Dec 2019 20:19:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dea2440f3d8645d587221a106bb249affd61425e76cc2ddd5dde65e8557233`  
		Last Modified: Sat, 28 Dec 2019 20:19:49 GMT  
		Size: 14.9 MB (14882224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649bcaf54170c4cd63a99ed326d39a923216563f4f0721325378a7cdf34ce226`  
		Last Modified: Sat, 28 Dec 2019 20:19:43 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aef28adb9261ac35a69849d5571500918f8982cb367407b2fd2809608c0e6b5`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ad091ce1cb239b0012874b210006f7c03b53cdffa8ccb08111b869af2038fb`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d3bfe1ba07823cbf208809c693031e47cadbbc426392afd2b144b82a46b89`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7c4357ace9f66702187924dddaff72c659358a6ca5bbebcfbd28172af34a6`  
		Last Modified: Sun, 29 Dec 2019 04:53:26 GMT  
		Size: 71.2 MB (71194229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d489ec07beb31e3bc26690c954bc8d3947b0d7e100e4330fd1f3df46063eada2`  
		Last Modified: Sun, 29 Dec 2019 04:53:09 GMT  
		Size: 2.9 MB (2863120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1d639a84d6660d51844ed94e20719d38a828e7541d14a2b734d751cf4dc867`  
		Last Modified: Sun, 29 Dec 2019 04:53:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f88e7849100e1cac1ac29e8cfd1c50a0f59f93ecba9a3a503cbc8acaeca03`  
		Last Modified: Sun, 29 Dec 2019 04:53:42 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8da8586fd0df698a9020506552f9e12c7e7f66dc625bfaa25294a99a24d1b77`  
		Last Modified: Sun, 29 Dec 2019 04:53:52 GMT  
		Size: 35.8 MB (35758158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:1.31.6`

```console
$ docker pull mediawiki@sha256:278a7d86fe664da12a21711f79f4401e9235557819bc5d4ef52d24f8455b8b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:1.31.6` - linux; amd64

```console
$ docker pull mediawiki@sha256:7a285ff0cb3d9a847790c653dfae7a2261d474a490c2c3bbde421c8c3dac6302
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251838718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db4ad228621f89c7f104fcb980cf662e52e302f8bde9fc52ee9231c9858d0263`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 22:06:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 22:06:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 22:06:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 22:10:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:56 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 22:10:56 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 22:10:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 22:10:57 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 22:10:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:57 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 22:10:57 GMT
EXPOSE 80
# Sat, 28 Dec 2019 22:10:58 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 11:00:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:58 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 11:01:59 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 11:02:00 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 11:02:07 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616effb632b1d9a229db46a4895f96ef822ed289120d5820f528d4e6d0196b04`  
		Last Modified: Sat, 28 Dec 2019 22:57:09 GMT  
		Size: 12.6 MB (12647459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20683410f309796015435a6c488b34d56f15a42751e53182ff36f9589a697aec`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39e604a3ca40968baa97b55862347eba6db9604fb7009f3b140a5b8a63a48f7`  
		Last Modified: Sat, 28 Dec 2019 22:57:11 GMT  
		Size: 13.8 MB (13840313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc05a4fae7428f9a56c576785244bc2c23c2cd11adec6c8d2a3e4446982b166`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e1a9337fe9acff76d7b3f49a9a55510ef7fa6af7ffa212294bf246d536d62`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1dfa87b2cec32d510224acaaa0ed06f71454e729937f1fb8c17d220fc5476`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b1c9144c1bfcaa8ce4f98f8f98a494041cce5252a5fb21132bb08f4a558e93`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb7894808376d3aa265e25e2dd498af7ded4951ad942b6579cb032969a17010`  
		Last Modified: Sun, 29 Dec 2019 11:02:49 GMT  
		Size: 64.4 MB (64382372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10650c299fdf015820f54960323b5705dce3208624414e83e10dda51b30d2b1d`  
		Last Modified: Sun, 29 Dec 2019 11:02:36 GMT  
		Size: 2.8 MB (2785348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a64e01650d7f7a990f91940bbfd797f1541260aff0abef13e3be9fe44aea78`  
		Last Modified: Sun, 29 Dec 2019 11:02:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa9e447661c47b37ea813400d2e10760cfcead04dc663add54ab05a39062be4`  
		Last Modified: Sun, 29 Dec 2019 11:02:54 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630b2092e36ecf8f916fb0f1c29cb172d732cdabd1586f9f7f9acfe560742b1`  
		Last Modified: Sun, 29 Dec 2019 11:03:03 GMT  
		Size: 35.8 MB (35757718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31.6` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:ef0bf6ae642cc2cba899051e324e6e51676eea40090ec0b3f8c8f6565aeb9304
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226409915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f411c12b250e4e3b6702aee343d48d59a7f6e47b6737edc97b8bd31d5cbd0f64`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:45:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Jan 2020 21:28:17 GMT
ENV PHP_VERSION=7.2.27
# Thu, 23 Jan 2020 21:28:18 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 21:28:19 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Thu, 23 Jan 2020 21:28:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 21:28:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 21:31:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 21:31:59 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 21:31:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 21:32:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 21:32:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:32:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 21:32:02 GMT
EXPOSE 80
# Thu, 23 Jan 2020 21:32:03 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:56:50 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:58:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:59:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:59:31 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:59:31 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 24 Jan 2020 00:59:32 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 24 Jan 2020 00:59:32 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Fri, 24 Jan 2020 00:59:33 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Fri, 24 Jan 2020 00:59:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2617be9432165f4ff50def4500ca5fcf541952391f0a5d4df67701bc394d2`  
		Last Modified: Thu, 23 Jan 2020 22:08:58 GMT  
		Size: 12.6 MB (12643254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8551c3f5356bf3cfa0a66e3855a0efe8066fe7e70afa47dff31910b97c986848`  
		Last Modified: Thu, 23 Jan 2020 22:08:46 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e729b7434145feec1c3d5e04f80e1c1e86d9e3e52bf329654c9e522b77de3e3b`  
		Last Modified: Thu, 23 Jan 2020 22:08:55 GMT  
		Size: 12.9 MB (12916666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b334636761919b50da4d1829bfaa0354494d1b74a4685041f786014c80cbf5`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3b4973e24f949da38cb81cd021c43453b3836f4745a762576934f89f0eedf4`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b9ab9698f568ba92711f2374a519a4b890fd3eada0b0094b4d69ab1e53891`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b083b324bc21fe14166b4df6df5698a848059740fab4c17079e43447727cc`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88798ca1063ce18ba0743649b0557aa3680d5d097f1ae254b83e3eafafc3c35`  
		Last Modified: Fri, 24 Jan 2020 01:01:57 GMT  
		Size: 60.7 MB (60727513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc48db92f8f0104e85ad6ea21e7710bd9a7011e5a6d84d7a1aee9190902329c`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 2.7 MB (2704392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fe0e9e4680176545f247126ad0874b5caa1fb9598ac33d4f5a19b6d236baf4`  
		Last Modified: Fri, 24 Jan 2020 01:02:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a5fd1a384f029c77fc234ced03fc82fe78dfae93c51a90cfa2ea26e1b3d362`  
		Last Modified: Fri, 24 Jan 2020 01:02:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eef34bca5469eb41f587ac2208ac25134c6030dbe0ece02ecb20f66967db849`  
		Last Modified: Fri, 24 Jan 2020 01:02:52 GMT  
		Size: 35.8 MB (35758727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31.6` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:902cdc9160421f7b67b42c5be34c59301ae0b40bac222f4a7036eb227b0c592f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.9 MB (219940488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cdf48b416a0015037cfeb85136efa5366b8820d4c57c4124ebec232ebe2c3a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:39:38 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 16:39:39 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 16:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:39:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:42:54 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:59 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:43:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:43:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:43:06 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:43:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:43:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:43:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:43:12 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:09:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:11:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:12:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:12:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:12:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 05:12:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 05:12:13 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 05:12:14 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 05:12:31 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3334f18cf3c9b09c2bb03110d24b806ceed4445b5da5e355e03e723c2b1614`  
		Last Modified: Sat, 28 Dec 2019 17:15:13 GMT  
		Size: 12.6 MB (12645461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eae1e83fddba25d3172b588bce688c3a310608a4bfe25de808e0eb566a04ebf`  
		Last Modified: Sat, 28 Dec 2019 17:15:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fbe17d996b2504cdc42ee40f7d649eca4aaa5be19429a4e539b3329ceb2148`  
		Last Modified: Sat, 28 Dec 2019 17:15:17 GMT  
		Size: 12.2 MB (12186080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2220d9961faeb5bedaefe8a20906c5f3c4539d6f03db8fb786855229732a4c`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc727f308c74cad30c947c8f15188cd2421c2acc731fe9c241b40c6feb1d00`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b81aa860ae65f310e7d52b99ebbd6e7444918b85929de2baa85b188c3863bdb`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128b3062692808ff44cfdd5411ee2739d2edda2e2dcd26883380e709464a2c4d`  
		Last Modified: Sat, 28 Dec 2019 17:15:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0deac41ba566db06f7dc310d07c83a525c13c2e98ea39414561b700d4ce4a66`  
		Last Modified: Sun, 29 Dec 2019 05:13:44 GMT  
		Size: 57.0 MB (57012633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8b99ec8846b071347e924fa2af35fa376c29870cb54fbd15d2a78ca96dd5df`  
		Last Modified: Sun, 29 Dec 2019 05:13:27 GMT  
		Size: 2.6 MB (2649286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c685626d5598b1e85347ad70b3993ba7cacb66f55f75a24ece771374630566`  
		Last Modified: Sun, 29 Dec 2019 05:13:56 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c353924db4c4df5a6902974ed493d1fbc76a399e2136bae23e262b83d17288a`  
		Last Modified: Sun, 29 Dec 2019 05:13:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977796e01e72d35f2a9eb6ca1a2d3ff55cb3908220f961b7ad2e7c94b8f8249a`  
		Last Modified: Sun, 29 Dec 2019 05:14:14 GMT  
		Size: 35.8 MB (35758447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31.6` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:8c85b7c7625e41de58299cdf2769a58db7dc942f1e73123f4186ab55c7500fca
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241651986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc428c097ace6e52051d6c653b9b13c9722609ca10ff30f732502eebb3f3622`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 15:33:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 15:33:35 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 15:33:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 15:33:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:37:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:13 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:37:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:37:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:37:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:37:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:21 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:37:22 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:37:23 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:23:20 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:26:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:26:09 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:26:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 06:26:17 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 06:26:19 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 06:26:21 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 06:26:38 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef55e879c10bb0bfe58b0e87d612c419ea5bd7503872b20b4f204c4ff29fc529`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 12.6 MB (12646118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f6952b67823bbc1f9d02a4c84126ee319f7453c8b50ba5c15d230f582a24cb`  
		Last Modified: Sat, 28 Dec 2019 16:12:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1409df52b683c197e2f155c5fff7655f3685cba677ed3cd88500b5c50a0b322e`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 13.5 MB (13537744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a0571861c31f3e3e66ef375bed45e5baf9b06264b2c21f16c281c14a6e425a`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5f5ab5fff422d4c5851f79af8e8bcd99629a1d824101f26afe878f49641733`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd643e176f0541609f1cc882c4c2bf40a168ea1a2774bbba5dddea14492e4c14`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266f7b1f11a53b6b15316c0eefecf0d4b8647f2672c42d0b8a7f745bb9939ae3`  
		Last Modified: Sat, 28 Dec 2019 16:12:19 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293f6ae45064ffc9bead71caf085d167b46041ea02c548d0a5051becaf93b138`  
		Last Modified: Sun, 29 Dec 2019 06:27:48 GMT  
		Size: 62.2 MB (62181447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4189a9c54e310f0ed59abeeb288b039c62fbea382ad7b6d2fa91460e2d444d95`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 2.8 MB (2758645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4e636ddcf984e5af604a377da8959f89ef3ebbf5e3f750d2e2720fa3e7fc4d`  
		Last Modified: Sun, 29 Dec 2019 06:27:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3672476e195cbe2f6a8e973fccb19d0ea4613bc6516b73bd2d85c598c659099`  
		Last Modified: Sun, 29 Dec 2019 06:27:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb9b160cbe9a80bf9b013df22a8204bdce4024a6e235bbc549a65b32249516c`  
		Last Modified: Sun, 29 Dec 2019 06:28:15 GMT  
		Size: 35.8 MB (35758354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31.6` - linux; 386

```console
$ docker pull mediawiki@sha256:6fbf0ace16a8122ea07b7f118f488890f81ffcbbe745196d8bad530354c9f3cf
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.7 MB (259742492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f4ef9d2378f4b8e23256d6601c7abb1673361047d70c77f15ac01be6db2c24`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:36:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 18:36:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:36:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:41:53 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:41:54 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:41:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:41:55 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:41:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:55 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:41:55 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:41:55 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:52:44 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:54:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:55:17 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:55:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 01:55:37 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7cf80bc7d8085b8ce0a31e3a98f5693961c49434a02d4140d3c71a07ca565`  
		Last Modified: Sat, 28 Dec 2019 19:37:07 GMT  
		Size: 12.6 MB (12646713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a2cb9f569f09db2f619aa046f4b6508bf2a6734586800e94606e2cd6d4c56d`  
		Last Modified: Sat, 28 Dec 2019 19:37:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59eac3b46370851360f3dd6921cd777da75f7e064a3f2b86bca60969d4f11e3`  
		Last Modified: Sat, 28 Dec 2019 19:37:11 GMT  
		Size: 14.2 MB (14165526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365a0af4c7ee6ef2bf0e01e4dd3aa80cdf65b41072447cd02e375d3da249dcb`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ffa88e5eec5d45da757fb19b139ff9468309d797987ffc10120d9538947db2`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec1aab950c8691b268d3ee910c230ebe39a8c86cd15872a46d482d9d919987`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8735cfcf9ac1f26b597e58e0dc46c495468cb03cb7bef0c4400da5e8fdbd7cca`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70d0681d2078e2326a14831637f16c3b57fe8f03a55b3f90fc6fb689aba645`  
		Last Modified: Sun, 29 Dec 2019 01:57:23 GMT  
		Size: 66.3 MB (66332499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a47642cce4d2c51efea83292928b49c8938d7cfcc64b60d49387d9e5fa0466`  
		Last Modified: Sun, 29 Dec 2019 01:56:48 GMT  
		Size: 2.8 MB (2775897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8aea51ae0228a216cb72d951e5c80aaa98a02d29c5d2217f7bdcaa95b1bbf65`  
		Last Modified: Sun, 29 Dec 2019 01:57:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59100766a49da5cc2fae5f62cdc492305df96a29f1b4fc106424ceb4aa643c17`  
		Last Modified: Sun, 29 Dec 2019 01:57:30 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3182a6bb97203a909bd4acfd36db720708ca6dd5392407da551710e4b2faf874`  
		Last Modified: Sun, 29 Dec 2019 01:57:50 GMT  
		Size: 35.8 MB (35757566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31.6` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:aa640970accbfb523f7db66d932a3b49a49b59dd5736a3c37bd75778990e1a98
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.9 MB (269939370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a94f92cfe74abdaeaef6b273e3ea467fefaf086f07e2af64297280d00380ad`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 19:27:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 19:27:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 19:27:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 19:27:39 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 19:28:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 19:28:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 19:33:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:08 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 19:33:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 19:33:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 19:33:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 19:33:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:25 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 19:33:28 GMT
EXPOSE 80
# Sat, 28 Dec 2019 19:33:32 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:49:09 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:50:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:51:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:51:33 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:51:36 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 04:51:39 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 04:51:41 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 04:51:45 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 04:52:05 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed447e92ed09c9a464d9a1193550b84f1554bb96dd375ae2518965c4acc5e7`  
		Last Modified: Sat, 28 Dec 2019 20:19:48 GMT  
		Size: 12.6 MB (12647171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98bdd73f274ddf4d613631b79831e24954ed7bdcbc3001a970ab2673c90191`  
		Last Modified: Sat, 28 Dec 2019 20:19:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dea2440f3d8645d587221a106bb249affd61425e76cc2ddd5dde65e8557233`  
		Last Modified: Sat, 28 Dec 2019 20:19:49 GMT  
		Size: 14.9 MB (14882224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649bcaf54170c4cd63a99ed326d39a923216563f4f0721325378a7cdf34ce226`  
		Last Modified: Sat, 28 Dec 2019 20:19:43 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aef28adb9261ac35a69849d5571500918f8982cb367407b2fd2809608c0e6b5`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ad091ce1cb239b0012874b210006f7c03b53cdffa8ccb08111b869af2038fb`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d3bfe1ba07823cbf208809c693031e47cadbbc426392afd2b144b82a46b89`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7c4357ace9f66702187924dddaff72c659358a6ca5bbebcfbd28172af34a6`  
		Last Modified: Sun, 29 Dec 2019 04:53:26 GMT  
		Size: 71.2 MB (71194229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d489ec07beb31e3bc26690c954bc8d3947b0d7e100e4330fd1f3df46063eada2`  
		Last Modified: Sun, 29 Dec 2019 04:53:09 GMT  
		Size: 2.9 MB (2863120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1d639a84d6660d51844ed94e20719d38a828e7541d14a2b734d751cf4dc867`  
		Last Modified: Sun, 29 Dec 2019 04:53:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f88e7849100e1cac1ac29e8cfd1c50a0f59f93ecba9a3a503cbc8acaeca03`  
		Last Modified: Sun, 29 Dec 2019 04:53:42 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8da8586fd0df698a9020506552f9e12c7e7f66dc625bfaa25294a99a24d1b77`  
		Last Modified: Sun, 29 Dec 2019 04:53:52 GMT  
		Size: 35.8 MB (35758158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:1.33`

```console
$ docker pull mediawiki@sha256:9b946c708b7cfc499c83f06eb8b36eecdc3ecc6e76235417d6cdce18e9cd4e5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:1.33` - linux; amd64

```console
$ docker pull mediawiki@sha256:359fa8b601cbab9afc052a3d172fdf9729e82ea83dc805522c40a8de4cc60552
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254485539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af8f16c5019a4cd2e3365c6b95efab1a7af3b715c3f62805aff87afae26499d4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 22:06:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 22:06:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 22:06:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 22:10:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:56 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 22:10:56 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 22:10:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 22:10:57 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 22:10:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:57 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 22:10:57 GMT
EXPOSE 80
# Sat, 28 Dec 2019 22:10:58 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 11:00:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:38 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 11:01:39 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 11:01:40 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 11:01:48 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616effb632b1d9a229db46a4895f96ef822ed289120d5820f528d4e6d0196b04`  
		Last Modified: Sat, 28 Dec 2019 22:57:09 GMT  
		Size: 12.6 MB (12647459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20683410f309796015435a6c488b34d56f15a42751e53182ff36f9589a697aec`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39e604a3ca40968baa97b55862347eba6db9604fb7009f3b140a5b8a63a48f7`  
		Last Modified: Sat, 28 Dec 2019 22:57:11 GMT  
		Size: 13.8 MB (13840313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc05a4fae7428f9a56c576785244bc2c23c2cd11adec6c8d2a3e4446982b166`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e1a9337fe9acff76d7b3f49a9a55510ef7fa6af7ffa212294bf246d536d62`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1dfa87b2cec32d510224acaaa0ed06f71454e729937f1fb8c17d220fc5476`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b1c9144c1bfcaa8ce4f98f8f98a494041cce5252a5fb21132bb08f4a558e93`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb7894808376d3aa265e25e2dd498af7ded4951ad942b6579cb032969a17010`  
		Last Modified: Sun, 29 Dec 2019 11:02:49 GMT  
		Size: 64.4 MB (64382372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10650c299fdf015820f54960323b5705dce3208624414e83e10dda51b30d2b1d`  
		Last Modified: Sun, 29 Dec 2019 11:02:36 GMT  
		Size: 2.8 MB (2785348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1f8f053ad728d5a3674d533f9858336736035c682b1476a00d7a62e35d5f6b`  
		Last Modified: Sun, 29 Dec 2019 11:02:35 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c81fb66e89a2da8a55d652fb13c1b3b54d11beacc5777d5842e948aae0da212`  
		Last Modified: Sun, 29 Dec 2019 11:02:35 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280d802648d655bef8649725137c4f2feaa1c387d210ed7de2fdd91e4f07f1ae`  
		Last Modified: Sun, 29 Dec 2019 11:02:35 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e16fd8e49e1c7ebad393b0d86f6cc2dbc09d0e115e46ca5c4ba98d826125b`  
		Last Modified: Sun, 29 Dec 2019 11:02:47 GMT  
		Size: 38.4 MB (38403961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:b9f3641156d3468cf34ac5a25d90eeef966bba06dc7506b715466d8606ebd32f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229056039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0129845204b9a068d23aa5ec3b344ba77093bdfd5a78ccadffaeeb3696130f2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:45:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Jan 2020 21:28:17 GMT
ENV PHP_VERSION=7.2.27
# Thu, 23 Jan 2020 21:28:18 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 21:28:19 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Thu, 23 Jan 2020 21:28:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 21:28:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 21:31:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 21:31:59 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 21:31:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 21:32:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 21:32:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:32:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 21:32:02 GMT
EXPOSE 80
# Thu, 23 Jan 2020 21:32:03 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:56:50 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:58:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:58:55 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 00:58:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:58:58 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:58:59 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 24 Jan 2020 00:58:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 24 Jan 2020 00:59:00 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Fri, 24 Jan 2020 00:59:00 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Fri, 24 Jan 2020 00:59:18 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2617be9432165f4ff50def4500ca5fcf541952391f0a5d4df67701bc394d2`  
		Last Modified: Thu, 23 Jan 2020 22:08:58 GMT  
		Size: 12.6 MB (12643254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8551c3f5356bf3cfa0a66e3855a0efe8066fe7e70afa47dff31910b97c986848`  
		Last Modified: Thu, 23 Jan 2020 22:08:46 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e729b7434145feec1c3d5e04f80e1c1e86d9e3e52bf329654c9e522b77de3e3b`  
		Last Modified: Thu, 23 Jan 2020 22:08:55 GMT  
		Size: 12.9 MB (12916666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b334636761919b50da4d1829bfaa0354494d1b74a4685041f786014c80cbf5`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3b4973e24f949da38cb81cd021c43453b3836f4745a762576934f89f0eedf4`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b9ab9698f568ba92711f2374a519a4b890fd3eada0b0094b4d69ab1e53891`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b083b324bc21fe14166b4df6df5698a848059740fab4c17079e43447727cc`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88798ca1063ce18ba0743649b0557aa3680d5d097f1ae254b83e3eafafc3c35`  
		Last Modified: Fri, 24 Jan 2020 01:01:57 GMT  
		Size: 60.7 MB (60727513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc48db92f8f0104e85ad6ea21e7710bd9a7011e5a6d84d7a1aee9190902329c`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 2.7 MB (2704392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1530367864dd497a5a8d1c2ddfc9a2619fcbd68613440fca5d360a4072002a`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4994b55ac4ae7d781c41887b7d2fde42a3f5db31099437695557d18738778269`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a99c54f8644a844a3d269e5af8e3f3646bef4c1ab3394ba007c3e000605b801`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b6f6b9e1358d41cba72f67e16f5b9415ec954f1acdc2f7636f2c2b93208e66`  
		Last Modified: Fri, 24 Jan 2020 01:01:44 GMT  
		Size: 38.4 MB (38404270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:5aa506775a4c82a6648de1da7c0ff77fc0b4b121018c22811ed55db57d335482
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222586741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8feab2dad602b08a9f2979979d72382a5abcdc7a1e0877b44f1b3aa2fda7eb0c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:39:38 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 16:39:39 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 16:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:39:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:42:54 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:59 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:43:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:43:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:43:06 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:43:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:43:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:43:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:43:12 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:09:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:11:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:11:21 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 05:11:24 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:11:27 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:11:27 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 05:11:28 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 05:11:29 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 05:11:30 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 05:11:54 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3334f18cf3c9b09c2bb03110d24b806ceed4445b5da5e355e03e723c2b1614`  
		Last Modified: Sat, 28 Dec 2019 17:15:13 GMT  
		Size: 12.6 MB (12645461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eae1e83fddba25d3172b588bce688c3a310608a4bfe25de808e0eb566a04ebf`  
		Last Modified: Sat, 28 Dec 2019 17:15:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fbe17d996b2504cdc42ee40f7d649eca4aaa5be19429a4e539b3329ceb2148`  
		Last Modified: Sat, 28 Dec 2019 17:15:17 GMT  
		Size: 12.2 MB (12186080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2220d9961faeb5bedaefe8a20906c5f3c4539d6f03db8fb786855229732a4c`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc727f308c74cad30c947c8f15188cd2421c2acc731fe9c241b40c6feb1d00`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b81aa860ae65f310e7d52b99ebbd6e7444918b85929de2baa85b188c3863bdb`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128b3062692808ff44cfdd5411ee2739d2edda2e2dcd26883380e709464a2c4d`  
		Last Modified: Sat, 28 Dec 2019 17:15:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0deac41ba566db06f7dc310d07c83a525c13c2e98ea39414561b700d4ce4a66`  
		Last Modified: Sun, 29 Dec 2019 05:13:44 GMT  
		Size: 57.0 MB (57012633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8b99ec8846b071347e924fa2af35fa376c29870cb54fbd15d2a78ca96dd5df`  
		Last Modified: Sun, 29 Dec 2019 05:13:27 GMT  
		Size: 2.6 MB (2649286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e60ec632bf71f86563144cf4e35fc8c513c33c852cb9e765ffc2875df6cf75`  
		Last Modified: Sun, 29 Dec 2019 05:13:26 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0249bc474c5b8c2d6456c07afcbe23f67ecf3f7895e619e454e14950026623a3`  
		Last Modified: Sun, 29 Dec 2019 05:13:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34394ad2ae2eb0f7e2b44365a3da6453e7f56f54edfa10bd16c29ce78de8fd4`  
		Last Modified: Sun, 29 Dec 2019 05:13:26 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff479b89d9f4d4d29d66bbd143f96e9932f6e46ad85cfa4c209a3976fb481ebc`  
		Last Modified: Sun, 29 Dec 2019 05:13:46 GMT  
		Size: 38.4 MB (38404118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:e59c6d09ef010365ddbd5490c515fcf67e67934b670e687c62f9cca9cfc56fbc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244298301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e38b5d01f808594bc7aeacdcb08eb4a35e5ec186170a68a354fb6896a84744d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 15:33:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 15:33:35 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 15:33:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 15:33:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:37:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:13 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:37:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:37:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:37:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:37:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:21 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:37:22 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:37:23 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:23:20 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:25:05 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 06:25:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:25:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:25:11 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 06:25:12 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 06:25:13 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 06:25:14 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 06:25:32 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef55e879c10bb0bfe58b0e87d612c419ea5bd7503872b20b4f204c4ff29fc529`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 12.6 MB (12646118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f6952b67823bbc1f9d02a4c84126ee319f7453c8b50ba5c15d230f582a24cb`  
		Last Modified: Sat, 28 Dec 2019 16:12:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1409df52b683c197e2f155c5fff7655f3685cba677ed3cd88500b5c50a0b322e`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 13.5 MB (13537744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a0571861c31f3e3e66ef375bed45e5baf9b06264b2c21f16c281c14a6e425a`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5f5ab5fff422d4c5851f79af8e8bcd99629a1d824101f26afe878f49641733`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd643e176f0541609f1cc882c4c2bf40a168ea1a2774bbba5dddea14492e4c14`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266f7b1f11a53b6b15316c0eefecf0d4b8647f2672c42d0b8a7f745bb9939ae3`  
		Last Modified: Sat, 28 Dec 2019 16:12:19 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293f6ae45064ffc9bead71caf085d167b46041ea02c548d0a5051becaf93b138`  
		Last Modified: Sun, 29 Dec 2019 06:27:48 GMT  
		Size: 62.2 MB (62181447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4189a9c54e310f0ed59abeeb288b039c62fbea382ad7b6d2fa91460e2d444d95`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 2.8 MB (2758645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3505bbad6e024712a3e32a22eae39e7270a0b97234e28ff9a5b0d460eab6c7ea`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d709b64262da7fb53be566d00c67b818fa62979cb819bc33a488482e4c45`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83262d9002968ac1df9efc63e137fec1a20648d0226372b894bf3dd7cf677ce7`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d448e490744eb93dfc7686d0e48e79bfd88b23f1d6a71fbfdfda20b2d23f237`  
		Last Modified: Sun, 29 Dec 2019 06:27:48 GMT  
		Size: 38.4 MB (38404077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33` - linux; 386

```console
$ docker pull mediawiki@sha256:744ce0f47bf1ea291f021f8c301b3e4356242963fb5e12dde1af01de09ef5d3c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262389336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6da020e16b26371a7ebccfb387cad0361dc6f827c27a8a2883691ec4440d066`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:36:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 18:36:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:36:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:41:53 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:41:54 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:41:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:41:55 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:41:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:55 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:41:55 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:41:55 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:52:44 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:54:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:54:48 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 01:54:49 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:54:50 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:54:50 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 01:54:51 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 01:54:51 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 01:54:51 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 01:55:09 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7cf80bc7d8085b8ce0a31e3a98f5693961c49434a02d4140d3c71a07ca565`  
		Last Modified: Sat, 28 Dec 2019 19:37:07 GMT  
		Size: 12.6 MB (12646713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a2cb9f569f09db2f619aa046f4b6508bf2a6734586800e94606e2cd6d4c56d`  
		Last Modified: Sat, 28 Dec 2019 19:37:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59eac3b46370851360f3dd6921cd777da75f7e064a3f2b86bca60969d4f11e3`  
		Last Modified: Sat, 28 Dec 2019 19:37:11 GMT  
		Size: 14.2 MB (14165526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365a0af4c7ee6ef2bf0e01e4dd3aa80cdf65b41072447cd02e375d3da249dcb`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ffa88e5eec5d45da757fb19b139ff9468309d797987ffc10120d9538947db2`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec1aab950c8691b268d3ee910c230ebe39a8c86cd15872a46d482d9d919987`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8735cfcf9ac1f26b597e58e0dc46c495468cb03cb7bef0c4400da5e8fdbd7cca`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70d0681d2078e2326a14831637f16c3b57fe8f03a55b3f90fc6fb689aba645`  
		Last Modified: Sun, 29 Dec 2019 01:57:23 GMT  
		Size: 66.3 MB (66332499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a47642cce4d2c51efea83292928b49c8938d7cfcc64b60d49387d9e5fa0466`  
		Last Modified: Sun, 29 Dec 2019 01:56:48 GMT  
		Size: 2.8 MB (2775897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424ab26a745ac3ea474c6f774ae98ac511d55c937d311dc3130b691647170065`  
		Last Modified: Sun, 29 Dec 2019 01:56:47 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdc270e7a25645ace70eb291be080460db20a6b91e979a3891aa0b8ebfc4fd8`  
		Last Modified: Sun, 29 Dec 2019 01:56:46 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb590edb4822037944e08e48ecfc21c928abb49b7ac0428ebe5a5efd6d946639`  
		Last Modified: Sun, 29 Dec 2019 01:56:46 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b797c353e22d07dd62f666bbb41f01d3b4008b2d631fabe5b428e818e4b70a`  
		Last Modified: Sun, 29 Dec 2019 01:57:18 GMT  
		Size: 38.4 MB (38403827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:a255a5fd8dbbb5d5c5a2e4779f636f7eb65cdb347fbcac310c9de5843ffe2cf2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272585730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:153f3fb344733f1c2e1d2a8513bfbaf29d328c5c85f441a7b86c1aeb7e19221b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 19:27:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 19:27:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 19:27:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 19:27:39 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 19:28:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 19:28:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 19:33:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:08 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 19:33:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 19:33:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 19:33:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 19:33:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:25 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 19:33:28 GMT
EXPOSE 80
# Sat, 28 Dec 2019 19:33:32 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:49:09 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:50:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:50:39 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 04:50:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:50:48 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:50:49 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 04:50:51 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 04:50:53 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 04:50:54 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 04:51:09 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed447e92ed09c9a464d9a1193550b84f1554bb96dd375ae2518965c4acc5e7`  
		Last Modified: Sat, 28 Dec 2019 20:19:48 GMT  
		Size: 12.6 MB (12647171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98bdd73f274ddf4d613631b79831e24954ed7bdcbc3001a970ab2673c90191`  
		Last Modified: Sat, 28 Dec 2019 20:19:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dea2440f3d8645d587221a106bb249affd61425e76cc2ddd5dde65e8557233`  
		Last Modified: Sat, 28 Dec 2019 20:19:49 GMT  
		Size: 14.9 MB (14882224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649bcaf54170c4cd63a99ed326d39a923216563f4f0721325378a7cdf34ce226`  
		Last Modified: Sat, 28 Dec 2019 20:19:43 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aef28adb9261ac35a69849d5571500918f8982cb367407b2fd2809608c0e6b5`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ad091ce1cb239b0012874b210006f7c03b53cdffa8ccb08111b869af2038fb`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d3bfe1ba07823cbf208809c693031e47cadbbc426392afd2b144b82a46b89`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7c4357ace9f66702187924dddaff72c659358a6ca5bbebcfbd28172af34a6`  
		Last Modified: Sun, 29 Dec 2019 04:53:26 GMT  
		Size: 71.2 MB (71194229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d489ec07beb31e3bc26690c954bc8d3947b0d7e100e4330fd1f3df46063eada2`  
		Last Modified: Sun, 29 Dec 2019 04:53:09 GMT  
		Size: 2.9 MB (2863120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70693b42d7923b4de1af7d1589cd7e90d85dd93a4a006c1ba1fd87743d8518bf`  
		Last Modified: Sun, 29 Dec 2019 04:53:08 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd69fc3ce7f2a3a104d20646b0de010935a9ad957b295341be2819810a6e86af`  
		Last Modified: Sun, 29 Dec 2019 04:53:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388010d812fdf9ae47b37b35ecde2ce0cdd9107a8f8bde03a9d44d4043a1a81f`  
		Last Modified: Sun, 29 Dec 2019 04:53:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd27acebe654b560f4a52cf3c0aa0a4f48a9acbe6f625c4659cb89d9fe398b`  
		Last Modified: Sun, 29 Dec 2019 04:53:21 GMT  
		Size: 38.4 MB (38403931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:1.33.2`

```console
$ docker pull mediawiki@sha256:9b946c708b7cfc499c83f06eb8b36eecdc3ecc6e76235417d6cdce18e9cd4e5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:1.33.2` - linux; amd64

```console
$ docker pull mediawiki@sha256:359fa8b601cbab9afc052a3d172fdf9729e82ea83dc805522c40a8de4cc60552
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254485539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af8f16c5019a4cd2e3365c6b95efab1a7af3b715c3f62805aff87afae26499d4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 22:06:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 22:06:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 22:06:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 22:10:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:56 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 22:10:56 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 22:10:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 22:10:57 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 22:10:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:57 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 22:10:57 GMT
EXPOSE 80
# Sat, 28 Dec 2019 22:10:58 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 11:00:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:38 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 11:01:39 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 11:01:40 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 11:01:48 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616effb632b1d9a229db46a4895f96ef822ed289120d5820f528d4e6d0196b04`  
		Last Modified: Sat, 28 Dec 2019 22:57:09 GMT  
		Size: 12.6 MB (12647459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20683410f309796015435a6c488b34d56f15a42751e53182ff36f9589a697aec`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39e604a3ca40968baa97b55862347eba6db9604fb7009f3b140a5b8a63a48f7`  
		Last Modified: Sat, 28 Dec 2019 22:57:11 GMT  
		Size: 13.8 MB (13840313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc05a4fae7428f9a56c576785244bc2c23c2cd11adec6c8d2a3e4446982b166`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e1a9337fe9acff76d7b3f49a9a55510ef7fa6af7ffa212294bf246d536d62`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1dfa87b2cec32d510224acaaa0ed06f71454e729937f1fb8c17d220fc5476`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b1c9144c1bfcaa8ce4f98f8f98a494041cce5252a5fb21132bb08f4a558e93`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb7894808376d3aa265e25e2dd498af7ded4951ad942b6579cb032969a17010`  
		Last Modified: Sun, 29 Dec 2019 11:02:49 GMT  
		Size: 64.4 MB (64382372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10650c299fdf015820f54960323b5705dce3208624414e83e10dda51b30d2b1d`  
		Last Modified: Sun, 29 Dec 2019 11:02:36 GMT  
		Size: 2.8 MB (2785348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1f8f053ad728d5a3674d533f9858336736035c682b1476a00d7a62e35d5f6b`  
		Last Modified: Sun, 29 Dec 2019 11:02:35 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c81fb66e89a2da8a55d652fb13c1b3b54d11beacc5777d5842e948aae0da212`  
		Last Modified: Sun, 29 Dec 2019 11:02:35 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280d802648d655bef8649725137c4f2feaa1c387d210ed7de2fdd91e4f07f1ae`  
		Last Modified: Sun, 29 Dec 2019 11:02:35 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e16fd8e49e1c7ebad393b0d86f6cc2dbc09d0e115e46ca5c4ba98d826125b`  
		Last Modified: Sun, 29 Dec 2019 11:02:47 GMT  
		Size: 38.4 MB (38403961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33.2` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:b9f3641156d3468cf34ac5a25d90eeef966bba06dc7506b715466d8606ebd32f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229056039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0129845204b9a068d23aa5ec3b344ba77093bdfd5a78ccadffaeeb3696130f2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:45:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Jan 2020 21:28:17 GMT
ENV PHP_VERSION=7.2.27
# Thu, 23 Jan 2020 21:28:18 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 21:28:19 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Thu, 23 Jan 2020 21:28:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 21:28:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 21:31:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 21:31:59 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 21:31:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 21:32:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 21:32:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:32:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 21:32:02 GMT
EXPOSE 80
# Thu, 23 Jan 2020 21:32:03 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:56:50 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:58:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:58:55 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 00:58:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:58:58 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:58:59 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 24 Jan 2020 00:58:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 24 Jan 2020 00:59:00 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Fri, 24 Jan 2020 00:59:00 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Fri, 24 Jan 2020 00:59:18 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2617be9432165f4ff50def4500ca5fcf541952391f0a5d4df67701bc394d2`  
		Last Modified: Thu, 23 Jan 2020 22:08:58 GMT  
		Size: 12.6 MB (12643254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8551c3f5356bf3cfa0a66e3855a0efe8066fe7e70afa47dff31910b97c986848`  
		Last Modified: Thu, 23 Jan 2020 22:08:46 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e729b7434145feec1c3d5e04f80e1c1e86d9e3e52bf329654c9e522b77de3e3b`  
		Last Modified: Thu, 23 Jan 2020 22:08:55 GMT  
		Size: 12.9 MB (12916666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b334636761919b50da4d1829bfaa0354494d1b74a4685041f786014c80cbf5`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3b4973e24f949da38cb81cd021c43453b3836f4745a762576934f89f0eedf4`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b9ab9698f568ba92711f2374a519a4b890fd3eada0b0094b4d69ab1e53891`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b083b324bc21fe14166b4df6df5698a848059740fab4c17079e43447727cc`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88798ca1063ce18ba0743649b0557aa3680d5d097f1ae254b83e3eafafc3c35`  
		Last Modified: Fri, 24 Jan 2020 01:01:57 GMT  
		Size: 60.7 MB (60727513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc48db92f8f0104e85ad6ea21e7710bd9a7011e5a6d84d7a1aee9190902329c`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 2.7 MB (2704392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1530367864dd497a5a8d1c2ddfc9a2619fcbd68613440fca5d360a4072002a`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4994b55ac4ae7d781c41887b7d2fde42a3f5db31099437695557d18738778269`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a99c54f8644a844a3d269e5af8e3f3646bef4c1ab3394ba007c3e000605b801`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b6f6b9e1358d41cba72f67e16f5b9415ec954f1acdc2f7636f2c2b93208e66`  
		Last Modified: Fri, 24 Jan 2020 01:01:44 GMT  
		Size: 38.4 MB (38404270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33.2` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:5aa506775a4c82a6648de1da7c0ff77fc0b4b121018c22811ed55db57d335482
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222586741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8feab2dad602b08a9f2979979d72382a5abcdc7a1e0877b44f1b3aa2fda7eb0c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:39:38 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 16:39:39 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 16:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:39:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:42:54 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:59 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:43:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:43:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:43:06 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:43:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:43:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:43:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:43:12 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:09:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:11:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:11:21 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 05:11:24 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:11:27 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:11:27 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 05:11:28 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 05:11:29 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 05:11:30 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 05:11:54 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3334f18cf3c9b09c2bb03110d24b806ceed4445b5da5e355e03e723c2b1614`  
		Last Modified: Sat, 28 Dec 2019 17:15:13 GMT  
		Size: 12.6 MB (12645461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eae1e83fddba25d3172b588bce688c3a310608a4bfe25de808e0eb566a04ebf`  
		Last Modified: Sat, 28 Dec 2019 17:15:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fbe17d996b2504cdc42ee40f7d649eca4aaa5be19429a4e539b3329ceb2148`  
		Last Modified: Sat, 28 Dec 2019 17:15:17 GMT  
		Size: 12.2 MB (12186080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2220d9961faeb5bedaefe8a20906c5f3c4539d6f03db8fb786855229732a4c`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc727f308c74cad30c947c8f15188cd2421c2acc731fe9c241b40c6feb1d00`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b81aa860ae65f310e7d52b99ebbd6e7444918b85929de2baa85b188c3863bdb`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128b3062692808ff44cfdd5411ee2739d2edda2e2dcd26883380e709464a2c4d`  
		Last Modified: Sat, 28 Dec 2019 17:15:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0deac41ba566db06f7dc310d07c83a525c13c2e98ea39414561b700d4ce4a66`  
		Last Modified: Sun, 29 Dec 2019 05:13:44 GMT  
		Size: 57.0 MB (57012633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8b99ec8846b071347e924fa2af35fa376c29870cb54fbd15d2a78ca96dd5df`  
		Last Modified: Sun, 29 Dec 2019 05:13:27 GMT  
		Size: 2.6 MB (2649286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e60ec632bf71f86563144cf4e35fc8c513c33c852cb9e765ffc2875df6cf75`  
		Last Modified: Sun, 29 Dec 2019 05:13:26 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0249bc474c5b8c2d6456c07afcbe23f67ecf3f7895e619e454e14950026623a3`  
		Last Modified: Sun, 29 Dec 2019 05:13:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34394ad2ae2eb0f7e2b44365a3da6453e7f56f54edfa10bd16c29ce78de8fd4`  
		Last Modified: Sun, 29 Dec 2019 05:13:26 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff479b89d9f4d4d29d66bbd143f96e9932f6e46ad85cfa4c209a3976fb481ebc`  
		Last Modified: Sun, 29 Dec 2019 05:13:46 GMT  
		Size: 38.4 MB (38404118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33.2` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:e59c6d09ef010365ddbd5490c515fcf67e67934b670e687c62f9cca9cfc56fbc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244298301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e38b5d01f808594bc7aeacdcb08eb4a35e5ec186170a68a354fb6896a84744d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 15:33:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 15:33:35 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 15:33:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 15:33:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:37:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:13 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:37:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:37:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:37:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:37:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:21 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:37:22 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:37:23 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:23:20 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:25:05 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 06:25:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:25:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:25:11 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 06:25:12 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 06:25:13 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 06:25:14 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 06:25:32 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef55e879c10bb0bfe58b0e87d612c419ea5bd7503872b20b4f204c4ff29fc529`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 12.6 MB (12646118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f6952b67823bbc1f9d02a4c84126ee319f7453c8b50ba5c15d230f582a24cb`  
		Last Modified: Sat, 28 Dec 2019 16:12:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1409df52b683c197e2f155c5fff7655f3685cba677ed3cd88500b5c50a0b322e`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 13.5 MB (13537744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a0571861c31f3e3e66ef375bed45e5baf9b06264b2c21f16c281c14a6e425a`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5f5ab5fff422d4c5851f79af8e8bcd99629a1d824101f26afe878f49641733`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd643e176f0541609f1cc882c4c2bf40a168ea1a2774bbba5dddea14492e4c14`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266f7b1f11a53b6b15316c0eefecf0d4b8647f2672c42d0b8a7f745bb9939ae3`  
		Last Modified: Sat, 28 Dec 2019 16:12:19 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293f6ae45064ffc9bead71caf085d167b46041ea02c548d0a5051becaf93b138`  
		Last Modified: Sun, 29 Dec 2019 06:27:48 GMT  
		Size: 62.2 MB (62181447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4189a9c54e310f0ed59abeeb288b039c62fbea382ad7b6d2fa91460e2d444d95`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 2.8 MB (2758645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3505bbad6e024712a3e32a22eae39e7270a0b97234e28ff9a5b0d460eab6c7ea`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d709b64262da7fb53be566d00c67b818fa62979cb819bc33a488482e4c45`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83262d9002968ac1df9efc63e137fec1a20648d0226372b894bf3dd7cf677ce7`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d448e490744eb93dfc7686d0e48e79bfd88b23f1d6a71fbfdfda20b2d23f237`  
		Last Modified: Sun, 29 Dec 2019 06:27:48 GMT  
		Size: 38.4 MB (38404077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33.2` - linux; 386

```console
$ docker pull mediawiki@sha256:744ce0f47bf1ea291f021f8c301b3e4356242963fb5e12dde1af01de09ef5d3c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262389336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6da020e16b26371a7ebccfb387cad0361dc6f827c27a8a2883691ec4440d066`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:36:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 18:36:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:36:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:41:53 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:41:54 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:41:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:41:55 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:41:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:55 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:41:55 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:41:55 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:52:44 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:54:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:54:48 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 01:54:49 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:54:50 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:54:50 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 01:54:51 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 01:54:51 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 01:54:51 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 01:55:09 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7cf80bc7d8085b8ce0a31e3a98f5693961c49434a02d4140d3c71a07ca565`  
		Last Modified: Sat, 28 Dec 2019 19:37:07 GMT  
		Size: 12.6 MB (12646713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a2cb9f569f09db2f619aa046f4b6508bf2a6734586800e94606e2cd6d4c56d`  
		Last Modified: Sat, 28 Dec 2019 19:37:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59eac3b46370851360f3dd6921cd777da75f7e064a3f2b86bca60969d4f11e3`  
		Last Modified: Sat, 28 Dec 2019 19:37:11 GMT  
		Size: 14.2 MB (14165526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365a0af4c7ee6ef2bf0e01e4dd3aa80cdf65b41072447cd02e375d3da249dcb`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ffa88e5eec5d45da757fb19b139ff9468309d797987ffc10120d9538947db2`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec1aab950c8691b268d3ee910c230ebe39a8c86cd15872a46d482d9d919987`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8735cfcf9ac1f26b597e58e0dc46c495468cb03cb7bef0c4400da5e8fdbd7cca`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70d0681d2078e2326a14831637f16c3b57fe8f03a55b3f90fc6fb689aba645`  
		Last Modified: Sun, 29 Dec 2019 01:57:23 GMT  
		Size: 66.3 MB (66332499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a47642cce4d2c51efea83292928b49c8938d7cfcc64b60d49387d9e5fa0466`  
		Last Modified: Sun, 29 Dec 2019 01:56:48 GMT  
		Size: 2.8 MB (2775897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424ab26a745ac3ea474c6f774ae98ac511d55c937d311dc3130b691647170065`  
		Last Modified: Sun, 29 Dec 2019 01:56:47 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdc270e7a25645ace70eb291be080460db20a6b91e979a3891aa0b8ebfc4fd8`  
		Last Modified: Sun, 29 Dec 2019 01:56:46 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb590edb4822037944e08e48ecfc21c928abb49b7ac0428ebe5a5efd6d946639`  
		Last Modified: Sun, 29 Dec 2019 01:56:46 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b797c353e22d07dd62f666bbb41f01d3b4008b2d631fabe5b428e818e4b70a`  
		Last Modified: Sun, 29 Dec 2019 01:57:18 GMT  
		Size: 38.4 MB (38403827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33.2` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:a255a5fd8dbbb5d5c5a2e4779f636f7eb65cdb347fbcac310c9de5843ffe2cf2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272585730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:153f3fb344733f1c2e1d2a8513bfbaf29d328c5c85f441a7b86c1aeb7e19221b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 19:27:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 19:27:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 19:27:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 19:27:39 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 19:28:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 19:28:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 19:33:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:08 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 19:33:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 19:33:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 19:33:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 19:33:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:25 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 19:33:28 GMT
EXPOSE 80
# Sat, 28 Dec 2019 19:33:32 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:49:09 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:50:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:50:39 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 04:50:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:50:48 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:50:49 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 04:50:51 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 04:50:53 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 04:50:54 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 04:51:09 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed447e92ed09c9a464d9a1193550b84f1554bb96dd375ae2518965c4acc5e7`  
		Last Modified: Sat, 28 Dec 2019 20:19:48 GMT  
		Size: 12.6 MB (12647171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98bdd73f274ddf4d613631b79831e24954ed7bdcbc3001a970ab2673c90191`  
		Last Modified: Sat, 28 Dec 2019 20:19:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dea2440f3d8645d587221a106bb249affd61425e76cc2ddd5dde65e8557233`  
		Last Modified: Sat, 28 Dec 2019 20:19:49 GMT  
		Size: 14.9 MB (14882224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649bcaf54170c4cd63a99ed326d39a923216563f4f0721325378a7cdf34ce226`  
		Last Modified: Sat, 28 Dec 2019 20:19:43 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aef28adb9261ac35a69849d5571500918f8982cb367407b2fd2809608c0e6b5`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ad091ce1cb239b0012874b210006f7c03b53cdffa8ccb08111b869af2038fb`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d3bfe1ba07823cbf208809c693031e47cadbbc426392afd2b144b82a46b89`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7c4357ace9f66702187924dddaff72c659358a6ca5bbebcfbd28172af34a6`  
		Last Modified: Sun, 29 Dec 2019 04:53:26 GMT  
		Size: 71.2 MB (71194229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d489ec07beb31e3bc26690c954bc8d3947b0d7e100e4330fd1f3df46063eada2`  
		Last Modified: Sun, 29 Dec 2019 04:53:09 GMT  
		Size: 2.9 MB (2863120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70693b42d7923b4de1af7d1589cd7e90d85dd93a4a006c1ba1fd87743d8518bf`  
		Last Modified: Sun, 29 Dec 2019 04:53:08 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd69fc3ce7f2a3a104d20646b0de010935a9ad957b295341be2819810a6e86af`  
		Last Modified: Sun, 29 Dec 2019 04:53:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388010d812fdf9ae47b37b35ecde2ce0cdd9107a8f8bde03a9d44d4043a1a81f`  
		Last Modified: Sun, 29 Dec 2019 04:53:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd27acebe654b560f4a52cf3c0aa0a4f48a9acbe6f625c4659cb89d9fe398b`  
		Last Modified: Sun, 29 Dec 2019 04:53:21 GMT  
		Size: 38.4 MB (38403931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:1.34`

```console
$ docker pull mediawiki@sha256:79b7ca659bb4b514ce4a2df205bea76d8cd9e29ab5636735a3531c514c2478d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:1.34` - linux; amd64

```console
$ docker pull mediawiki@sha256:fa2e7a9e8eeb91fbb6e39cc2c8846a111aa6efe8876a08ba4bab155ca63da1b9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.1 MB (257115331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f7db6799cb077e044fe43ac250c57c391c666f26c7bbf8b3c698e318ea7ce15`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 21:12:38 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 21:12:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 21:12:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 21:17:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:03 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 21:17:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 21:17:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 21:17:04 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 21:17:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:05 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 21:17:05 GMT
EXPOSE 80
# Sat, 28 Dec 2019 21:17:05 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 10:58:27 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 10:59:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 10:59:41 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 10:59:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 10:59:43 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 10:59:52 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e316fd5b3b31a7c6ac4320517a41f6bbb3eb02f527cfc8fae23ca0dc68ffebd`  
		Last Modified: Sat, 28 Dec 2019 22:55:15 GMT  
		Size: 12.4 MB (12440404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578b40496c371640b6bb2c25d655d386b471ca78f820f28dcbb500506430c489`  
		Last Modified: Sat, 28 Dec 2019 22:55:13 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814ae7711d3c4266c8bffe679dd7ce200e879a32943f9b5c760806fed9877627`  
		Last Modified: Sat, 28 Dec 2019 22:55:18 GMT  
		Size: 14.1 MB (14078040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4896fed78b6b0c6ece3825c30fa479aad229a8e7cfcea2236e42207167310e20`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d71e9611db3c5ae3e77251f4091fbde1cc7d62fdaf0e05321eb618acb1081`  
		Last Modified: Sat, 28 Dec 2019 22:55:13 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46017765526c6535682249b21a12ab2f2b85da2047896a62c0874e068682c867`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28038609845819461b2f18a28f6d89b977b43ee6c7c33ec6c8d833739b20503e`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4c6dc86636371d2f17622db1191fa4a2e3db0a19a0e546bb1b6fe958acab10`  
		Last Modified: Sun, 29 Dec 2019 11:02:29 GMT  
		Size: 64.4 MB (64382208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78773447511cfd68c3fca6dcbec102b4be71e21e87aeb7d3478fde32e151c136`  
		Last Modified: Sun, 29 Dec 2019 11:02:16 GMT  
		Size: 2.9 MB (2856667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb5f3759c20331020223e292ad0037973aeeea83337fcd9d78c978baf8f654`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c28e9635c157094f7faec7c7303005ea7e4004d716060598f8994bec784101`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5b1ac8187703f0cd091b241689517343104c6fd3691120f7432f4fb7817ab8`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9be11e3e301dc81628d2df0396841a8873a4e36e92f48adde51a182450c3bb3`  
		Last Modified: Sun, 29 Dec 2019 11:02:27 GMT  
		Size: 40.9 MB (40931929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:2a59cf5694724bdc3104e9e9a83f4d324bacc9dda1983e01d8209f16f11a55b4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231632999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bd487ee3bdb02521edabdbaf4507312a5c154e8c208254b9213103d6ffcddc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:09:24 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Jan 2020 20:52:31 GMT
ENV PHP_VERSION=7.3.14
# Thu, 23 Jan 2020 20:52:32 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.14.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.14.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 20:52:32 GMT
ENV PHP_SHA256=cc05dd373ca5d36652800762f65c10e828a17de35aaf246262e3efa99d00cdb0 PHP_MD5=
# Thu, 23 Jan 2020 20:52:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 20:52:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 20:56:08 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:10 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 20:56:12 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 20:56:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 20:56:14 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 20:56:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:15 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 20:56:15 GMT
EXPOSE 80
# Thu, 23 Jan 2020 20:56:16 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:52:57 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:54:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:54:48 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 00:54:50 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:54:52 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:54:53 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 24 Jan 2020 00:54:53 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 24 Jan 2020 00:54:54 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Fri, 24 Jan 2020 00:54:55 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Fri, 24 Jan 2020 00:55:14 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cfdf0470bce0679253384cf02f9f1b896fb4665bedb65be5023e0e950e7a3b`  
		Last Modified: Thu, 23 Jan 2020 22:04:53 GMT  
		Size: 12.4 MB (12442341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f9507d43050ba009b8afb20570d27bad84ee2e000949f7a885fdb0ef4f1557`  
		Last Modified: Thu, 23 Jan 2020 22:04:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412c7b752a5d961cf2d2ec06b55c62dcbb7efdd5e5f55dec745c459b5ebb4ffb`  
		Last Modified: Thu, 23 Jan 2020 22:04:40 GMT  
		Size: 13.1 MB (13096070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791346c7fb72630bee2dfd762c43e4852e134ac1da979744fd67ed0aaf6a6b03`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c80400256513da81e6a7768c42565cbc9f674c778d2bd0b3b7e51153ac63cf`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46ccc7504b358e47f682a6f4a2c3e04eb75e9d4755563239f063ee7237f47da`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd1668a5072f1159e7d273194180e9d2c696372e381f8ed31b977ecf210c8d8`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef4e257e74e23370b32c8129e66472fee2b920888c673eec95f0f0bb8dfb392`  
		Last Modified: Fri, 24 Jan 2020 01:01:02 GMT  
		Size: 60.7 MB (60728020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60803715dcb5429ed46dd9c5323a5bf8a61ad55a3dc275e1f69b91fd5c67084`  
		Last Modified: Fri, 24 Jan 2020 01:00:21 GMT  
		Size: 2.8 MB (2773953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1b3320ab21de757eb540ea6ae9c72e9c8edd27ce1ffb99a6e3566f3a31ecd6`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0badbebef8582d532b9e59061158039e5992e6ffe99d6bcb984ead050942b2e9`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7510e9105626e90e19a149010b107192574f107d91ffa836bcdbfbad33b6a6`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c694bee0d570fb407c748485c00be541e026fb9680005fa5dbc0a7eec5e6f`  
		Last Modified: Fri, 24 Jan 2020 01:00:58 GMT  
		Size: 40.9 MB (40932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:bb2cde30cfb77bbefc0747a44414af3d4ccd4dbc9f6c27a3589510e08c6f8bdd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225173738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989fa8539446c99e6a7bb303e7248decb122e4a4641aa0b237e0442d24ecd36f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:04:33 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 16:04:34 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 16:04:35 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:04:35 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 16:04:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:04:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:07:44 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:46 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:07:48 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:07:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:07:49 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:07:50 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:50 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:07:51 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:07:52 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:04:06 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:06:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:06:32 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 05:06:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:06:38 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:06:39 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 05:06:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 05:06:48 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 05:06:52 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 05:07:22 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba412d4719663d33c51866d47de7345e1621312855e2db94800f664f40f9fc46`  
		Last Modified: Sat, 28 Dec 2019 17:12:50 GMT  
		Size: 12.4 MB (12438758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158410b29bc5cad857c8af8d243e90a2ef5c21d0f270cd6f3eb9f14192bfdb49`  
		Last Modified: Sat, 28 Dec 2019 17:12:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53d0ff92ce7f082a72df95f2334266d4209b0dca7c7c8c7ce8aea0ee8b25b07`  
		Last Modified: Sat, 28 Dec 2019 17:12:51 GMT  
		Size: 12.4 MB (12389028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a6a7649fcf1dc3b10b9d139d9bf7e601383add0639abc28ec09fb660733f14`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efe161da3c5f30edf92e6113f47c5f5ec90557610df7bc1d23153fa786c541e`  
		Last Modified: Sat, 28 Dec 2019 17:12:48 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918b07eae5c339e0737ac9c830418b24d504eee6e03986cf7353f8319c89f81`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452371523c58e6c53c6b43b2e7083bd45d47aa8563718ea062976b7f6d65bff5`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e7b431fc2b68efc8f852bed077d13b915fee8e76e4d608b5426d395afbae89`  
		Last Modified: Sun, 29 Dec 2019 05:13:10 GMT  
		Size: 57.0 MB (57013104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dc54d7e0e858778ed287c4d054b42747522b4ebe67e7a57f868060dce8d514`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 2.7 MB (2711321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461d0281d7782cdaf29caf55dafb9b802a3cbd0af7793123b086133c8e622d33`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0e2b5086c134e4aced9bbdcc59edcc492ddec6cfa7191932a3a5b4b422cc0c`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6903a78739071fb34b5aa3b5d6977902597d42343e9b401771bc228b392928`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dcdcc55cd54b87347584b0f9a743f1cc3d88b86f1bf1b44fcca57f06e89a6d`  
		Last Modified: Sun, 29 Dec 2019 05:13:12 GMT  
		Size: 40.9 MB (40932366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:c41b4fece19a7eda9df74a8ad973b0085146bbf33a6c2394a56f53d1f5142691
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246913885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f70165dace035f4eeac8964f6f9667b9da5d3ba26fb151f86c029f2538324383`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 14:58:04 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 14:58:05 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 14:58:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 14:58:07 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 14:58:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 14:58:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:01:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:01:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:02:01 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:02:05 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:02:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:02:07 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:02:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:02:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:02:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:02:13 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:18:45 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:20:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:20:37 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 06:20:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:20:54 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:20:57 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 06:20:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 06:21:01 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 06:21:04 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 06:21:23 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8241649bcf4d2c0e4de74b5e67bb5834ba5d996b49389c84d0f32a989b53ede4`  
		Last Modified: Sat, 28 Dec 2019 16:09:56 GMT  
		Size: 12.4 MB (12439327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e01a20edc8a7bd66d5648fcb221677d86430c207f9c97968483929222df1c9`  
		Last Modified: Sat, 28 Dec 2019 16:09:54 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdd333a6533fb4ebd12aa95ac0a21a8138a145f155144da2109445c06188c45`  
		Last Modified: Sat, 28 Dec 2019 16:09:58 GMT  
		Size: 13.8 MB (13763525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5992756a97c614d861128176ca4f21bbeb5c28e8c94e0127dbfc7bd01cb0141e`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e040aa8fe3067cbf62833e3e2b0452a789c765202130cc632949a1f135b4598c`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a45d8c12182c605c0d3ccdcc1c7e8d537d422b7a7692da668bd44bd9a863412`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab7296dc5aacd20a3cb5406612d125fa5d253c6fbf175024b04a6f885293db0`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520f8b3f9930cceaf2ab7fbea0dab9f280b0c4c910f6b92a0a0d1dcfefb5074`  
		Last Modified: Sun, 29 Dec 2019 06:27:19 GMT  
		Size: 62.2 MB (62181139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d1f01cb89b01ac2491622e4180fb78330e3ae3d35ac94e31769783921b021`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 2.8 MB (2827061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0645b51c7b70e20eb35c2f55959a9114ac5987935dd6ea3769bf087f2f531`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3104adb907115dbcaf78d8db11472e663e3c693b2bdd717bfd0f7c864e5db`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abc8f4b9512b7d519327ed7527cbdc7ea7c6dddbf4fc2107034665c8e3a3479`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0776b66828933d5d10d8d9e28113786b148f524f6466240561b9156a41555a4`  
		Last Modified: Sun, 29 Dec 2019 06:27:19 GMT  
		Size: 40.9 MB (40932574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34` - linux; 386

```console
$ docker pull mediawiki@sha256:0fd3e08dd5184937450379bb85b426ed9e87f236dd49b62d192acf329a77991b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.0 MB (265026151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83455a08dd11ca0df8cf1c9e88237819f4f026508f361a6b79f5446dbfe65d7c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 17:28:59 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 17:28:59 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 17:28:59 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 17:29:00 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 17:29:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 17:29:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 17:34:27 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:28 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 17:34:28 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 17:34:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 17:34:29 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 17:34:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:29 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 17:34:30 GMT
EXPOSE 80
# Sat, 28 Dec 2019 17:34:30 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:49:08 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:51:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:51:35 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 01:51:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:51:36 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 01:51:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbae8f4e561644d6fcb797a8a499d14be3b8e5f4e64cd9c11866211c3aa75b8e`  
		Last Modified: Sat, 28 Dec 2019 19:34:27 GMT  
		Size: 12.4 MB (12439783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2200f9f0e9086bbdd7693678f3fc977f28b45179fcd97d345cb8bf2303796ae6`  
		Last Modified: Sat, 28 Dec 2019 19:34:25 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5683d09b9e01268b13b81e0a6d2a42ba144c7afe1b5f84192459f6421e4ce10`  
		Last Modified: Sat, 28 Dec 2019 19:34:30 GMT  
		Size: 14.4 MB (14397717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97025580058c4727f58cd59f45f94aadef3f08a243448089e64a9d7cf7136557`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0418088aa2e9c1d45141e23bdaca8c4130ed3a741643b629eb1057fbfa16f04`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896d0f7b562bcc05e29ac3bcf325266b9635738affb3ee55e59a24d9741a019c`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86f2a214dfd81d395465643bc44d03d6d0ab7552ed58686d2f7745e34fadb43`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d40990dd467c89da4a260e98d10d7a90f664d3169c2a48bf598db40f60e8b6`  
		Last Modified: Sun, 29 Dec 2019 01:56:39 GMT  
		Size: 66.3 MB (66332990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6febce75820693e6c4e898a065204a7bb7787d9810aac90d7a8512f2083a8d`  
		Last Modified: Sun, 29 Dec 2019 01:55:59 GMT  
		Size: 2.9 MB (2858990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde3d4d1d88f3ed029aa9b4cdd85cd0e676358e0584795979cfcc05a6efda8c7`  
		Last Modified: Sun, 29 Dec 2019 01:55:56 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739e246f8ce3c87dcad419a9e9cd83e0ef3c9e7ff62c34acce2b4c27e6c20ba5`  
		Last Modified: Sun, 29 Dec 2019 01:55:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd6a279f87a22c52a9c476bfd0681f6e67dcb59e4b3dd6e5d1c4f24eb52b27`  
		Last Modified: Sun, 29 Dec 2019 01:55:57 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257a5c5a35d34039bd859cd2fed06fc7d593b686fb11618bd8ee3da909546467`  
		Last Modified: Sun, 29 Dec 2019 01:56:37 GMT  
		Size: 40.9 MB (40931805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:926a1bd0a19244ef37247a70e76af381e5b262a61f13e9ba47c95e90e36f80df
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.2 MB (275228055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29105a492974cb1d750661e2b0cb46f8f38fbf977bda8a4643c09eaf3f3f8187`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:40:03 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 18:40:06 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 18:40:08 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:40:09 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 18:40:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:44:30 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:34 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:44:38 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:44:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:44:43 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:44:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:47 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:44:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:44:49 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:44:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:45:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:46:02 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 04:46:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:46:09 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:46:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 04:46:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 04:46:15 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 04:46:16 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 04:46:30 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9634193639ed291491ea9f346a0554328813bb7b79d0416931174bcdea39df99`  
		Last Modified: Sat, 28 Dec 2019 20:16:00 GMT  
		Size: 12.4 MB (12440219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae57e04f3b19c888646aedbe8a470dee96faf2b4116fd493a4f1f8b558cfd99`  
		Last Modified: Sat, 28 Dec 2019 20:15:57 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21684f23e5fad6d298cee5be9f5edbdb30016b023be97524c1d1a0aae912d64`  
		Last Modified: Sat, 28 Dec 2019 20:16:00 GMT  
		Size: 15.1 MB (15125611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481e0073e5430a6d6ac7f434499ae092a2e4eec3f8cc092e3824f8892d381f`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7793ac58e2b2da04ccc838ca0a711ec7cdb93cf59bc9ce21670a40b597304b51`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d325992be0623123fa8da4459947c53bacdfb00d3d57699f0252a81b33368f2`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5354b81e9a9735e6d42aa4b9979bfbb6b9e0bd673aec99d34604fb687d59be0d`  
		Last Modified: Sat, 28 Dec 2019 20:15:55 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d597b22c2a647f907286930b6aebe07b9930094f9919a9c19e7cb43c6480cca`  
		Last Modified: Sun, 29 Dec 2019 04:52:49 GMT  
		Size: 71.2 MB (71193311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e463f8c0b36c08e1ecbf0b6e0f490530cbbea4e38faf2c0b9bb89da5d0f53d3`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 2.9 MB (2941366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538c2724296bd18e364881c99531c797daab73f2b82832b0efc2281e20a27201`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c569317609dd46d122aca2eecdea14d15a946ffb83e4dc3b642c91db181c51`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d6ec7d4fd0c652a627acb57607c8609a3f34ed4b55403c567976fa88a3c5ef`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f033473836325de151dac311fd5af5f0c1ceff5abe02450702668a155f9a25`  
		Last Modified: Sun, 29 Dec 2019 04:52:44 GMT  
		Size: 40.9 MB (40932495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:1.34.0`

```console
$ docker pull mediawiki@sha256:79b7ca659bb4b514ce4a2df205bea76d8cd9e29ab5636735a3531c514c2478d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:1.34.0` - linux; amd64

```console
$ docker pull mediawiki@sha256:fa2e7a9e8eeb91fbb6e39cc2c8846a111aa6efe8876a08ba4bab155ca63da1b9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.1 MB (257115331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f7db6799cb077e044fe43ac250c57c391c666f26c7bbf8b3c698e318ea7ce15`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 21:12:38 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 21:12:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 21:12:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 21:17:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:03 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 21:17:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 21:17:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 21:17:04 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 21:17:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:05 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 21:17:05 GMT
EXPOSE 80
# Sat, 28 Dec 2019 21:17:05 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 10:58:27 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 10:59:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 10:59:41 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 10:59:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 10:59:43 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 10:59:52 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e316fd5b3b31a7c6ac4320517a41f6bbb3eb02f527cfc8fae23ca0dc68ffebd`  
		Last Modified: Sat, 28 Dec 2019 22:55:15 GMT  
		Size: 12.4 MB (12440404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578b40496c371640b6bb2c25d655d386b471ca78f820f28dcbb500506430c489`  
		Last Modified: Sat, 28 Dec 2019 22:55:13 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814ae7711d3c4266c8bffe679dd7ce200e879a32943f9b5c760806fed9877627`  
		Last Modified: Sat, 28 Dec 2019 22:55:18 GMT  
		Size: 14.1 MB (14078040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4896fed78b6b0c6ece3825c30fa479aad229a8e7cfcea2236e42207167310e20`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d71e9611db3c5ae3e77251f4091fbde1cc7d62fdaf0e05321eb618acb1081`  
		Last Modified: Sat, 28 Dec 2019 22:55:13 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46017765526c6535682249b21a12ab2f2b85da2047896a62c0874e068682c867`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28038609845819461b2f18a28f6d89b977b43ee6c7c33ec6c8d833739b20503e`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4c6dc86636371d2f17622db1191fa4a2e3db0a19a0e546bb1b6fe958acab10`  
		Last Modified: Sun, 29 Dec 2019 11:02:29 GMT  
		Size: 64.4 MB (64382208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78773447511cfd68c3fca6dcbec102b4be71e21e87aeb7d3478fde32e151c136`  
		Last Modified: Sun, 29 Dec 2019 11:02:16 GMT  
		Size: 2.9 MB (2856667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb5f3759c20331020223e292ad0037973aeeea83337fcd9d78c978baf8f654`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c28e9635c157094f7faec7c7303005ea7e4004d716060598f8994bec784101`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5b1ac8187703f0cd091b241689517343104c6fd3691120f7432f4fb7817ab8`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9be11e3e301dc81628d2df0396841a8873a4e36e92f48adde51a182450c3bb3`  
		Last Modified: Sun, 29 Dec 2019 11:02:27 GMT  
		Size: 40.9 MB (40931929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34.0` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:2a59cf5694724bdc3104e9e9a83f4d324bacc9dda1983e01d8209f16f11a55b4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231632999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bd487ee3bdb02521edabdbaf4507312a5c154e8c208254b9213103d6ffcddc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:09:24 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Jan 2020 20:52:31 GMT
ENV PHP_VERSION=7.3.14
# Thu, 23 Jan 2020 20:52:32 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.14.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.14.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 20:52:32 GMT
ENV PHP_SHA256=cc05dd373ca5d36652800762f65c10e828a17de35aaf246262e3efa99d00cdb0 PHP_MD5=
# Thu, 23 Jan 2020 20:52:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 20:52:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 20:56:08 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:10 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 20:56:12 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 20:56:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 20:56:14 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 20:56:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:15 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 20:56:15 GMT
EXPOSE 80
# Thu, 23 Jan 2020 20:56:16 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:52:57 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:54:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:54:48 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 00:54:50 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:54:52 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:54:53 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 24 Jan 2020 00:54:53 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 24 Jan 2020 00:54:54 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Fri, 24 Jan 2020 00:54:55 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Fri, 24 Jan 2020 00:55:14 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cfdf0470bce0679253384cf02f9f1b896fb4665bedb65be5023e0e950e7a3b`  
		Last Modified: Thu, 23 Jan 2020 22:04:53 GMT  
		Size: 12.4 MB (12442341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f9507d43050ba009b8afb20570d27bad84ee2e000949f7a885fdb0ef4f1557`  
		Last Modified: Thu, 23 Jan 2020 22:04:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412c7b752a5d961cf2d2ec06b55c62dcbb7efdd5e5f55dec745c459b5ebb4ffb`  
		Last Modified: Thu, 23 Jan 2020 22:04:40 GMT  
		Size: 13.1 MB (13096070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791346c7fb72630bee2dfd762c43e4852e134ac1da979744fd67ed0aaf6a6b03`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c80400256513da81e6a7768c42565cbc9f674c778d2bd0b3b7e51153ac63cf`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46ccc7504b358e47f682a6f4a2c3e04eb75e9d4755563239f063ee7237f47da`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd1668a5072f1159e7d273194180e9d2c696372e381f8ed31b977ecf210c8d8`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef4e257e74e23370b32c8129e66472fee2b920888c673eec95f0f0bb8dfb392`  
		Last Modified: Fri, 24 Jan 2020 01:01:02 GMT  
		Size: 60.7 MB (60728020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60803715dcb5429ed46dd9c5323a5bf8a61ad55a3dc275e1f69b91fd5c67084`  
		Last Modified: Fri, 24 Jan 2020 01:00:21 GMT  
		Size: 2.8 MB (2773953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1b3320ab21de757eb540ea6ae9c72e9c8edd27ce1ffb99a6e3566f3a31ecd6`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0badbebef8582d532b9e59061158039e5992e6ffe99d6bcb984ead050942b2e9`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7510e9105626e90e19a149010b107192574f107d91ffa836bcdbfbad33b6a6`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c694bee0d570fb407c748485c00be541e026fb9680005fa5dbc0a7eec5e6f`  
		Last Modified: Fri, 24 Jan 2020 01:00:58 GMT  
		Size: 40.9 MB (40932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34.0` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:bb2cde30cfb77bbefc0747a44414af3d4ccd4dbc9f6c27a3589510e08c6f8bdd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225173738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989fa8539446c99e6a7bb303e7248decb122e4a4641aa0b237e0442d24ecd36f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:04:33 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 16:04:34 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 16:04:35 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:04:35 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 16:04:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:04:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:07:44 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:46 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:07:48 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:07:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:07:49 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:07:50 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:50 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:07:51 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:07:52 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:04:06 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:06:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:06:32 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 05:06:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:06:38 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:06:39 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 05:06:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 05:06:48 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 05:06:52 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 05:07:22 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba412d4719663d33c51866d47de7345e1621312855e2db94800f664f40f9fc46`  
		Last Modified: Sat, 28 Dec 2019 17:12:50 GMT  
		Size: 12.4 MB (12438758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158410b29bc5cad857c8af8d243e90a2ef5c21d0f270cd6f3eb9f14192bfdb49`  
		Last Modified: Sat, 28 Dec 2019 17:12:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53d0ff92ce7f082a72df95f2334266d4209b0dca7c7c8c7ce8aea0ee8b25b07`  
		Last Modified: Sat, 28 Dec 2019 17:12:51 GMT  
		Size: 12.4 MB (12389028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a6a7649fcf1dc3b10b9d139d9bf7e601383add0639abc28ec09fb660733f14`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efe161da3c5f30edf92e6113f47c5f5ec90557610df7bc1d23153fa786c541e`  
		Last Modified: Sat, 28 Dec 2019 17:12:48 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918b07eae5c339e0737ac9c830418b24d504eee6e03986cf7353f8319c89f81`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452371523c58e6c53c6b43b2e7083bd45d47aa8563718ea062976b7f6d65bff5`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e7b431fc2b68efc8f852bed077d13b915fee8e76e4d608b5426d395afbae89`  
		Last Modified: Sun, 29 Dec 2019 05:13:10 GMT  
		Size: 57.0 MB (57013104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dc54d7e0e858778ed287c4d054b42747522b4ebe67e7a57f868060dce8d514`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 2.7 MB (2711321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461d0281d7782cdaf29caf55dafb9b802a3cbd0af7793123b086133c8e622d33`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0e2b5086c134e4aced9bbdcc59edcc492ddec6cfa7191932a3a5b4b422cc0c`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6903a78739071fb34b5aa3b5d6977902597d42343e9b401771bc228b392928`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dcdcc55cd54b87347584b0f9a743f1cc3d88b86f1bf1b44fcca57f06e89a6d`  
		Last Modified: Sun, 29 Dec 2019 05:13:12 GMT  
		Size: 40.9 MB (40932366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34.0` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:c41b4fece19a7eda9df74a8ad973b0085146bbf33a6c2394a56f53d1f5142691
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246913885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f70165dace035f4eeac8964f6f9667b9da5d3ba26fb151f86c029f2538324383`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 14:58:04 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 14:58:05 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 14:58:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 14:58:07 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 14:58:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 14:58:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:01:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:01:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:02:01 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:02:05 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:02:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:02:07 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:02:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:02:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:02:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:02:13 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:18:45 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:20:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:20:37 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 06:20:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:20:54 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:20:57 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 06:20:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 06:21:01 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 06:21:04 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 06:21:23 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8241649bcf4d2c0e4de74b5e67bb5834ba5d996b49389c84d0f32a989b53ede4`  
		Last Modified: Sat, 28 Dec 2019 16:09:56 GMT  
		Size: 12.4 MB (12439327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e01a20edc8a7bd66d5648fcb221677d86430c207f9c97968483929222df1c9`  
		Last Modified: Sat, 28 Dec 2019 16:09:54 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdd333a6533fb4ebd12aa95ac0a21a8138a145f155144da2109445c06188c45`  
		Last Modified: Sat, 28 Dec 2019 16:09:58 GMT  
		Size: 13.8 MB (13763525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5992756a97c614d861128176ca4f21bbeb5c28e8c94e0127dbfc7bd01cb0141e`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e040aa8fe3067cbf62833e3e2b0452a789c765202130cc632949a1f135b4598c`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a45d8c12182c605c0d3ccdcc1c7e8d537d422b7a7692da668bd44bd9a863412`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab7296dc5aacd20a3cb5406612d125fa5d253c6fbf175024b04a6f885293db0`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520f8b3f9930cceaf2ab7fbea0dab9f280b0c4c910f6b92a0a0d1dcfefb5074`  
		Last Modified: Sun, 29 Dec 2019 06:27:19 GMT  
		Size: 62.2 MB (62181139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d1f01cb89b01ac2491622e4180fb78330e3ae3d35ac94e31769783921b021`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 2.8 MB (2827061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0645b51c7b70e20eb35c2f55959a9114ac5987935dd6ea3769bf087f2f531`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3104adb907115dbcaf78d8db11472e663e3c693b2bdd717bfd0f7c864e5db`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abc8f4b9512b7d519327ed7527cbdc7ea7c6dddbf4fc2107034665c8e3a3479`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0776b66828933d5d10d8d9e28113786b148f524f6466240561b9156a41555a4`  
		Last Modified: Sun, 29 Dec 2019 06:27:19 GMT  
		Size: 40.9 MB (40932574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34.0` - linux; 386

```console
$ docker pull mediawiki@sha256:0fd3e08dd5184937450379bb85b426ed9e87f236dd49b62d192acf329a77991b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.0 MB (265026151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83455a08dd11ca0df8cf1c9e88237819f4f026508f361a6b79f5446dbfe65d7c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 17:28:59 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 17:28:59 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 17:28:59 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 17:29:00 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 17:29:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 17:29:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 17:34:27 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:28 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 17:34:28 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 17:34:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 17:34:29 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 17:34:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:29 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 17:34:30 GMT
EXPOSE 80
# Sat, 28 Dec 2019 17:34:30 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:49:08 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:51:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:51:35 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 01:51:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:51:36 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 01:51:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbae8f4e561644d6fcb797a8a499d14be3b8e5f4e64cd9c11866211c3aa75b8e`  
		Last Modified: Sat, 28 Dec 2019 19:34:27 GMT  
		Size: 12.4 MB (12439783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2200f9f0e9086bbdd7693678f3fc977f28b45179fcd97d345cb8bf2303796ae6`  
		Last Modified: Sat, 28 Dec 2019 19:34:25 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5683d09b9e01268b13b81e0a6d2a42ba144c7afe1b5f84192459f6421e4ce10`  
		Last Modified: Sat, 28 Dec 2019 19:34:30 GMT  
		Size: 14.4 MB (14397717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97025580058c4727f58cd59f45f94aadef3f08a243448089e64a9d7cf7136557`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0418088aa2e9c1d45141e23bdaca8c4130ed3a741643b629eb1057fbfa16f04`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896d0f7b562bcc05e29ac3bcf325266b9635738affb3ee55e59a24d9741a019c`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86f2a214dfd81d395465643bc44d03d6d0ab7552ed58686d2f7745e34fadb43`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d40990dd467c89da4a260e98d10d7a90f664d3169c2a48bf598db40f60e8b6`  
		Last Modified: Sun, 29 Dec 2019 01:56:39 GMT  
		Size: 66.3 MB (66332990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6febce75820693e6c4e898a065204a7bb7787d9810aac90d7a8512f2083a8d`  
		Last Modified: Sun, 29 Dec 2019 01:55:59 GMT  
		Size: 2.9 MB (2858990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde3d4d1d88f3ed029aa9b4cdd85cd0e676358e0584795979cfcc05a6efda8c7`  
		Last Modified: Sun, 29 Dec 2019 01:55:56 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739e246f8ce3c87dcad419a9e9cd83e0ef3c9e7ff62c34acce2b4c27e6c20ba5`  
		Last Modified: Sun, 29 Dec 2019 01:55:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd6a279f87a22c52a9c476bfd0681f6e67dcb59e4b3dd6e5d1c4f24eb52b27`  
		Last Modified: Sun, 29 Dec 2019 01:55:57 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257a5c5a35d34039bd859cd2fed06fc7d593b686fb11618bd8ee3da909546467`  
		Last Modified: Sun, 29 Dec 2019 01:56:37 GMT  
		Size: 40.9 MB (40931805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34.0` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:926a1bd0a19244ef37247a70e76af381e5b262a61f13e9ba47c95e90e36f80df
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.2 MB (275228055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29105a492974cb1d750661e2b0cb46f8f38fbf977bda8a4643c09eaf3f3f8187`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:40:03 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 18:40:06 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 18:40:08 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:40:09 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 18:40:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:44:30 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:34 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:44:38 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:44:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:44:43 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:44:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:47 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:44:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:44:49 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:44:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:45:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:46:02 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 04:46:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:46:09 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:46:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 04:46:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 04:46:15 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 04:46:16 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 04:46:30 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9634193639ed291491ea9f346a0554328813bb7b79d0416931174bcdea39df99`  
		Last Modified: Sat, 28 Dec 2019 20:16:00 GMT  
		Size: 12.4 MB (12440219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae57e04f3b19c888646aedbe8a470dee96faf2b4116fd493a4f1f8b558cfd99`  
		Last Modified: Sat, 28 Dec 2019 20:15:57 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21684f23e5fad6d298cee5be9f5edbdb30016b023be97524c1d1a0aae912d64`  
		Last Modified: Sat, 28 Dec 2019 20:16:00 GMT  
		Size: 15.1 MB (15125611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481e0073e5430a6d6ac7f434499ae092a2e4eec3f8cc092e3824f8892d381f`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7793ac58e2b2da04ccc838ca0a711ec7cdb93cf59bc9ce21670a40b597304b51`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d325992be0623123fa8da4459947c53bacdfb00d3d57699f0252a81b33368f2`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5354b81e9a9735e6d42aa4b9979bfbb6b9e0bd673aec99d34604fb687d59be0d`  
		Last Modified: Sat, 28 Dec 2019 20:15:55 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d597b22c2a647f907286930b6aebe07b9930094f9919a9c19e7cb43c6480cca`  
		Last Modified: Sun, 29 Dec 2019 04:52:49 GMT  
		Size: 71.2 MB (71193311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e463f8c0b36c08e1ecbf0b6e0f490530cbbea4e38faf2c0b9bb89da5d0f53d3`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 2.9 MB (2941366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538c2724296bd18e364881c99531c797daab73f2b82832b0efc2281e20a27201`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c569317609dd46d122aca2eecdea14d15a946ffb83e4dc3b642c91db181c51`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d6ec7d4fd0c652a627acb57607c8609a3f34ed4b55403c567976fa88a3c5ef`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f033473836325de151dac311fd5af5f0c1ceff5abe02450702668a155f9a25`  
		Last Modified: Sun, 29 Dec 2019 04:52:44 GMT  
		Size: 40.9 MB (40932495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:latest`

```console
$ docker pull mediawiki@sha256:79b7ca659bb4b514ce4a2df205bea76d8cd9e29ab5636735a3531c514c2478d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:latest` - linux; amd64

```console
$ docker pull mediawiki@sha256:fa2e7a9e8eeb91fbb6e39cc2c8846a111aa6efe8876a08ba4bab155ca63da1b9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.1 MB (257115331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f7db6799cb077e044fe43ac250c57c391c666f26c7bbf8b3c698e318ea7ce15`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 21:12:38 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 21:12:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 21:12:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 21:17:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:03 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 21:17:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 21:17:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 21:17:04 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 21:17:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:05 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 21:17:05 GMT
EXPOSE 80
# Sat, 28 Dec 2019 21:17:05 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 10:58:27 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 10:59:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 10:59:41 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 10:59:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 10:59:43 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 10:59:52 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e316fd5b3b31a7c6ac4320517a41f6bbb3eb02f527cfc8fae23ca0dc68ffebd`  
		Last Modified: Sat, 28 Dec 2019 22:55:15 GMT  
		Size: 12.4 MB (12440404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578b40496c371640b6bb2c25d655d386b471ca78f820f28dcbb500506430c489`  
		Last Modified: Sat, 28 Dec 2019 22:55:13 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814ae7711d3c4266c8bffe679dd7ce200e879a32943f9b5c760806fed9877627`  
		Last Modified: Sat, 28 Dec 2019 22:55:18 GMT  
		Size: 14.1 MB (14078040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4896fed78b6b0c6ece3825c30fa479aad229a8e7cfcea2236e42207167310e20`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d71e9611db3c5ae3e77251f4091fbde1cc7d62fdaf0e05321eb618acb1081`  
		Last Modified: Sat, 28 Dec 2019 22:55:13 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46017765526c6535682249b21a12ab2f2b85da2047896a62c0874e068682c867`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28038609845819461b2f18a28f6d89b977b43ee6c7c33ec6c8d833739b20503e`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4c6dc86636371d2f17622db1191fa4a2e3db0a19a0e546bb1b6fe958acab10`  
		Last Modified: Sun, 29 Dec 2019 11:02:29 GMT  
		Size: 64.4 MB (64382208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78773447511cfd68c3fca6dcbec102b4be71e21e87aeb7d3478fde32e151c136`  
		Last Modified: Sun, 29 Dec 2019 11:02:16 GMT  
		Size: 2.9 MB (2856667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb5f3759c20331020223e292ad0037973aeeea83337fcd9d78c978baf8f654`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c28e9635c157094f7faec7c7303005ea7e4004d716060598f8994bec784101`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5b1ac8187703f0cd091b241689517343104c6fd3691120f7432f4fb7817ab8`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9be11e3e301dc81628d2df0396841a8873a4e36e92f48adde51a182450c3bb3`  
		Last Modified: Sun, 29 Dec 2019 11:02:27 GMT  
		Size: 40.9 MB (40931929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:latest` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:2a59cf5694724bdc3104e9e9a83f4d324bacc9dda1983e01d8209f16f11a55b4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231632999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bd487ee3bdb02521edabdbaf4507312a5c154e8c208254b9213103d6ffcddc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:09:24 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Jan 2020 20:52:31 GMT
ENV PHP_VERSION=7.3.14
# Thu, 23 Jan 2020 20:52:32 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.14.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.14.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 20:52:32 GMT
ENV PHP_SHA256=cc05dd373ca5d36652800762f65c10e828a17de35aaf246262e3efa99d00cdb0 PHP_MD5=
# Thu, 23 Jan 2020 20:52:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 20:52:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 20:56:08 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:10 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 20:56:12 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 20:56:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 20:56:14 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 20:56:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:15 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 20:56:15 GMT
EXPOSE 80
# Thu, 23 Jan 2020 20:56:16 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:52:57 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:54:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:54:48 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 00:54:50 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:54:52 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:54:53 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 24 Jan 2020 00:54:53 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 24 Jan 2020 00:54:54 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Fri, 24 Jan 2020 00:54:55 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Fri, 24 Jan 2020 00:55:14 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cfdf0470bce0679253384cf02f9f1b896fb4665bedb65be5023e0e950e7a3b`  
		Last Modified: Thu, 23 Jan 2020 22:04:53 GMT  
		Size: 12.4 MB (12442341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f9507d43050ba009b8afb20570d27bad84ee2e000949f7a885fdb0ef4f1557`  
		Last Modified: Thu, 23 Jan 2020 22:04:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412c7b752a5d961cf2d2ec06b55c62dcbb7efdd5e5f55dec745c459b5ebb4ffb`  
		Last Modified: Thu, 23 Jan 2020 22:04:40 GMT  
		Size: 13.1 MB (13096070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791346c7fb72630bee2dfd762c43e4852e134ac1da979744fd67ed0aaf6a6b03`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c80400256513da81e6a7768c42565cbc9f674c778d2bd0b3b7e51153ac63cf`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46ccc7504b358e47f682a6f4a2c3e04eb75e9d4755563239f063ee7237f47da`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd1668a5072f1159e7d273194180e9d2c696372e381f8ed31b977ecf210c8d8`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef4e257e74e23370b32c8129e66472fee2b920888c673eec95f0f0bb8dfb392`  
		Last Modified: Fri, 24 Jan 2020 01:01:02 GMT  
		Size: 60.7 MB (60728020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60803715dcb5429ed46dd9c5323a5bf8a61ad55a3dc275e1f69b91fd5c67084`  
		Last Modified: Fri, 24 Jan 2020 01:00:21 GMT  
		Size: 2.8 MB (2773953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1b3320ab21de757eb540ea6ae9c72e9c8edd27ce1ffb99a6e3566f3a31ecd6`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0badbebef8582d532b9e59061158039e5992e6ffe99d6bcb984ead050942b2e9`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7510e9105626e90e19a149010b107192574f107d91ffa836bcdbfbad33b6a6`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c694bee0d570fb407c748485c00be541e026fb9680005fa5dbc0a7eec5e6f`  
		Last Modified: Fri, 24 Jan 2020 01:00:58 GMT  
		Size: 40.9 MB (40932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:latest` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:bb2cde30cfb77bbefc0747a44414af3d4ccd4dbc9f6c27a3589510e08c6f8bdd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225173738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989fa8539446c99e6a7bb303e7248decb122e4a4641aa0b237e0442d24ecd36f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:04:33 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 16:04:34 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 16:04:35 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:04:35 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 16:04:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:04:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:07:44 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:46 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:07:48 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:07:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:07:49 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:07:50 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:50 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:07:51 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:07:52 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:04:06 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:06:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:06:32 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 05:06:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:06:38 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:06:39 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 05:06:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 05:06:48 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 05:06:52 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 05:07:22 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba412d4719663d33c51866d47de7345e1621312855e2db94800f664f40f9fc46`  
		Last Modified: Sat, 28 Dec 2019 17:12:50 GMT  
		Size: 12.4 MB (12438758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158410b29bc5cad857c8af8d243e90a2ef5c21d0f270cd6f3eb9f14192bfdb49`  
		Last Modified: Sat, 28 Dec 2019 17:12:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53d0ff92ce7f082a72df95f2334266d4209b0dca7c7c8c7ce8aea0ee8b25b07`  
		Last Modified: Sat, 28 Dec 2019 17:12:51 GMT  
		Size: 12.4 MB (12389028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a6a7649fcf1dc3b10b9d139d9bf7e601383add0639abc28ec09fb660733f14`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efe161da3c5f30edf92e6113f47c5f5ec90557610df7bc1d23153fa786c541e`  
		Last Modified: Sat, 28 Dec 2019 17:12:48 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918b07eae5c339e0737ac9c830418b24d504eee6e03986cf7353f8319c89f81`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452371523c58e6c53c6b43b2e7083bd45d47aa8563718ea062976b7f6d65bff5`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e7b431fc2b68efc8f852bed077d13b915fee8e76e4d608b5426d395afbae89`  
		Last Modified: Sun, 29 Dec 2019 05:13:10 GMT  
		Size: 57.0 MB (57013104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dc54d7e0e858778ed287c4d054b42747522b4ebe67e7a57f868060dce8d514`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 2.7 MB (2711321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461d0281d7782cdaf29caf55dafb9b802a3cbd0af7793123b086133c8e622d33`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0e2b5086c134e4aced9bbdcc59edcc492ddec6cfa7191932a3a5b4b422cc0c`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6903a78739071fb34b5aa3b5d6977902597d42343e9b401771bc228b392928`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dcdcc55cd54b87347584b0f9a743f1cc3d88b86f1bf1b44fcca57f06e89a6d`  
		Last Modified: Sun, 29 Dec 2019 05:13:12 GMT  
		Size: 40.9 MB (40932366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:latest` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:c41b4fece19a7eda9df74a8ad973b0085146bbf33a6c2394a56f53d1f5142691
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246913885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f70165dace035f4eeac8964f6f9667b9da5d3ba26fb151f86c029f2538324383`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 14:58:04 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 14:58:05 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 14:58:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 14:58:07 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 14:58:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 14:58:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:01:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:01:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:02:01 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:02:05 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:02:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:02:07 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:02:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:02:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:02:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:02:13 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:18:45 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:20:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:20:37 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 06:20:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:20:54 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:20:57 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 06:20:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 06:21:01 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 06:21:04 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 06:21:23 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8241649bcf4d2c0e4de74b5e67bb5834ba5d996b49389c84d0f32a989b53ede4`  
		Last Modified: Sat, 28 Dec 2019 16:09:56 GMT  
		Size: 12.4 MB (12439327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e01a20edc8a7bd66d5648fcb221677d86430c207f9c97968483929222df1c9`  
		Last Modified: Sat, 28 Dec 2019 16:09:54 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdd333a6533fb4ebd12aa95ac0a21a8138a145f155144da2109445c06188c45`  
		Last Modified: Sat, 28 Dec 2019 16:09:58 GMT  
		Size: 13.8 MB (13763525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5992756a97c614d861128176ca4f21bbeb5c28e8c94e0127dbfc7bd01cb0141e`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e040aa8fe3067cbf62833e3e2b0452a789c765202130cc632949a1f135b4598c`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a45d8c12182c605c0d3ccdcc1c7e8d537d422b7a7692da668bd44bd9a863412`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab7296dc5aacd20a3cb5406612d125fa5d253c6fbf175024b04a6f885293db0`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520f8b3f9930cceaf2ab7fbea0dab9f280b0c4c910f6b92a0a0d1dcfefb5074`  
		Last Modified: Sun, 29 Dec 2019 06:27:19 GMT  
		Size: 62.2 MB (62181139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d1f01cb89b01ac2491622e4180fb78330e3ae3d35ac94e31769783921b021`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 2.8 MB (2827061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0645b51c7b70e20eb35c2f55959a9114ac5987935dd6ea3769bf087f2f531`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3104adb907115dbcaf78d8db11472e663e3c693b2bdd717bfd0f7c864e5db`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abc8f4b9512b7d519327ed7527cbdc7ea7c6dddbf4fc2107034665c8e3a3479`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0776b66828933d5d10d8d9e28113786b148f524f6466240561b9156a41555a4`  
		Last Modified: Sun, 29 Dec 2019 06:27:19 GMT  
		Size: 40.9 MB (40932574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:latest` - linux; 386

```console
$ docker pull mediawiki@sha256:0fd3e08dd5184937450379bb85b426ed9e87f236dd49b62d192acf329a77991b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.0 MB (265026151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83455a08dd11ca0df8cf1c9e88237819f4f026508f361a6b79f5446dbfe65d7c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 17:28:59 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 17:28:59 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 17:28:59 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 17:29:00 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 17:29:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 17:29:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 17:34:27 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:28 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 17:34:28 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 17:34:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 17:34:29 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 17:34:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:29 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 17:34:30 GMT
EXPOSE 80
# Sat, 28 Dec 2019 17:34:30 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:49:08 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:51:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:51:35 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 01:51:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:51:36 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 01:51:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbae8f4e561644d6fcb797a8a499d14be3b8e5f4e64cd9c11866211c3aa75b8e`  
		Last Modified: Sat, 28 Dec 2019 19:34:27 GMT  
		Size: 12.4 MB (12439783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2200f9f0e9086bbdd7693678f3fc977f28b45179fcd97d345cb8bf2303796ae6`  
		Last Modified: Sat, 28 Dec 2019 19:34:25 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5683d09b9e01268b13b81e0a6d2a42ba144c7afe1b5f84192459f6421e4ce10`  
		Last Modified: Sat, 28 Dec 2019 19:34:30 GMT  
		Size: 14.4 MB (14397717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97025580058c4727f58cd59f45f94aadef3f08a243448089e64a9d7cf7136557`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0418088aa2e9c1d45141e23bdaca8c4130ed3a741643b629eb1057fbfa16f04`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896d0f7b562bcc05e29ac3bcf325266b9635738affb3ee55e59a24d9741a019c`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86f2a214dfd81d395465643bc44d03d6d0ab7552ed58686d2f7745e34fadb43`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d40990dd467c89da4a260e98d10d7a90f664d3169c2a48bf598db40f60e8b6`  
		Last Modified: Sun, 29 Dec 2019 01:56:39 GMT  
		Size: 66.3 MB (66332990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6febce75820693e6c4e898a065204a7bb7787d9810aac90d7a8512f2083a8d`  
		Last Modified: Sun, 29 Dec 2019 01:55:59 GMT  
		Size: 2.9 MB (2858990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde3d4d1d88f3ed029aa9b4cdd85cd0e676358e0584795979cfcc05a6efda8c7`  
		Last Modified: Sun, 29 Dec 2019 01:55:56 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739e246f8ce3c87dcad419a9e9cd83e0ef3c9e7ff62c34acce2b4c27e6c20ba5`  
		Last Modified: Sun, 29 Dec 2019 01:55:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd6a279f87a22c52a9c476bfd0681f6e67dcb59e4b3dd6e5d1c4f24eb52b27`  
		Last Modified: Sun, 29 Dec 2019 01:55:57 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257a5c5a35d34039bd859cd2fed06fc7d593b686fb11618bd8ee3da909546467`  
		Last Modified: Sun, 29 Dec 2019 01:56:37 GMT  
		Size: 40.9 MB (40931805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:latest` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:926a1bd0a19244ef37247a70e76af381e5b262a61f13e9ba47c95e90e36f80df
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.2 MB (275228055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29105a492974cb1d750661e2b0cb46f8f38fbf977bda8a4643c09eaf3f3f8187`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:40:03 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 18:40:06 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 18:40:08 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:40:09 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 18:40:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:44:30 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:34 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:44:38 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:44:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:44:43 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:44:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:47 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:44:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:44:49 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:44:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:45:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:46:02 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 04:46:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:46:09 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:46:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 04:46:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 04:46:15 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 04:46:16 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 04:46:30 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9634193639ed291491ea9f346a0554328813bb7b79d0416931174bcdea39df99`  
		Last Modified: Sat, 28 Dec 2019 20:16:00 GMT  
		Size: 12.4 MB (12440219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae57e04f3b19c888646aedbe8a470dee96faf2b4116fd493a4f1f8b558cfd99`  
		Last Modified: Sat, 28 Dec 2019 20:15:57 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21684f23e5fad6d298cee5be9f5edbdb30016b023be97524c1d1a0aae912d64`  
		Last Modified: Sat, 28 Dec 2019 20:16:00 GMT  
		Size: 15.1 MB (15125611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481e0073e5430a6d6ac7f434499ae092a2e4eec3f8cc092e3824f8892d381f`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7793ac58e2b2da04ccc838ca0a711ec7cdb93cf59bc9ce21670a40b597304b51`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d325992be0623123fa8da4459947c53bacdfb00d3d57699f0252a81b33368f2`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5354b81e9a9735e6d42aa4b9979bfbb6b9e0bd673aec99d34604fb687d59be0d`  
		Last Modified: Sat, 28 Dec 2019 20:15:55 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d597b22c2a647f907286930b6aebe07b9930094f9919a9c19e7cb43c6480cca`  
		Last Modified: Sun, 29 Dec 2019 04:52:49 GMT  
		Size: 71.2 MB (71193311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e463f8c0b36c08e1ecbf0b6e0f490530cbbea4e38faf2c0b9bb89da5d0f53d3`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 2.9 MB (2941366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538c2724296bd18e364881c99531c797daab73f2b82832b0efc2281e20a27201`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c569317609dd46d122aca2eecdea14d15a946ffb83e4dc3b642c91db181c51`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d6ec7d4fd0c652a627acb57607c8609a3f34ed4b55403c567976fa88a3c5ef`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f033473836325de151dac311fd5af5f0c1ceff5abe02450702668a155f9a25`  
		Last Modified: Sun, 29 Dec 2019 04:52:44 GMT  
		Size: 40.9 MB (40932495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:legacy`

```console
$ docker pull mediawiki@sha256:9b946c708b7cfc499c83f06eb8b36eecdc3ecc6e76235417d6cdce18e9cd4e5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:legacy` - linux; amd64

```console
$ docker pull mediawiki@sha256:359fa8b601cbab9afc052a3d172fdf9729e82ea83dc805522c40a8de4cc60552
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254485539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af8f16c5019a4cd2e3365c6b95efab1a7af3b715c3f62805aff87afae26499d4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 22:06:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 22:06:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 22:06:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 22:10:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:56 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 22:10:56 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 22:10:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 22:10:57 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 22:10:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:57 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 22:10:57 GMT
EXPOSE 80
# Sat, 28 Dec 2019 22:10:58 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 11:00:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:38 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 11:01:39 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 11:01:40 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 11:01:40 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 11:01:48 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616effb632b1d9a229db46a4895f96ef822ed289120d5820f528d4e6d0196b04`  
		Last Modified: Sat, 28 Dec 2019 22:57:09 GMT  
		Size: 12.6 MB (12647459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20683410f309796015435a6c488b34d56f15a42751e53182ff36f9589a697aec`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39e604a3ca40968baa97b55862347eba6db9604fb7009f3b140a5b8a63a48f7`  
		Last Modified: Sat, 28 Dec 2019 22:57:11 GMT  
		Size: 13.8 MB (13840313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc05a4fae7428f9a56c576785244bc2c23c2cd11adec6c8d2a3e4446982b166`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e1a9337fe9acff76d7b3f49a9a55510ef7fa6af7ffa212294bf246d536d62`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1dfa87b2cec32d510224acaaa0ed06f71454e729937f1fb8c17d220fc5476`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b1c9144c1bfcaa8ce4f98f8f98a494041cce5252a5fb21132bb08f4a558e93`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb7894808376d3aa265e25e2dd498af7ded4951ad942b6579cb032969a17010`  
		Last Modified: Sun, 29 Dec 2019 11:02:49 GMT  
		Size: 64.4 MB (64382372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10650c299fdf015820f54960323b5705dce3208624414e83e10dda51b30d2b1d`  
		Last Modified: Sun, 29 Dec 2019 11:02:36 GMT  
		Size: 2.8 MB (2785348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1f8f053ad728d5a3674d533f9858336736035c682b1476a00d7a62e35d5f6b`  
		Last Modified: Sun, 29 Dec 2019 11:02:35 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c81fb66e89a2da8a55d652fb13c1b3b54d11beacc5777d5842e948aae0da212`  
		Last Modified: Sun, 29 Dec 2019 11:02:35 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280d802648d655bef8649725137c4f2feaa1c387d210ed7de2fdd91e4f07f1ae`  
		Last Modified: Sun, 29 Dec 2019 11:02:35 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01e16fd8e49e1c7ebad393b0d86f6cc2dbc09d0e115e46ca5c4ba98d826125b`  
		Last Modified: Sun, 29 Dec 2019 11:02:47 GMT  
		Size: 38.4 MB (38403961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:b9f3641156d3468cf34ac5a25d90eeef966bba06dc7506b715466d8606ebd32f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229056039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0129845204b9a068d23aa5ec3b344ba77093bdfd5a78ccadffaeeb3696130f2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:45:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Jan 2020 21:28:17 GMT
ENV PHP_VERSION=7.2.27
# Thu, 23 Jan 2020 21:28:18 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 21:28:19 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Thu, 23 Jan 2020 21:28:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 21:28:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 21:31:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 21:31:59 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 21:31:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 21:32:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 21:32:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:32:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 21:32:02 GMT
EXPOSE 80
# Thu, 23 Jan 2020 21:32:03 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:56:50 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:58:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:58:55 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 00:58:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:58:58 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:58:59 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 24 Jan 2020 00:58:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 24 Jan 2020 00:59:00 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Fri, 24 Jan 2020 00:59:00 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Fri, 24 Jan 2020 00:59:18 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2617be9432165f4ff50def4500ca5fcf541952391f0a5d4df67701bc394d2`  
		Last Modified: Thu, 23 Jan 2020 22:08:58 GMT  
		Size: 12.6 MB (12643254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8551c3f5356bf3cfa0a66e3855a0efe8066fe7e70afa47dff31910b97c986848`  
		Last Modified: Thu, 23 Jan 2020 22:08:46 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e729b7434145feec1c3d5e04f80e1c1e86d9e3e52bf329654c9e522b77de3e3b`  
		Last Modified: Thu, 23 Jan 2020 22:08:55 GMT  
		Size: 12.9 MB (12916666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b334636761919b50da4d1829bfaa0354494d1b74a4685041f786014c80cbf5`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3b4973e24f949da38cb81cd021c43453b3836f4745a762576934f89f0eedf4`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b9ab9698f568ba92711f2374a519a4b890fd3eada0b0094b4d69ab1e53891`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b083b324bc21fe14166b4df6df5698a848059740fab4c17079e43447727cc`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88798ca1063ce18ba0743649b0557aa3680d5d097f1ae254b83e3eafafc3c35`  
		Last Modified: Fri, 24 Jan 2020 01:01:57 GMT  
		Size: 60.7 MB (60727513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc48db92f8f0104e85ad6ea21e7710bd9a7011e5a6d84d7a1aee9190902329c`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 2.7 MB (2704392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1530367864dd497a5a8d1c2ddfc9a2619fcbd68613440fca5d360a4072002a`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 580.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4994b55ac4ae7d781c41887b7d2fde42a3f5db31099437695557d18738778269`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a99c54f8644a844a3d269e5af8e3f3646bef4c1ab3394ba007c3e000605b801`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b6f6b9e1358d41cba72f67e16f5b9415ec954f1acdc2f7636f2c2b93208e66`  
		Last Modified: Fri, 24 Jan 2020 01:01:44 GMT  
		Size: 38.4 MB (38404270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:5aa506775a4c82a6648de1da7c0ff77fc0b4b121018c22811ed55db57d335482
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222586741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8feab2dad602b08a9f2979979d72382a5abcdc7a1e0877b44f1b3aa2fda7eb0c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:39:38 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 16:39:39 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 16:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:39:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:42:54 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:59 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:43:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:43:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:43:06 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:43:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:43:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:43:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:43:12 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:09:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:11:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:11:21 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 05:11:24 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:11:27 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:11:27 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 05:11:28 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 05:11:29 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 05:11:30 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 05:11:54 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3334f18cf3c9b09c2bb03110d24b806ceed4445b5da5e355e03e723c2b1614`  
		Last Modified: Sat, 28 Dec 2019 17:15:13 GMT  
		Size: 12.6 MB (12645461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eae1e83fddba25d3172b588bce688c3a310608a4bfe25de808e0eb566a04ebf`  
		Last Modified: Sat, 28 Dec 2019 17:15:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fbe17d996b2504cdc42ee40f7d649eca4aaa5be19429a4e539b3329ceb2148`  
		Last Modified: Sat, 28 Dec 2019 17:15:17 GMT  
		Size: 12.2 MB (12186080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2220d9961faeb5bedaefe8a20906c5f3c4539d6f03db8fb786855229732a4c`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc727f308c74cad30c947c8f15188cd2421c2acc731fe9c241b40c6feb1d00`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b81aa860ae65f310e7d52b99ebbd6e7444918b85929de2baa85b188c3863bdb`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128b3062692808ff44cfdd5411ee2739d2edda2e2dcd26883380e709464a2c4d`  
		Last Modified: Sat, 28 Dec 2019 17:15:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0deac41ba566db06f7dc310d07c83a525c13c2e98ea39414561b700d4ce4a66`  
		Last Modified: Sun, 29 Dec 2019 05:13:44 GMT  
		Size: 57.0 MB (57012633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8b99ec8846b071347e924fa2af35fa376c29870cb54fbd15d2a78ca96dd5df`  
		Last Modified: Sun, 29 Dec 2019 05:13:27 GMT  
		Size: 2.6 MB (2649286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e60ec632bf71f86563144cf4e35fc8c513c33c852cb9e765ffc2875df6cf75`  
		Last Modified: Sun, 29 Dec 2019 05:13:26 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0249bc474c5b8c2d6456c07afcbe23f67ecf3f7895e619e454e14950026623a3`  
		Last Modified: Sun, 29 Dec 2019 05:13:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34394ad2ae2eb0f7e2b44365a3da6453e7f56f54edfa10bd16c29ce78de8fd4`  
		Last Modified: Sun, 29 Dec 2019 05:13:26 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff479b89d9f4d4d29d66bbd143f96e9932f6e46ad85cfa4c209a3976fb481ebc`  
		Last Modified: Sun, 29 Dec 2019 05:13:46 GMT  
		Size: 38.4 MB (38404118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:e59c6d09ef010365ddbd5490c515fcf67e67934b670e687c62f9cca9cfc56fbc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244298301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e38b5d01f808594bc7aeacdcb08eb4a35e5ec186170a68a354fb6896a84744d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 15:33:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 15:33:35 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 15:33:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 15:33:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:37:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:13 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:37:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:37:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:37:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:37:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:21 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:37:22 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:37:23 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:23:20 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:25:05 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 06:25:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:25:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:25:11 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 06:25:12 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 06:25:13 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 06:25:14 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 06:25:32 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef55e879c10bb0bfe58b0e87d612c419ea5bd7503872b20b4f204c4ff29fc529`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 12.6 MB (12646118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f6952b67823bbc1f9d02a4c84126ee319f7453c8b50ba5c15d230f582a24cb`  
		Last Modified: Sat, 28 Dec 2019 16:12:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1409df52b683c197e2f155c5fff7655f3685cba677ed3cd88500b5c50a0b322e`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 13.5 MB (13537744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a0571861c31f3e3e66ef375bed45e5baf9b06264b2c21f16c281c14a6e425a`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5f5ab5fff422d4c5851f79af8e8bcd99629a1d824101f26afe878f49641733`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd643e176f0541609f1cc882c4c2bf40a168ea1a2774bbba5dddea14492e4c14`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266f7b1f11a53b6b15316c0eefecf0d4b8647f2672c42d0b8a7f745bb9939ae3`  
		Last Modified: Sat, 28 Dec 2019 16:12:19 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293f6ae45064ffc9bead71caf085d167b46041ea02c548d0a5051becaf93b138`  
		Last Modified: Sun, 29 Dec 2019 06:27:48 GMT  
		Size: 62.2 MB (62181447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4189a9c54e310f0ed59abeeb288b039c62fbea382ad7b6d2fa91460e2d444d95`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 2.8 MB (2758645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3505bbad6e024712a3e32a22eae39e7270a0b97234e28ff9a5b0d460eab6c7ea`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8084d709b64262da7fb53be566d00c67b818fa62979cb819bc33a488482e4c45`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83262d9002968ac1df9efc63e137fec1a20648d0226372b894bf3dd7cf677ce7`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d448e490744eb93dfc7686d0e48e79bfd88b23f1d6a71fbfdfda20b2d23f237`  
		Last Modified: Sun, 29 Dec 2019 06:27:48 GMT  
		Size: 38.4 MB (38404077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; 386

```console
$ docker pull mediawiki@sha256:744ce0f47bf1ea291f021f8c301b3e4356242963fb5e12dde1af01de09ef5d3c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262389336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6da020e16b26371a7ebccfb387cad0361dc6f827c27a8a2883691ec4440d066`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:36:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 18:36:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:36:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:41:53 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:41:54 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:41:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:41:55 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:41:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:55 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:41:55 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:41:55 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:52:44 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:54:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:54:48 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 01:54:49 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:54:50 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:54:50 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 01:54:51 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 01:54:51 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 01:54:51 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 01:55:09 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7cf80bc7d8085b8ce0a31e3a98f5693961c49434a02d4140d3c71a07ca565`  
		Last Modified: Sat, 28 Dec 2019 19:37:07 GMT  
		Size: 12.6 MB (12646713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a2cb9f569f09db2f619aa046f4b6508bf2a6734586800e94606e2cd6d4c56d`  
		Last Modified: Sat, 28 Dec 2019 19:37:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59eac3b46370851360f3dd6921cd777da75f7e064a3f2b86bca60969d4f11e3`  
		Last Modified: Sat, 28 Dec 2019 19:37:11 GMT  
		Size: 14.2 MB (14165526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365a0af4c7ee6ef2bf0e01e4dd3aa80cdf65b41072447cd02e375d3da249dcb`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ffa88e5eec5d45da757fb19b139ff9468309d797987ffc10120d9538947db2`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec1aab950c8691b268d3ee910c230ebe39a8c86cd15872a46d482d9d919987`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8735cfcf9ac1f26b597e58e0dc46c495468cb03cb7bef0c4400da5e8fdbd7cca`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70d0681d2078e2326a14831637f16c3b57fe8f03a55b3f90fc6fb689aba645`  
		Last Modified: Sun, 29 Dec 2019 01:57:23 GMT  
		Size: 66.3 MB (66332499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a47642cce4d2c51efea83292928b49c8938d7cfcc64b60d49387d9e5fa0466`  
		Last Modified: Sun, 29 Dec 2019 01:56:48 GMT  
		Size: 2.8 MB (2775897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424ab26a745ac3ea474c6f774ae98ac511d55c937d311dc3130b691647170065`  
		Last Modified: Sun, 29 Dec 2019 01:56:47 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdc270e7a25645ace70eb291be080460db20a6b91e979a3891aa0b8ebfc4fd8`  
		Last Modified: Sun, 29 Dec 2019 01:56:46 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb590edb4822037944e08e48ecfc21c928abb49b7ac0428ebe5a5efd6d946639`  
		Last Modified: Sun, 29 Dec 2019 01:56:46 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b797c353e22d07dd62f666bbb41f01d3b4008b2d631fabe5b428e818e4b70a`  
		Last Modified: Sun, 29 Dec 2019 01:57:18 GMT  
		Size: 38.4 MB (38403827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:a255a5fd8dbbb5d5c5a2e4779f636f7eb65cdb347fbcac310c9de5843ffe2cf2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272585730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:153f3fb344733f1c2e1d2a8513bfbaf29d328c5c85f441a7b86c1aeb7e19221b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 19:27:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 19:27:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 19:27:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 19:27:39 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 19:28:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 19:28:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 19:33:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:08 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 19:33:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 19:33:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 19:33:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 19:33:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:25 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 19:33:28 GMT
EXPOSE 80
# Sat, 28 Dec 2019 19:33:32 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:49:09 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:50:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:50:39 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 04:50:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:50:48 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:50:49 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Sun, 29 Dec 2019 04:50:51 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Sun, 29 Dec 2019 04:50:53 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Sun, 29 Dec 2019 04:50:54 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Sun, 29 Dec 2019 04:51:09 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed447e92ed09c9a464d9a1193550b84f1554bb96dd375ae2518965c4acc5e7`  
		Last Modified: Sat, 28 Dec 2019 20:19:48 GMT  
		Size: 12.6 MB (12647171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98bdd73f274ddf4d613631b79831e24954ed7bdcbc3001a970ab2673c90191`  
		Last Modified: Sat, 28 Dec 2019 20:19:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dea2440f3d8645d587221a106bb249affd61425e76cc2ddd5dde65e8557233`  
		Last Modified: Sat, 28 Dec 2019 20:19:49 GMT  
		Size: 14.9 MB (14882224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649bcaf54170c4cd63a99ed326d39a923216563f4f0721325378a7cdf34ce226`  
		Last Modified: Sat, 28 Dec 2019 20:19:43 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aef28adb9261ac35a69849d5571500918f8982cb367407b2fd2809608c0e6b5`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ad091ce1cb239b0012874b210006f7c03b53cdffa8ccb08111b869af2038fb`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d3bfe1ba07823cbf208809c693031e47cadbbc426392afd2b144b82a46b89`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7c4357ace9f66702187924dddaff72c659358a6ca5bbebcfbd28172af34a6`  
		Last Modified: Sun, 29 Dec 2019 04:53:26 GMT  
		Size: 71.2 MB (71194229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d489ec07beb31e3bc26690c954bc8d3947b0d7e100e4330fd1f3df46063eada2`  
		Last Modified: Sun, 29 Dec 2019 04:53:09 GMT  
		Size: 2.9 MB (2863120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70693b42d7923b4de1af7d1589cd7e90d85dd93a4a006c1ba1fd87743d8518bf`  
		Last Modified: Sun, 29 Dec 2019 04:53:08 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd69fc3ce7f2a3a104d20646b0de010935a9ad957b295341be2819810a6e86af`  
		Last Modified: Sun, 29 Dec 2019 04:53:08 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388010d812fdf9ae47b37b35ecde2ce0cdd9107a8f8bde03a9d44d4043a1a81f`  
		Last Modified: Sun, 29 Dec 2019 04:53:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bd27acebe654b560f4a52cf3c0aa0a4f48a9acbe6f625c4659cb89d9fe398b`  
		Last Modified: Sun, 29 Dec 2019 04:53:21 GMT  
		Size: 38.4 MB (38403931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:legacylts`

```console
$ docker pull mediawiki@sha256:278a7d86fe664da12a21711f79f4401e9235557819bc5d4ef52d24f8455b8b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:legacylts` - linux; amd64

```console
$ docker pull mediawiki@sha256:7a285ff0cb3d9a847790c653dfae7a2261d474a490c2c3bbde421c8c3dac6302
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251838718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db4ad228621f89c7f104fcb980cf662e52e302f8bde9fc52ee9231c9858d0263`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 22:06:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 22:06:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 22:06:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 22:10:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:56 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 22:10:56 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 22:10:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 22:10:57 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 22:10:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:57 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 22:10:57 GMT
EXPOSE 80
# Sat, 28 Dec 2019 22:10:58 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 11:00:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:58 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 11:01:59 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 11:02:00 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 11:02:07 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616effb632b1d9a229db46a4895f96ef822ed289120d5820f528d4e6d0196b04`  
		Last Modified: Sat, 28 Dec 2019 22:57:09 GMT  
		Size: 12.6 MB (12647459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20683410f309796015435a6c488b34d56f15a42751e53182ff36f9589a697aec`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39e604a3ca40968baa97b55862347eba6db9604fb7009f3b140a5b8a63a48f7`  
		Last Modified: Sat, 28 Dec 2019 22:57:11 GMT  
		Size: 13.8 MB (13840313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc05a4fae7428f9a56c576785244bc2c23c2cd11adec6c8d2a3e4446982b166`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e1a9337fe9acff76d7b3f49a9a55510ef7fa6af7ffa212294bf246d536d62`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1dfa87b2cec32d510224acaaa0ed06f71454e729937f1fb8c17d220fc5476`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b1c9144c1bfcaa8ce4f98f8f98a494041cce5252a5fb21132bb08f4a558e93`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb7894808376d3aa265e25e2dd498af7ded4951ad942b6579cb032969a17010`  
		Last Modified: Sun, 29 Dec 2019 11:02:49 GMT  
		Size: 64.4 MB (64382372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10650c299fdf015820f54960323b5705dce3208624414e83e10dda51b30d2b1d`  
		Last Modified: Sun, 29 Dec 2019 11:02:36 GMT  
		Size: 2.8 MB (2785348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a64e01650d7f7a990f91940bbfd797f1541260aff0abef13e3be9fe44aea78`  
		Last Modified: Sun, 29 Dec 2019 11:02:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa9e447661c47b37ea813400d2e10760cfcead04dc663add54ab05a39062be4`  
		Last Modified: Sun, 29 Dec 2019 11:02:54 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630b2092e36ecf8f916fb0f1c29cb172d732cdabd1586f9f7f9acfe560742b1`  
		Last Modified: Sun, 29 Dec 2019 11:03:03 GMT  
		Size: 35.8 MB (35757718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacylts` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:ef0bf6ae642cc2cba899051e324e6e51676eea40090ec0b3f8c8f6565aeb9304
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226409915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f411c12b250e4e3b6702aee343d48d59a7f6e47b6737edc97b8bd31d5cbd0f64`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:45:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Jan 2020 21:28:17 GMT
ENV PHP_VERSION=7.2.27
# Thu, 23 Jan 2020 21:28:18 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 21:28:19 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Thu, 23 Jan 2020 21:28:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 21:28:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 21:31:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 21:31:59 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 21:31:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 21:32:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 21:32:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:32:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 21:32:02 GMT
EXPOSE 80
# Thu, 23 Jan 2020 21:32:03 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:56:50 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:58:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:59:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:59:31 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:59:31 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 24 Jan 2020 00:59:32 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 24 Jan 2020 00:59:32 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Fri, 24 Jan 2020 00:59:33 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Fri, 24 Jan 2020 00:59:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2617be9432165f4ff50def4500ca5fcf541952391f0a5d4df67701bc394d2`  
		Last Modified: Thu, 23 Jan 2020 22:08:58 GMT  
		Size: 12.6 MB (12643254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8551c3f5356bf3cfa0a66e3855a0efe8066fe7e70afa47dff31910b97c986848`  
		Last Modified: Thu, 23 Jan 2020 22:08:46 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e729b7434145feec1c3d5e04f80e1c1e86d9e3e52bf329654c9e522b77de3e3b`  
		Last Modified: Thu, 23 Jan 2020 22:08:55 GMT  
		Size: 12.9 MB (12916666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b334636761919b50da4d1829bfaa0354494d1b74a4685041f786014c80cbf5`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3b4973e24f949da38cb81cd021c43453b3836f4745a762576934f89f0eedf4`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b9ab9698f568ba92711f2374a519a4b890fd3eada0b0094b4d69ab1e53891`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b083b324bc21fe14166b4df6df5698a848059740fab4c17079e43447727cc`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88798ca1063ce18ba0743649b0557aa3680d5d097f1ae254b83e3eafafc3c35`  
		Last Modified: Fri, 24 Jan 2020 01:01:57 GMT  
		Size: 60.7 MB (60727513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc48db92f8f0104e85ad6ea21e7710bd9a7011e5a6d84d7a1aee9190902329c`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 2.7 MB (2704392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fe0e9e4680176545f247126ad0874b5caa1fb9598ac33d4f5a19b6d236baf4`  
		Last Modified: Fri, 24 Jan 2020 01:02:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a5fd1a384f029c77fc234ced03fc82fe78dfae93c51a90cfa2ea26e1b3d362`  
		Last Modified: Fri, 24 Jan 2020 01:02:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eef34bca5469eb41f587ac2208ac25134c6030dbe0ece02ecb20f66967db849`  
		Last Modified: Fri, 24 Jan 2020 01:02:52 GMT  
		Size: 35.8 MB (35758727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacylts` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:902cdc9160421f7b67b42c5be34c59301ae0b40bac222f4a7036eb227b0c592f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.9 MB (219940488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cdf48b416a0015037cfeb85136efa5366b8820d4c57c4124ebec232ebe2c3a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:39:38 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 16:39:39 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 16:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:39:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:42:54 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:59 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:43:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:43:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:43:06 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:43:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:43:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:43:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:43:12 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:09:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:11:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:12:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:12:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:12:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 05:12:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 05:12:13 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 05:12:14 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 05:12:31 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3334f18cf3c9b09c2bb03110d24b806ceed4445b5da5e355e03e723c2b1614`  
		Last Modified: Sat, 28 Dec 2019 17:15:13 GMT  
		Size: 12.6 MB (12645461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eae1e83fddba25d3172b588bce688c3a310608a4bfe25de808e0eb566a04ebf`  
		Last Modified: Sat, 28 Dec 2019 17:15:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fbe17d996b2504cdc42ee40f7d649eca4aaa5be19429a4e539b3329ceb2148`  
		Last Modified: Sat, 28 Dec 2019 17:15:17 GMT  
		Size: 12.2 MB (12186080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2220d9961faeb5bedaefe8a20906c5f3c4539d6f03db8fb786855229732a4c`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc727f308c74cad30c947c8f15188cd2421c2acc731fe9c241b40c6feb1d00`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b81aa860ae65f310e7d52b99ebbd6e7444918b85929de2baa85b188c3863bdb`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128b3062692808ff44cfdd5411ee2739d2edda2e2dcd26883380e709464a2c4d`  
		Last Modified: Sat, 28 Dec 2019 17:15:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0deac41ba566db06f7dc310d07c83a525c13c2e98ea39414561b700d4ce4a66`  
		Last Modified: Sun, 29 Dec 2019 05:13:44 GMT  
		Size: 57.0 MB (57012633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8b99ec8846b071347e924fa2af35fa376c29870cb54fbd15d2a78ca96dd5df`  
		Last Modified: Sun, 29 Dec 2019 05:13:27 GMT  
		Size: 2.6 MB (2649286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c685626d5598b1e85347ad70b3993ba7cacb66f55f75a24ece771374630566`  
		Last Modified: Sun, 29 Dec 2019 05:13:56 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c353924db4c4df5a6902974ed493d1fbc76a399e2136bae23e262b83d17288a`  
		Last Modified: Sun, 29 Dec 2019 05:13:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977796e01e72d35f2a9eb6ca1a2d3ff55cb3908220f961b7ad2e7c94b8f8249a`  
		Last Modified: Sun, 29 Dec 2019 05:14:14 GMT  
		Size: 35.8 MB (35758447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacylts` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:8c85b7c7625e41de58299cdf2769a58db7dc942f1e73123f4186ab55c7500fca
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241651986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc428c097ace6e52051d6c653b9b13c9722609ca10ff30f732502eebb3f3622`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 15:33:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 15:33:35 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 15:33:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 15:33:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:37:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:13 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:37:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:37:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:37:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:37:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:21 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:37:22 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:37:23 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:23:20 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:26:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:26:09 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:26:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 06:26:17 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 06:26:19 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 06:26:21 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 06:26:38 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef55e879c10bb0bfe58b0e87d612c419ea5bd7503872b20b4f204c4ff29fc529`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 12.6 MB (12646118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f6952b67823bbc1f9d02a4c84126ee319f7453c8b50ba5c15d230f582a24cb`  
		Last Modified: Sat, 28 Dec 2019 16:12:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1409df52b683c197e2f155c5fff7655f3685cba677ed3cd88500b5c50a0b322e`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 13.5 MB (13537744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a0571861c31f3e3e66ef375bed45e5baf9b06264b2c21f16c281c14a6e425a`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5f5ab5fff422d4c5851f79af8e8bcd99629a1d824101f26afe878f49641733`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd643e176f0541609f1cc882c4c2bf40a168ea1a2774bbba5dddea14492e4c14`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266f7b1f11a53b6b15316c0eefecf0d4b8647f2672c42d0b8a7f745bb9939ae3`  
		Last Modified: Sat, 28 Dec 2019 16:12:19 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293f6ae45064ffc9bead71caf085d167b46041ea02c548d0a5051becaf93b138`  
		Last Modified: Sun, 29 Dec 2019 06:27:48 GMT  
		Size: 62.2 MB (62181447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4189a9c54e310f0ed59abeeb288b039c62fbea382ad7b6d2fa91460e2d444d95`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 2.8 MB (2758645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4e636ddcf984e5af604a377da8959f89ef3ebbf5e3f750d2e2720fa3e7fc4d`  
		Last Modified: Sun, 29 Dec 2019 06:27:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3672476e195cbe2f6a8e973fccb19d0ea4613bc6516b73bd2d85c598c659099`  
		Last Modified: Sun, 29 Dec 2019 06:27:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb9b160cbe9a80bf9b013df22a8204bdce4024a6e235bbc549a65b32249516c`  
		Last Modified: Sun, 29 Dec 2019 06:28:15 GMT  
		Size: 35.8 MB (35758354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacylts` - linux; 386

```console
$ docker pull mediawiki@sha256:6fbf0ace16a8122ea07b7f118f488890f81ffcbbe745196d8bad530354c9f3cf
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.7 MB (259742492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f4ef9d2378f4b8e23256d6601c7abb1673361047d70c77f15ac01be6db2c24`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:36:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 18:36:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:36:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:41:53 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:41:54 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:41:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:41:55 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:41:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:55 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:41:55 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:41:55 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:52:44 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:54:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:55:17 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:55:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 01:55:37 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7cf80bc7d8085b8ce0a31e3a98f5693961c49434a02d4140d3c71a07ca565`  
		Last Modified: Sat, 28 Dec 2019 19:37:07 GMT  
		Size: 12.6 MB (12646713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a2cb9f569f09db2f619aa046f4b6508bf2a6734586800e94606e2cd6d4c56d`  
		Last Modified: Sat, 28 Dec 2019 19:37:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59eac3b46370851360f3dd6921cd777da75f7e064a3f2b86bca60969d4f11e3`  
		Last Modified: Sat, 28 Dec 2019 19:37:11 GMT  
		Size: 14.2 MB (14165526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365a0af4c7ee6ef2bf0e01e4dd3aa80cdf65b41072447cd02e375d3da249dcb`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ffa88e5eec5d45da757fb19b139ff9468309d797987ffc10120d9538947db2`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec1aab950c8691b268d3ee910c230ebe39a8c86cd15872a46d482d9d919987`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8735cfcf9ac1f26b597e58e0dc46c495468cb03cb7bef0c4400da5e8fdbd7cca`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70d0681d2078e2326a14831637f16c3b57fe8f03a55b3f90fc6fb689aba645`  
		Last Modified: Sun, 29 Dec 2019 01:57:23 GMT  
		Size: 66.3 MB (66332499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a47642cce4d2c51efea83292928b49c8938d7cfcc64b60d49387d9e5fa0466`  
		Last Modified: Sun, 29 Dec 2019 01:56:48 GMT  
		Size: 2.8 MB (2775897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8aea51ae0228a216cb72d951e5c80aaa98a02d29c5d2217f7bdcaa95b1bbf65`  
		Last Modified: Sun, 29 Dec 2019 01:57:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59100766a49da5cc2fae5f62cdc492305df96a29f1b4fc106424ceb4aa643c17`  
		Last Modified: Sun, 29 Dec 2019 01:57:30 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3182a6bb97203a909bd4acfd36db720708ca6dd5392407da551710e4b2faf874`  
		Last Modified: Sun, 29 Dec 2019 01:57:50 GMT  
		Size: 35.8 MB (35757566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacylts` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:aa640970accbfb523f7db66d932a3b49a49b59dd5736a3c37bd75778990e1a98
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.9 MB (269939370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a94f92cfe74abdaeaef6b273e3ea467fefaf086f07e2af64297280d00380ad`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 19:27:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 19:27:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 19:27:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 19:27:39 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 19:28:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 19:28:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 19:33:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:08 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 19:33:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 19:33:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 19:33:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 19:33:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:25 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 19:33:28 GMT
EXPOSE 80
# Sat, 28 Dec 2019 19:33:32 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:49:09 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:50:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:51:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:51:33 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:51:36 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 04:51:39 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 04:51:41 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 04:51:45 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 04:52:05 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed447e92ed09c9a464d9a1193550b84f1554bb96dd375ae2518965c4acc5e7`  
		Last Modified: Sat, 28 Dec 2019 20:19:48 GMT  
		Size: 12.6 MB (12647171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98bdd73f274ddf4d613631b79831e24954ed7bdcbc3001a970ab2673c90191`  
		Last Modified: Sat, 28 Dec 2019 20:19:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dea2440f3d8645d587221a106bb249affd61425e76cc2ddd5dde65e8557233`  
		Last Modified: Sat, 28 Dec 2019 20:19:49 GMT  
		Size: 14.9 MB (14882224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649bcaf54170c4cd63a99ed326d39a923216563f4f0721325378a7cdf34ce226`  
		Last Modified: Sat, 28 Dec 2019 20:19:43 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aef28adb9261ac35a69849d5571500918f8982cb367407b2fd2809608c0e6b5`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ad091ce1cb239b0012874b210006f7c03b53cdffa8ccb08111b869af2038fb`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d3bfe1ba07823cbf208809c693031e47cadbbc426392afd2b144b82a46b89`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7c4357ace9f66702187924dddaff72c659358a6ca5bbebcfbd28172af34a6`  
		Last Modified: Sun, 29 Dec 2019 04:53:26 GMT  
		Size: 71.2 MB (71194229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d489ec07beb31e3bc26690c954bc8d3947b0d7e100e4330fd1f3df46063eada2`  
		Last Modified: Sun, 29 Dec 2019 04:53:09 GMT  
		Size: 2.9 MB (2863120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1d639a84d6660d51844ed94e20719d38a828e7541d14a2b734d751cf4dc867`  
		Last Modified: Sun, 29 Dec 2019 04:53:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f88e7849100e1cac1ac29e8cfd1c50a0f59f93ecba9a3a503cbc8acaeca03`  
		Last Modified: Sun, 29 Dec 2019 04:53:42 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8da8586fd0df698a9020506552f9e12c7e7f66dc625bfaa25294a99a24d1b77`  
		Last Modified: Sun, 29 Dec 2019 04:53:52 GMT  
		Size: 35.8 MB (35758158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:lts`

```console
$ docker pull mediawiki@sha256:278a7d86fe664da12a21711f79f4401e9235557819bc5d4ef52d24f8455b8b34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:lts` - linux; amd64

```console
$ docker pull mediawiki@sha256:7a285ff0cb3d9a847790c653dfae7a2261d474a490c2c3bbde421c8c3dac6302
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.8 MB (251838718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db4ad228621f89c7f104fcb980cf662e52e302f8bde9fc52ee9231c9858d0263`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 22:06:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 22:06:19 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 22:06:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 22:06:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 22:10:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:56 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 22:10:56 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 22:10:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 22:10:57 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 22:10:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 22:10:57 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 22:10:57 GMT
EXPOSE 80
# Sat, 28 Dec 2019 22:10:58 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 11:00:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 11:01:58 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 11:01:59 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 11:01:59 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 11:02:00 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 11:02:07 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616effb632b1d9a229db46a4895f96ef822ed289120d5820f528d4e6d0196b04`  
		Last Modified: Sat, 28 Dec 2019 22:57:09 GMT  
		Size: 12.6 MB (12647459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20683410f309796015435a6c488b34d56f15a42751e53182ff36f9589a697aec`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39e604a3ca40968baa97b55862347eba6db9604fb7009f3b140a5b8a63a48f7`  
		Last Modified: Sat, 28 Dec 2019 22:57:11 GMT  
		Size: 13.8 MB (13840313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc05a4fae7428f9a56c576785244bc2c23c2cd11adec6c8d2a3e4446982b166`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341e1a9337fe9acff76d7b3f49a9a55510ef7fa6af7ffa212294bf246d536d62`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1dfa87b2cec32d510224acaaa0ed06f71454e729937f1fb8c17d220fc5476`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b1c9144c1bfcaa8ce4f98f8f98a494041cce5252a5fb21132bb08f4a558e93`  
		Last Modified: Sat, 28 Dec 2019 22:57:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb7894808376d3aa265e25e2dd498af7ded4951ad942b6579cb032969a17010`  
		Last Modified: Sun, 29 Dec 2019 11:02:49 GMT  
		Size: 64.4 MB (64382372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10650c299fdf015820f54960323b5705dce3208624414e83e10dda51b30d2b1d`  
		Last Modified: Sun, 29 Dec 2019 11:02:36 GMT  
		Size: 2.8 MB (2785348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a64e01650d7f7a990f91940bbfd797f1541260aff0abef13e3be9fe44aea78`  
		Last Modified: Sun, 29 Dec 2019 11:02:54 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa9e447661c47b37ea813400d2e10760cfcead04dc663add54ab05a39062be4`  
		Last Modified: Sun, 29 Dec 2019 11:02:54 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630b2092e36ecf8f916fb0f1c29cb172d732cdabd1586f9f7f9acfe560742b1`  
		Last Modified: Sun, 29 Dec 2019 11:03:03 GMT  
		Size: 35.8 MB (35757718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:ef0bf6ae642cc2cba899051e324e6e51676eea40090ec0b3f8c8f6565aeb9304
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226409915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f411c12b250e4e3b6702aee343d48d59a7f6e47b6737edc97b8bd31d5cbd0f64`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:45:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Jan 2020 21:28:17 GMT
ENV PHP_VERSION=7.2.27
# Thu, 23 Jan 2020 21:28:18 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 21:28:19 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Thu, 23 Jan 2020 21:28:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 21:28:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 21:31:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:31:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 21:31:59 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 21:31:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 21:32:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 21:32:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:32:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 21:32:02 GMT
EXPOSE 80
# Thu, 23 Jan 2020 21:32:03 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:56:50 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:58:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:59:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:59:31 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:59:31 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 24 Jan 2020 00:59:32 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 24 Jan 2020 00:59:32 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Fri, 24 Jan 2020 00:59:33 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Fri, 24 Jan 2020 00:59:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2617be9432165f4ff50def4500ca5fcf541952391f0a5d4df67701bc394d2`  
		Last Modified: Thu, 23 Jan 2020 22:08:58 GMT  
		Size: 12.6 MB (12643254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8551c3f5356bf3cfa0a66e3855a0efe8066fe7e70afa47dff31910b97c986848`  
		Last Modified: Thu, 23 Jan 2020 22:08:46 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e729b7434145feec1c3d5e04f80e1c1e86d9e3e52bf329654c9e522b77de3e3b`  
		Last Modified: Thu, 23 Jan 2020 22:08:55 GMT  
		Size: 12.9 MB (12916666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23b334636761919b50da4d1829bfaa0354494d1b74a4685041f786014c80cbf5`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3b4973e24f949da38cb81cd021c43453b3836f4745a762576934f89f0eedf4`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07b9ab9698f568ba92711f2374a519a4b890fd3eada0b0094b4d69ab1e53891`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3b083b324bc21fe14166b4df6df5698a848059740fab4c17079e43447727cc`  
		Last Modified: Thu, 23 Jan 2020 22:08:45 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88798ca1063ce18ba0743649b0557aa3680d5d097f1ae254b83e3eafafc3c35`  
		Last Modified: Fri, 24 Jan 2020 01:01:57 GMT  
		Size: 60.7 MB (60727513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc48db92f8f0104e85ad6ea21e7710bd9a7011e5a6d84d7a1aee9190902329c`  
		Last Modified: Fri, 24 Jan 2020 01:01:18 GMT  
		Size: 2.7 MB (2704392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fe0e9e4680176545f247126ad0874b5caa1fb9598ac33d4f5a19b6d236baf4`  
		Last Modified: Fri, 24 Jan 2020 01:02:07 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a5fd1a384f029c77fc234ced03fc82fe78dfae93c51a90cfa2ea26e1b3d362`  
		Last Modified: Fri, 24 Jan 2020 01:02:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eef34bca5469eb41f587ac2208ac25134c6030dbe0ece02ecb20f66967db849`  
		Last Modified: Fri, 24 Jan 2020 01:02:52 GMT  
		Size: 35.8 MB (35758727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:902cdc9160421f7b67b42c5be34c59301ae0b40bac222f4a7036eb227b0c592f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.9 MB (219940488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91cdf48b416a0015037cfeb85136efa5366b8820d4c57c4124ebec232ebe2c3a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:39:38 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 16:39:39 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:39:40 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 16:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:39:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:42:54 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:42:59 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:43:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:43:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:43:06 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:43:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:43:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:43:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:43:12 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:09:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:11:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:12:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:12:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:12:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 05:12:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 05:12:13 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 05:12:14 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 05:12:31 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3334f18cf3c9b09c2bb03110d24b806ceed4445b5da5e355e03e723c2b1614`  
		Last Modified: Sat, 28 Dec 2019 17:15:13 GMT  
		Size: 12.6 MB (12645461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eae1e83fddba25d3172b588bce688c3a310608a4bfe25de808e0eb566a04ebf`  
		Last Modified: Sat, 28 Dec 2019 17:15:12 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fbe17d996b2504cdc42ee40f7d649eca4aaa5be19429a4e539b3329ceb2148`  
		Last Modified: Sat, 28 Dec 2019 17:15:17 GMT  
		Size: 12.2 MB (12186080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2220d9961faeb5bedaefe8a20906c5f3c4539d6f03db8fb786855229732a4c`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4dc727f308c74cad30c947c8f15188cd2421c2acc731fe9c241b40c6feb1d00`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b81aa860ae65f310e7d52b99ebbd6e7444918b85929de2baa85b188c3863bdb`  
		Last Modified: Sat, 28 Dec 2019 17:15:10 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128b3062692808ff44cfdd5411ee2739d2edda2e2dcd26883380e709464a2c4d`  
		Last Modified: Sat, 28 Dec 2019 17:15:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0deac41ba566db06f7dc310d07c83a525c13c2e98ea39414561b700d4ce4a66`  
		Last Modified: Sun, 29 Dec 2019 05:13:44 GMT  
		Size: 57.0 MB (57012633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8b99ec8846b071347e924fa2af35fa376c29870cb54fbd15d2a78ca96dd5df`  
		Last Modified: Sun, 29 Dec 2019 05:13:27 GMT  
		Size: 2.6 MB (2649286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c685626d5598b1e85347ad70b3993ba7cacb66f55f75a24ece771374630566`  
		Last Modified: Sun, 29 Dec 2019 05:13:56 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c353924db4c4df5a6902974ed493d1fbc76a399e2136bae23e262b83d17288a`  
		Last Modified: Sun, 29 Dec 2019 05:13:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977796e01e72d35f2a9eb6ca1a2d3ff55cb3908220f961b7ad2e7c94b8f8249a`  
		Last Modified: Sun, 29 Dec 2019 05:14:14 GMT  
		Size: 35.8 MB (35758447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:8c85b7c7625e41de58299cdf2769a58db7dc942f1e73123f4186ab55c7500fca
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241651986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc428c097ace6e52051d6c653b9b13c9722609ca10ff30f732502eebb3f3622`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 15:33:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 15:33:35 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 15:33:36 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 15:33:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 15:33:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:37:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:13 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:37:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:37:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:37:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:37:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:37:21 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:37:22 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:37:23 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:23:20 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:25:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:26:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:26:09 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:26:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 06:26:17 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 06:26:19 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 06:26:21 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 06:26:38 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef55e879c10bb0bfe58b0e87d612c419ea5bd7503872b20b4f204c4ff29fc529`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 12.6 MB (12646118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f6952b67823bbc1f9d02a4c84126ee319f7453c8b50ba5c15d230f582a24cb`  
		Last Modified: Sat, 28 Dec 2019 16:12:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1409df52b683c197e2f155c5fff7655f3685cba677ed3cd88500b5c50a0b322e`  
		Last Modified: Sat, 28 Dec 2019 16:12:24 GMT  
		Size: 13.5 MB (13537744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a0571861c31f3e3e66ef375bed45e5baf9b06264b2c21f16c281c14a6e425a`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5f5ab5fff422d4c5851f79af8e8bcd99629a1d824101f26afe878f49641733`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd643e176f0541609f1cc882c4c2bf40a168ea1a2774bbba5dddea14492e4c14`  
		Last Modified: Sat, 28 Dec 2019 16:12:18 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266f7b1f11a53b6b15316c0eefecf0d4b8647f2672c42d0b8a7f745bb9939ae3`  
		Last Modified: Sat, 28 Dec 2019 16:12:19 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293f6ae45064ffc9bead71caf085d167b46041ea02c548d0a5051becaf93b138`  
		Last Modified: Sun, 29 Dec 2019 06:27:48 GMT  
		Size: 62.2 MB (62181447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4189a9c54e310f0ed59abeeb288b039c62fbea382ad7b6d2fa91460e2d444d95`  
		Last Modified: Sun, 29 Dec 2019 06:27:31 GMT  
		Size: 2.8 MB (2758645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4e636ddcf984e5af604a377da8959f89ef3ebbf5e3f750d2e2720fa3e7fc4d`  
		Last Modified: Sun, 29 Dec 2019 06:27:59 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3672476e195cbe2f6a8e973fccb19d0ea4613bc6516b73bd2d85c598c659099`  
		Last Modified: Sun, 29 Dec 2019 06:27:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb9b160cbe9a80bf9b013df22a8204bdce4024a6e235bbc549a65b32249516c`  
		Last Modified: Sun, 29 Dec 2019 06:28:15 GMT  
		Size: 35.8 MB (35758354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; 386

```console
$ docker pull mediawiki@sha256:6fbf0ace16a8122ea07b7f118f488890f81ffcbbe745196d8bad530354c9f3cf
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.7 MB (259742492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02f4ef9d2378f4b8e23256d6601c7abb1673361047d70c77f15ac01be6db2c24`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:36:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:36:31 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 18:36:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:36:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:41:53 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:41:54 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:41:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:41:55 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:41:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:41:55 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:41:55 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:41:55 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:52:44 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:54:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:55:17 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:55:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 01:55:19 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 01:55:37 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f7cf80bc7d8085b8ce0a31e3a98f5693961c49434a02d4140d3c71a07ca565`  
		Last Modified: Sat, 28 Dec 2019 19:37:07 GMT  
		Size: 12.6 MB (12646713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a2cb9f569f09db2f619aa046f4b6508bf2a6734586800e94606e2cd6d4c56d`  
		Last Modified: Sat, 28 Dec 2019 19:37:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59eac3b46370851360f3dd6921cd777da75f7e064a3f2b86bca60969d4f11e3`  
		Last Modified: Sat, 28 Dec 2019 19:37:11 GMT  
		Size: 14.2 MB (14165526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365a0af4c7ee6ef2bf0e01e4dd3aa80cdf65b41072447cd02e375d3da249dcb`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ffa88e5eec5d45da757fb19b139ff9468309d797987ffc10120d9538947db2`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ec1aab950c8691b268d3ee910c230ebe39a8c86cd15872a46d482d9d919987`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8735cfcf9ac1f26b597e58e0dc46c495468cb03cb7bef0c4400da5e8fdbd7cca`  
		Last Modified: Sat, 28 Dec 2019 19:37:04 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae70d0681d2078e2326a14831637f16c3b57fe8f03a55b3f90fc6fb689aba645`  
		Last Modified: Sun, 29 Dec 2019 01:57:23 GMT  
		Size: 66.3 MB (66332499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a47642cce4d2c51efea83292928b49c8938d7cfcc64b60d49387d9e5fa0466`  
		Last Modified: Sun, 29 Dec 2019 01:56:48 GMT  
		Size: 2.8 MB (2775897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8aea51ae0228a216cb72d951e5c80aaa98a02d29c5d2217f7bdcaa95b1bbf65`  
		Last Modified: Sun, 29 Dec 2019 01:57:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59100766a49da5cc2fae5f62cdc492305df96a29f1b4fc106424ceb4aa643c17`  
		Last Modified: Sun, 29 Dec 2019 01:57:30 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3182a6bb97203a909bd4acfd36db720708ca6dd5392407da551710e4b2faf874`  
		Last Modified: Sun, 29 Dec 2019 01:57:50 GMT  
		Size: 35.8 MB (35757566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:aa640970accbfb523f7db66d932a3b49a49b59dd5736a3c37bd75778990e1a98
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.9 MB (269939370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a94f92cfe74abdaeaef6b273e3ea467fefaf086f07e2af64297280d00380ad`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 19:27:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 28 Dec 2019 19:27:31 GMT
ENV PHP_VERSION=7.2.26
# Sat, 28 Dec 2019 19:27:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.26.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.26.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 19:27:39 GMT
ENV PHP_SHA256=1dd3bc875e105f5c9d21fb4dc240670bd2c22037820ff03890f5ab883c88b78d PHP_MD5=
# Sat, 28 Dec 2019 19:28:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 19:28:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 19:33:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:08 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 19:33:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 19:33:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 19:33:19 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 19:33:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 19:33:25 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 19:33:28 GMT
EXPOSE 80
# Sat, 28 Dec 2019 19:33:32 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:49:09 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:50:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:51:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:51:33 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:51:36 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Sun, 29 Dec 2019 04:51:39 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Sun, 29 Dec 2019 04:51:41 GMT
ENV MEDIAWIKI_VERSION=1.31.6
# Sun, 29 Dec 2019 04:51:45 GMT
ENV MEDIAWIKI_SHA512=4c6431edc591357f30cba1174825540efd721dccd365d704a704cb1ad03ce6541074074a37f6cb9f30ec8289e00a768ab3592c4b8e74f67ae828a0bb8669baab
# Sun, 29 Dec 2019 04:52:05 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bed447e92ed09c9a464d9a1193550b84f1554bb96dd375ae2518965c4acc5e7`  
		Last Modified: Sat, 28 Dec 2019 20:19:48 GMT  
		Size: 12.6 MB (12647171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98bdd73f274ddf4d613631b79831e24954ed7bdcbc3001a970ab2673c90191`  
		Last Modified: Sat, 28 Dec 2019 20:19:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dea2440f3d8645d587221a106bb249affd61425e76cc2ddd5dde65e8557233`  
		Last Modified: Sat, 28 Dec 2019 20:19:49 GMT  
		Size: 14.9 MB (14882224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649bcaf54170c4cd63a99ed326d39a923216563f4f0721325378a7cdf34ce226`  
		Last Modified: Sat, 28 Dec 2019 20:19:43 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aef28adb9261ac35a69849d5571500918f8982cb367407b2fd2809608c0e6b5`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ad091ce1cb239b0012874b210006f7c03b53cdffa8ccb08111b869af2038fb`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546d3bfe1ba07823cbf208809c693031e47cadbbc426392afd2b144b82a46b89`  
		Last Modified: Sat, 28 Dec 2019 20:19:42 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe7c4357ace9f66702187924dddaff72c659358a6ca5bbebcfbd28172af34a6`  
		Last Modified: Sun, 29 Dec 2019 04:53:26 GMT  
		Size: 71.2 MB (71194229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d489ec07beb31e3bc26690c954bc8d3947b0d7e100e4330fd1f3df46063eada2`  
		Last Modified: Sun, 29 Dec 2019 04:53:09 GMT  
		Size: 2.9 MB (2863120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1d639a84d6660d51844ed94e20719d38a828e7541d14a2b734d751cf4dc867`  
		Last Modified: Sun, 29 Dec 2019 04:53:41 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f88e7849100e1cac1ac29e8cfd1c50a0f59f93ecba9a3a503cbc8acaeca03`  
		Last Modified: Sun, 29 Dec 2019 04:53:42 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8da8586fd0df698a9020506552f9e12c7e7f66dc625bfaa25294a99a24d1b77`  
		Last Modified: Sun, 29 Dec 2019 04:53:52 GMT  
		Size: 35.8 MB (35758158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:stable`

```console
$ docker pull mediawiki@sha256:79b7ca659bb4b514ce4a2df205bea76d8cd9e29ab5636735a3531c514c2478d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:stable` - linux; amd64

```console
$ docker pull mediawiki@sha256:fa2e7a9e8eeb91fbb6e39cc2c8846a111aa6efe8876a08ba4bab155ca63da1b9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.1 MB (257115331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f7db6799cb077e044fe43ac250c57c391c666f26c7bbf8b3c698e318ea7ce15`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 20:39:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 20:39:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 20:40:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 20:40:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 20:40:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 20:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 20:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 20:46:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 20:46:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 20:46:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 20:46:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 21:12:38 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 21:12:38 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 21:12:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 21:12:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 21:17:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:03 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 21:17:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 21:17:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 21:17:04 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 21:17:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 21:17:05 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 21:17:05 GMT
EXPOSE 80
# Sat, 28 Dec 2019 21:17:05 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 10:58:27 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 10:59:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 10:59:41 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 10:59:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 10:59:43 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 10:59:43 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 10:59:52 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf4fc8647872d4db40c6957c1a7cfefd3bcb785281f88762706926c307c56c`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970dadf4ccb644b7e193c317c67e6002c9b1386a99e062c2d67dd089625c64ec`  
		Last Modified: Sat, 28 Dec 2019 22:53:59 GMT  
		Size: 76.7 MB (76651636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c04561117a4645551bc4379b1eebdc32e178a61d11c5db8d79f2658178f6639`  
		Last Modified: Sat, 28 Dec 2019 22:53:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b7434b63a246cff24e7a3d2310de1b31f04f89af889acda1a1aabb53c299c5`  
		Last Modified: Sat, 28 Dec 2019 22:54:19 GMT  
		Size: 18.7 MB (18675679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d8859e9744116aa6e790b787a05a0ec71230f107ecd511b7fd2f299ca91e55`  
		Last Modified: Sat, 28 Dec 2019 22:54:15 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3d824d0ad5a0258fd7214a6e3faef915791d37af27b7afe0e59ba28c86f884`  
		Last Modified: Sat, 28 Dec 2019 22:54:14 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e316fd5b3b31a7c6ac4320517a41f6bbb3eb02f527cfc8fae23ca0dc68ffebd`  
		Last Modified: Sat, 28 Dec 2019 22:55:15 GMT  
		Size: 12.4 MB (12440404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578b40496c371640b6bb2c25d655d386b471ca78f820f28dcbb500506430c489`  
		Last Modified: Sat, 28 Dec 2019 22:55:13 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814ae7711d3c4266c8bffe679dd7ce200e879a32943f9b5c760806fed9877627`  
		Last Modified: Sat, 28 Dec 2019 22:55:18 GMT  
		Size: 14.1 MB (14078040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4896fed78b6b0c6ece3825c30fa479aad229a8e7cfcea2236e42207167310e20`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74d71e9611db3c5ae3e77251f4091fbde1cc7d62fdaf0e05321eb618acb1081`  
		Last Modified: Sat, 28 Dec 2019 22:55:13 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46017765526c6535682249b21a12ab2f2b85da2047896a62c0874e068682c867`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28038609845819461b2f18a28f6d89b977b43ee6c7c33ec6c8d833739b20503e`  
		Last Modified: Sat, 28 Dec 2019 22:55:12 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4c6dc86636371d2f17622db1191fa4a2e3db0a19a0e546bb1b6fe958acab10`  
		Last Modified: Sun, 29 Dec 2019 11:02:29 GMT  
		Size: 64.4 MB (64382208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78773447511cfd68c3fca6dcbec102b4be71e21e87aeb7d3478fde32e151c136`  
		Last Modified: Sun, 29 Dec 2019 11:02:16 GMT  
		Size: 2.9 MB (2856667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbb5f3759c20331020223e292ad0037973aeeea83337fcd9d78c978baf8f654`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c28e9635c157094f7faec7c7303005ea7e4004d716060598f8994bec784101`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5b1ac8187703f0cd091b241689517343104c6fd3691120f7432f4fb7817ab8`  
		Last Modified: Sun, 29 Dec 2019 11:02:15 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9be11e3e301dc81628d2df0396841a8873a4e36e92f48adde51a182450c3bb3`  
		Last Modified: Sun, 29 Dec 2019 11:02:27 GMT  
		Size: 40.9 MB (40931929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:2a59cf5694724bdc3104e9e9a83f4d324bacc9dda1983e01d8209f16f11a55b4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.6 MB (231632999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1bd487ee3bdb02521edabdbaf4507312a5c154e8c208254b9213103d6ffcddc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:46:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 11:46:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 11:46:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:46:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 11:46:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 11:51:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 11:52:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 11:52:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 11:52:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 11:52:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 11:52:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 11:52:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 12:09:24 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 23 Jan 2020 20:52:31 GMT
ENV PHP_VERSION=7.3.14
# Thu, 23 Jan 2020 20:52:32 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.14.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.14.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 20:52:32 GMT
ENV PHP_SHA256=cc05dd373ca5d36652800762f65c10e828a17de35aaf246262e3efa99d00cdb0 PHP_MD5=
# Thu, 23 Jan 2020 20:52:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 20:52:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 20:56:08 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:10 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 20:56:12 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 20:56:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 20:56:14 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 20:56:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 20:56:15 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 20:56:15 GMT
EXPOSE 80
# Thu, 23 Jan 2020 20:56:16 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 00:52:57 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:54:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 00:54:48 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 00:54:50 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 00:54:52 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 00:54:53 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 24 Jan 2020 00:54:53 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 24 Jan 2020 00:54:54 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Fri, 24 Jan 2020 00:54:55 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Fri, 24 Jan 2020 00:55:14 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb31ffad3b14d29eb4441c87b0f3a709311362013f6cb7af3b9a08356e3f54b`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c480440b3d2ffec23c2715bc1a23b63727a2cd4ec16dba2a4b8092960d29408`  
		Last Modified: Sat, 28 Dec 2019 13:15:33 GMT  
		Size: 58.8 MB (58799289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0b6d7351fa8842e4f35ee4f387772cef51f2b0371e8426fc5fda008f66f6c1`  
		Last Modified: Sat, 28 Dec 2019 13:15:11 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da5e5fa374e831ba6fecd4fd0f4cb996d6f225cfdb539ca67b782016c3d6e97`  
		Last Modified: Sat, 28 Dec 2019 13:16:06 GMT  
		Size: 18.0 MB (18024381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82722248cd3cc009d44e401aae5b794d5f29a6dd09448f81b669b2177f10eb52`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb194a191156ae4e4b8f5be5ffd2b156ccea22cec6c79ead9b26d6a78ce698f`  
		Last Modified: Sat, 28 Dec 2019 13:16:00 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cfdf0470bce0679253384cf02f9f1b896fb4665bedb65be5023e0e950e7a3b`  
		Last Modified: Thu, 23 Jan 2020 22:04:53 GMT  
		Size: 12.4 MB (12442341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f9507d43050ba009b8afb20570d27bad84ee2e000949f7a885fdb0ef4f1557`  
		Last Modified: Thu, 23 Jan 2020 22:04:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412c7b752a5d961cf2d2ec06b55c62dcbb7efdd5e5f55dec745c459b5ebb4ffb`  
		Last Modified: Thu, 23 Jan 2020 22:04:40 GMT  
		Size: 13.1 MB (13096070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791346c7fb72630bee2dfd762c43e4852e134ac1da979744fd67ed0aaf6a6b03`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c80400256513da81e6a7768c42565cbc9f674c778d2bd0b3b7e51153ac63cf`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46ccc7504b358e47f682a6f4a2c3e04eb75e9d4755563239f063ee7237f47da`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd1668a5072f1159e7d273194180e9d2c696372e381f8ed31b977ecf210c8d8`  
		Last Modified: Thu, 23 Jan 2020 22:04:37 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef4e257e74e23370b32c8129e66472fee2b920888c673eec95f0f0bb8dfb392`  
		Last Modified: Fri, 24 Jan 2020 01:01:02 GMT  
		Size: 60.7 MB (60728020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f60803715dcb5429ed46dd9c5323a5bf8a61ad55a3dc275e1f69b91fd5c67084`  
		Last Modified: Fri, 24 Jan 2020 01:00:21 GMT  
		Size: 2.8 MB (2773953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1b3320ab21de757eb540ea6ae9c72e9c8edd27ce1ffb99a6e3566f3a31ecd6`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0badbebef8582d532b9e59061158039e5992e6ffe99d6bcb984ead050942b2e9`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7510e9105626e90e19a149010b107192574f107d91ffa836bcdbfbad33b6a6`  
		Last Modified: Fri, 24 Jan 2020 01:00:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c694bee0d570fb407c748485c00be541e026fb9680005fa5dbc0a7eec5e6f`  
		Last Modified: Fri, 24 Jan 2020 01:00:58 GMT  
		Size: 40.9 MB (40932676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:bb2cde30cfb77bbefc0747a44414af3d4ccd4dbc9f6c27a3589510e08c6f8bdd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225173738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989fa8539446c99e6a7bb303e7248decb122e4a4641aa0b237e0442d24ecd36f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:41:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 15:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 15:42:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:42:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 15:42:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 15:46:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 15:46:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 15:47:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 15:47:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 15:47:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 15:47:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 15:47:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 15:47:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 16:04:33 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 16:04:34 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 16:04:35 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 16:04:35 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 16:04:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 16:04:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 16:07:44 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:46 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 16:07:48 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 16:07:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 16:07:49 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 16:07:50 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 16:07:50 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 16:07:51 GMT
EXPOSE 80
# Sat, 28 Dec 2019 16:07:52 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 05:04:06 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:06:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 05:06:32 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 05:06:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 05:06:38 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 05:06:39 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 05:06:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 05:06:48 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 05:06:52 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 05:07:22 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20b9b291ff1c8a76bfb2a542028eab868cdfeb8f7ce1b2816a2dd685bead53a7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadbe9ebf4298c5a6e9a9970ebfda7d6fcee35b1a30de8ee56d0a5ba5d12306`  
		Last Modified: Sat, 28 Dec 2019 17:10:35 GMT  
		Size: 59.5 MB (59500969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7f0f0a98e4a0343fb0ce2b3ee95aef4a695335ed00d7585878a052385fdac7`  
		Last Modified: Sat, 28 Dec 2019 17:10:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9280131d10e0a4bccd45d145fee5637ab0e0765ab559dd1e2b5dc7af27750c0`  
		Last Modified: Sat, 28 Dec 2019 17:11:09 GMT  
		Size: 17.5 MB (17482411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1816edc9dd5b62a2a48c193080b5268ad8c008bbe3ddca391d0b04f76205f7`  
		Last Modified: Sat, 28 Dec 2019 17:11:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cfad187f0b662b320dd69ffc0f6f8dfd3f3802162529030831c885da10cfde8`  
		Last Modified: Sat, 28 Dec 2019 17:11:03 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba412d4719663d33c51866d47de7345e1621312855e2db94800f664f40f9fc46`  
		Last Modified: Sat, 28 Dec 2019 17:12:50 GMT  
		Size: 12.4 MB (12438758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158410b29bc5cad857c8af8d243e90a2ef5c21d0f270cd6f3eb9f14192bfdb49`  
		Last Modified: Sat, 28 Dec 2019 17:12:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53d0ff92ce7f082a72df95f2334266d4209b0dca7c7c8c7ce8aea0ee8b25b07`  
		Last Modified: Sat, 28 Dec 2019 17:12:51 GMT  
		Size: 12.4 MB (12389028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a6a7649fcf1dc3b10b9d139d9bf7e601383add0639abc28ec09fb660733f14`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2efe161da3c5f30edf92e6113f47c5f5ec90557610df7bc1d23153fa786c541e`  
		Last Modified: Sat, 28 Dec 2019 17:12:48 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d918b07eae5c339e0737ac9c830418b24d504eee6e03986cf7353f8319c89f81`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452371523c58e6c53c6b43b2e7083bd45d47aa8563718ea062976b7f6d65bff5`  
		Last Modified: Sat, 28 Dec 2019 17:12:47 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e7b431fc2b68efc8f852bed077d13b915fee8e76e4d608b5426d395afbae89`  
		Last Modified: Sun, 29 Dec 2019 05:13:10 GMT  
		Size: 57.0 MB (57013104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dc54d7e0e858778ed287c4d054b42747522b4ebe67e7a57f868060dce8d514`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 2.7 MB (2711321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461d0281d7782cdaf29caf55dafb9b802a3cbd0af7793123b086133c8e622d33`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0e2b5086c134e4aced9bbdcc59edcc492ddec6cfa7191932a3a5b4b422cc0c`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb6903a78739071fb34b5aa3b5d6977902597d42343e9b401771bc228b392928`  
		Last Modified: Sun, 29 Dec 2019 05:12:51 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dcdcc55cd54b87347584b0f9a743f1cc3d88b86f1bf1b44fcca57f06e89a6d`  
		Last Modified: Sun, 29 Dec 2019 05:13:12 GMT  
		Size: 40.9 MB (40932366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:c41b4fece19a7eda9df74a8ad973b0085146bbf33a6c2394a56f53d1f5142691
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.9 MB (246913885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f70165dace035f4eeac8964f6f9667b9da5d3ba26fb151f86c029f2538324383`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:34:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 14:34:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 14:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:35:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 14:35:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 14:39:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 14:40:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 14:40:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 14:40:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 14:40:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 14:40:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 14:40:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 14:58:04 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 14:58:05 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 14:58:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 14:58:07 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 14:58:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 14:58:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:01:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 15:01:55 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:02:01 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 15:02:05 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 15:02:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 15:02:07 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 15:02:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 15:02:10 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 15:02:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 15:02:13 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 06:18:45 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:20:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 06:20:37 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 06:20:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 06:20:54 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 06:20:57 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 06:20:59 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 06:21:01 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 06:21:04 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 06:21:23 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8122173c172bc43784f104fb71aa1776a8615c131c729e70f550881523035d01`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77da451916b9bf0e21115b77fe13d76cc5ba92ffb452241f98f1f6da974c366`  
		Last Modified: Sat, 28 Dec 2019 16:07:56 GMT  
		Size: 70.3 MB (70335271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b031d86c7e7fc5c4c1f9be702b575c168ca6c602d89158e2a8bade9abe3c594c`  
		Last Modified: Sat, 28 Dec 2019 16:07:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ff20e5dfef45f1afca83759a318399f8a81e1aaba22b5307be488d2e1fbe81`  
		Last Modified: Sat, 28 Dec 2019 16:08:27 GMT  
		Size: 18.6 MB (18577647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245e3077408b6e8030226b0ce72eea3a01b0bc0f1f4ebe1a2154e42f9ce2a84a`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3090a390778cfa9720209069fb2b3ed504f255d2111e8ffdd7f986fa5fc96f2c`  
		Last Modified: Sat, 28 Dec 2019 16:08:22 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8241649bcf4d2c0e4de74b5e67bb5834ba5d996b49389c84d0f32a989b53ede4`  
		Last Modified: Sat, 28 Dec 2019 16:09:56 GMT  
		Size: 12.4 MB (12439327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e01a20edc8a7bd66d5648fcb221677d86430c207f9c97968483929222df1c9`  
		Last Modified: Sat, 28 Dec 2019 16:09:54 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdd333a6533fb4ebd12aa95ac0a21a8138a145f155144da2109445c06188c45`  
		Last Modified: Sat, 28 Dec 2019 16:09:58 GMT  
		Size: 13.8 MB (13763525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5992756a97c614d861128176ca4f21bbeb5c28e8c94e0127dbfc7bd01cb0141e`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e040aa8fe3067cbf62833e3e2b0452a789c765202130cc632949a1f135b4598c`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a45d8c12182c605c0d3ccdcc1c7e8d537d422b7a7692da668bd44bd9a863412`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab7296dc5aacd20a3cb5406612d125fa5d253c6fbf175024b04a6f885293db0`  
		Last Modified: Sat, 28 Dec 2019 16:09:53 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c520f8b3f9930cceaf2ab7fbea0dab9f280b0c4c910f6b92a0a0d1dcfefb5074`  
		Last Modified: Sun, 29 Dec 2019 06:27:19 GMT  
		Size: 62.2 MB (62181139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653d1f01cb89b01ac2491622e4180fb78330e3ae3d35ac94e31769783921b021`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 2.8 MB (2827061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e0645b51c7b70e20eb35c2f55959a9114ac5987935dd6ea3769bf087f2f531`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 578.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f3104adb907115dbcaf78d8db11472e663e3c693b2bdd717bfd0f7c864e5db`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abc8f4b9512b7d519327ed7527cbdc7ea7c6dddbf4fc2107034665c8e3a3479`  
		Last Modified: Sun, 29 Dec 2019 06:27:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0776b66828933d5d10d8d9e28113786b148f524f6466240561b9156a41555a4`  
		Last Modified: Sun, 29 Dec 2019 06:27:19 GMT  
		Size: 40.9 MB (40932574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable` - linux; 386

```console
$ docker pull mediawiki@sha256:0fd3e08dd5184937450379bb85b426ed9e87f236dd49b62d192acf329a77991b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.0 MB (265026151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83455a08dd11ca0df8cf1c9e88237819f4f026508f361a6b79f5446dbfe65d7c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 16:47:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 16:47:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 16:47:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 16:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 16:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 16:56:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 16:56:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 16:56:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 16:56:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 16:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 17:28:59 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 17:28:59 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 17:28:59 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 17:29:00 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 17:29:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 17:29:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 17:34:27 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:28 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 17:34:28 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 17:34:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 17:34:29 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 17:34:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 17:34:29 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 17:34:30 GMT
EXPOSE 80
# Sat, 28 Dec 2019 17:34:30 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 01:49:08 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:51:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 01:51:35 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 01:51:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 01:51:36 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 01:51:37 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 01:51:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7834f8ef235a445001f7975675aa8af1b872e0c7104ce978c07e59dc443dbec`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e81a6f724259f2ff6a49a67e0c30d55830e1534058351fab438c06d13a8170f`  
		Last Modified: Sat, 28 Dec 2019 19:32:45 GMT  
		Size: 81.2 MB (81199517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75064f0106e77c164ad954ecae2c728eb2076867d32fb11b447d14dfa02dd3e5`  
		Last Modified: Sat, 28 Dec 2019 19:32:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40761e8229cc73d8ea7d9fa0d451565c5ff38066ac2546dea71211509b36dd4a`  
		Last Modified: Sat, 28 Dec 2019 19:33:12 GMT  
		Size: 19.1 MB (19111841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cebfb9b041b1fae88162028743c04818963a522ea14ea6b174dbad195c9a41`  
		Last Modified: Sat, 28 Dec 2019 19:33:06 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f53ce68c003e5a9a03fd4b11879aeb24cfb5559217d3ed022d06647f6b95e306`  
		Last Modified: Sat, 28 Dec 2019 19:33:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbae8f4e561644d6fcb797a8a499d14be3b8e5f4e64cd9c11866211c3aa75b8e`  
		Last Modified: Sat, 28 Dec 2019 19:34:27 GMT  
		Size: 12.4 MB (12439783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2200f9f0e9086bbdd7693678f3fc977f28b45179fcd97d345cb8bf2303796ae6`  
		Last Modified: Sat, 28 Dec 2019 19:34:25 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5683d09b9e01268b13b81e0a6d2a42ba144c7afe1b5f84192459f6421e4ce10`  
		Last Modified: Sat, 28 Dec 2019 19:34:30 GMT  
		Size: 14.4 MB (14397717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97025580058c4727f58cd59f45f94aadef3f08a243448089e64a9d7cf7136557`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0418088aa2e9c1d45141e23bdaca8c4130ed3a741643b629eb1057fbfa16f04`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896d0f7b562bcc05e29ac3bcf325266b9635738affb3ee55e59a24d9741a019c`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86f2a214dfd81d395465643bc44d03d6d0ab7552ed58686d2f7745e34fadb43`  
		Last Modified: Sat, 28 Dec 2019 19:34:24 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d40990dd467c89da4a260e98d10d7a90f664d3169c2a48bf598db40f60e8b6`  
		Last Modified: Sun, 29 Dec 2019 01:56:39 GMT  
		Size: 66.3 MB (66332990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c6febce75820693e6c4e898a065204a7bb7787d9810aac90d7a8512f2083a8d`  
		Last Modified: Sun, 29 Dec 2019 01:55:59 GMT  
		Size: 2.9 MB (2858990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde3d4d1d88f3ed029aa9b4cdd85cd0e676358e0584795979cfcc05a6efda8c7`  
		Last Modified: Sun, 29 Dec 2019 01:55:56 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739e246f8ce3c87dcad419a9e9cd83e0ef3c9e7ff62c34acce2b4c27e6c20ba5`  
		Last Modified: Sun, 29 Dec 2019 01:55:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddd6a279f87a22c52a9c476bfd0681f6e67dcb59e4b3dd6e5d1c4f24eb52b27`  
		Last Modified: Sun, 29 Dec 2019 01:55:57 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257a5c5a35d34039bd859cd2fed06fc7d593b686fb11618bd8ee3da909546467`  
		Last Modified: Sun, 29 Dec 2019 01:56:37 GMT  
		Size: 40.9 MB (40931805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:926a1bd0a19244ef37247a70e76af381e5b262a61f13e9ba47c95e90e36f80df
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.2 MB (275228055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29105a492974cb1d750661e2b0cb46f8f38fbf977bda8a4643c09eaf3f3f8187`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 18:07:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 Dec 2019 18:07:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 Dec 2019 18:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 18:09:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Dec 2019 18:09:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Dec 2019 18:15:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 Dec 2019 18:15:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 Dec 2019 18:16:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 Dec 2019 18:17:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 Dec 2019 18:17:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 Dec 2019 18:17:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 28 Dec 2019 18:17:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 28 Dec 2019 18:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Dec 2019 18:17:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 28 Dec 2019 18:40:03 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Sat, 28 Dec 2019 18:40:06 GMT
ENV PHP_VERSION=7.3.13
# Sat, 28 Dec 2019 18:40:08 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.13.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.13.tar.xz.asc/from/this/mirror
# Sat, 28 Dec 2019 18:40:09 GMT
ENV PHP_SHA256=57ac55fe442d2da650abeb9e6fa161bd3a98ba6528c029f076f8bba43dd5c228 PHP_MD5=
# Sat, 28 Dec 2019 18:40:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 Dec 2019 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 28 Dec 2019 18:44:30 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:34 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 Dec 2019 18:44:38 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Sat, 28 Dec 2019 18:44:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 Dec 2019 18:44:43 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 18:44:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 Dec 2019 18:44:47 GMT
WORKDIR /var/www/html
# Sat, 28 Dec 2019 18:44:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 18:44:49 GMT
CMD ["apache2-foreground"]
# Sun, 29 Dec 2019 04:44:37 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:45:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 04:46:02 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Sun, 29 Dec 2019 04:46:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 Dec 2019 04:46:09 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sun, 29 Dec 2019 04:46:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Sun, 29 Dec 2019 04:46:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Sun, 29 Dec 2019 04:46:15 GMT
ENV MEDIAWIKI_VERSION=1.34.0
# Sun, 29 Dec 2019 04:46:16 GMT
ENV MEDIAWIKI_SHA512=b6b1aeec26a1c114eeec0bdf18d4b3160fe02dac2920a39a045acb74e62aa8f8a28e6a81c01fedba7976e4dd0c96463e0f1badfddd3015eef9197b01586a236d
# Sun, 29 Dec 2019 04:46:30 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253f3f96795b9e74581686a5867b34cf3ecd5456bb7932c9ec497837086b036c`  
		Last Modified: Sat, 28 Dec 2019 20:11:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3077abe7f19b79a3a23bfa7192e160eec857b8a062f0a13f4bf6bbce92bee057`  
		Last Modified: Sat, 28 Dec 2019 20:12:16 GMT  
		Size: 82.3 MB (82259503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c1c236ff11a718b8647ec9809cbe25c526a10c71b8062301809806c2d05bd`  
		Last Modified: Sat, 28 Dec 2019 20:11:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1372dfcd0e5e6d2bb1596fd6d6b76343945db2d38c2bf250246fb8cd3d5a2c1`  
		Last Modified: Sat, 28 Dec 2019 20:13:20 GMT  
		Size: 19.8 MB (19811373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324fd437fe3df3006e8a7a6aefd39c9ccc10c1b57193917c4e4cee049076d29b`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6942ad65b54758c147c0578b07c2458a0ac935892e3591c3222ad3085b3cb8`  
		Last Modified: Sat, 28 Dec 2019 20:13:10 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9634193639ed291491ea9f346a0554328813bb7b79d0416931174bcdea39df99`  
		Last Modified: Sat, 28 Dec 2019 20:16:00 GMT  
		Size: 12.4 MB (12440219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae57e04f3b19c888646aedbe8a470dee96faf2b4116fd493a4f1f8b558cfd99`  
		Last Modified: Sat, 28 Dec 2019 20:15:57 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21684f23e5fad6d298cee5be9f5edbdb30016b023be97524c1d1a0aae912d64`  
		Last Modified: Sat, 28 Dec 2019 20:16:00 GMT  
		Size: 15.1 MB (15125611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42481e0073e5430a6d6ac7f434499ae092a2e4eec3f8cc092e3824f8892d381f`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7793ac58e2b2da04ccc838ca0a711ec7cdb93cf59bc9ce21670a40b597304b51`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d325992be0623123fa8da4459947c53bacdfb00d3d57699f0252a81b33368f2`  
		Last Modified: Sat, 28 Dec 2019 20:15:54 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5354b81e9a9735e6d42aa4b9979bfbb6b9e0bd673aec99d34604fb687d59be0d`  
		Last Modified: Sat, 28 Dec 2019 20:15:55 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d597b22c2a647f907286930b6aebe07b9930094f9919a9c19e7cb43c6480cca`  
		Last Modified: Sun, 29 Dec 2019 04:52:49 GMT  
		Size: 71.2 MB (71193311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e463f8c0b36c08e1ecbf0b6e0f490530cbbea4e38faf2c0b9bb89da5d0f53d3`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 2.9 MB (2941366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538c2724296bd18e364881c99531c797daab73f2b82832b0efc2281e20a27201`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c569317609dd46d122aca2eecdea14d15a946ffb83e4dc3b642c91db181c51`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d6ec7d4fd0c652a627acb57607c8609a3f34ed4b55403c567976fa88a3c5ef`  
		Last Modified: Sun, 29 Dec 2019 04:52:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f033473836325de151dac311fd5af5f0c1ceff5abe02450702668a155f9a25`  
		Last Modified: Sun, 29 Dec 2019 04:52:44 GMT  
		Size: 40.9 MB (40932495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
