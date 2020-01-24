## `mediawiki:legacy`

```console
$ docker pull mediawiki@sha256:00946003c93494fe034a5db695572a9d91f2b8d4068fb7b848c35185d9b3eb8a
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
$ docker pull mediawiki@sha256:d440f341e7c08bb3f00691ca8ac6b0c54de2a91dbcf096b56ef8ca1f90fd8f0d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254491750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40b3dcd1510512fc234b4b3d2ea7d3f9bbcebf9c4a1513c26afd15076c2a633a`
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
# Fri, 24 Jan 2020 09:18:35 GMT
ENV PHP_VERSION=7.2.27
# Fri, 24 Jan 2020 09:18:35 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Fri, 24 Jan 2020 09:18:35 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Fri, 24 Jan 2020 09:18:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 24 Jan 2020 09:18:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jan 2020 09:21:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 24 Jan 2020 09:21:50 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 24 Jan 2020 09:21:51 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jan 2020 09:21:52 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 24 Jan 2020 09:21:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jan 2020 09:21:52 GMT
STOPSIGNAL SIGWINCH
# Fri, 24 Jan 2020 09:21:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 24 Jan 2020 09:21:53 GMT
WORKDIR /var/www/html
# Fri, 24 Jan 2020 09:21:53 GMT
EXPOSE 80
# Fri, 24 Jan 2020 09:21:53 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 11:41:28 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 11:42:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 11:42:53 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 11:42:54 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 11:42:55 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 11:42:55 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 24 Jan 2020 11:42:55 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 24 Jan 2020 11:42:55 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Fri, 24 Jan 2020 11:42:55 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Fri, 24 Jan 2020 11:43:05 GMT
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
	-	`sha256:5bf151d73a83027f8fb21515f810bb56f9cd310b4c693090f26e887638b3f8c8`  
		Last Modified: Fri, 24 Jan 2020 10:46:08 GMT  
		Size: 12.6 MB (12645397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d1780495b139a3125f0a8525eff5bd9fd2678db666976ae4fc0db7da9282ec`  
		Last Modified: Fri, 24 Jan 2020 10:46:05 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8acdee7575085d4185a179cc2bec5d7d81c6f0a39f2af3a94cdd3a1c429ec2`  
		Last Modified: Fri, 24 Jan 2020 10:46:14 GMT  
		Size: 13.8 MB (13841458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02f795e28ee2aeaeaaa3bfebc960821c4e705dae019e300345aaab229778907`  
		Last Modified: Fri, 24 Jan 2020 10:46:04 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae4ecc29fc811c88c40bc121192a1934756d552580bae5f4fdad52be64fcd64`  
		Last Modified: Fri, 24 Jan 2020 10:46:04 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abc78403636b9b5b84ae82af9092efef2e94cd0f66fd802a8b3567da76a026f`  
		Last Modified: Fri, 24 Jan 2020 10:46:04 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6181179a3e436f30ebe83fb2ea7e696ed1870038c5acb9b88ba9f49c5ec6423a`  
		Last Modified: Fri, 24 Jan 2020 10:46:05 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d805d05a25abc53d7add56193e6287ec3df84467cd1b6d5c95d90ed232e583`  
		Last Modified: Fri, 24 Jan 2020 11:44:20 GMT  
		Size: 64.4 MB (64389494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e202eb995f80f5ee5aad93379736fe0b6ea08839084698d5fd7174f758df5ad`  
		Last Modified: Fri, 24 Jan 2020 11:44:06 GMT  
		Size: 2.8 MB (2785459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e96d0514a3c50f09d8b977a56585e5c1bd815d0c36a82c08d780063e951566`  
		Last Modified: Fri, 24 Jan 2020 11:44:05 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725ee2b5b10f987b456d20303f55916e953df02cfb52831fd402f07991f65f03`  
		Last Modified: Fri, 24 Jan 2020 11:44:06 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41aa3c7643f8c9f9b9c2ebe92535d6a2a4f9c263c544f703472f41c819c9b39`  
		Last Modified: Fri, 24 Jan 2020 11:44:05 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811dbcdac959c26c7d6624baa8879b2af3b12d679ec26ce52d590e28a716462e`  
		Last Modified: Fri, 24 Jan 2020 11:44:18 GMT  
		Size: 38.4 MB (38403853 bytes)  
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
$ docker pull mediawiki@sha256:2f42798856bf84358adcf5cf8526a2ddcc6e756520b0dd1a5434f7b1d2dfbd37
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222594328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa41ff4546e554f8ad08bf8854ed47b5017dc3850fd741feec2d3c50fc615714`
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
# Thu, 23 Jan 2020 22:47:29 GMT
ENV PHP_VERSION=7.2.27
# Thu, 23 Jan 2020 22:47:30 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 22:47:31 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Thu, 23 Jan 2020 22:47:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jan 2020 22:47:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:50:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 22:50:46 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:50:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 22:50:51 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Jan 2020 22:50:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 22:50:53 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jan 2020 22:50:54 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jan 2020 22:50:56 GMT
WORKDIR /var/www/html
# Thu, 23 Jan 2020 22:50:57 GMT
EXPOSE 80
# Thu, 23 Jan 2020 22:50:58 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 04:29:10 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 04:30:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 04:30:35 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 04:30:37 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 04:30:39 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 04:30:39 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 24 Jan 2020 04:30:40 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 24 Jan 2020 04:30:40 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Fri, 24 Jan 2020 04:30:41 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Fri, 24 Jan 2020 04:30:59 GMT
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
	-	`sha256:26805bc203948aadeda056d2e497902da6f7228ca9e003b74e3bb86f95203b5f`  
		Last Modified: Thu, 23 Jan 2020 23:49:43 GMT  
		Size: 12.6 MB (12643304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba73644e5534d433ffb0dd19ca67d76d1fb18a3d80c2459736d7a7b27d65e340`  
		Last Modified: Thu, 23 Jan 2020 23:49:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef73dd928f58380ae9e7d2092eb19addd41c6c8619fb387e7e67e7ea588c9b0`  
		Last Modified: Thu, 23 Jan 2020 23:49:46 GMT  
		Size: 12.2 MB (12186073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d7e8782f8b61fe94c322abf2f7b727c171321fa9ca9c1e9c7d063920ea717c`  
		Last Modified: Thu, 23 Jan 2020 23:49:40 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc97c1c88db50814d265515a25406e833647256a6da41bd415359764756f7b02`  
		Last Modified: Thu, 23 Jan 2020 23:49:40 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92122c7c67a28259ca66bc51a4fc3ac5fc33167c8fc6ce3e2c8d39f7e59f9ed`  
		Last Modified: Thu, 23 Jan 2020 23:49:40 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87303932048be5e3a37d4be810a5fdf3890d2448457e93fae62d729a07668b81`  
		Last Modified: Thu, 23 Jan 2020 23:49:40 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422c3c96b0b69c25fc8f2e4bf95d614b0452d0e3082716295461ff3f20d9c578`  
		Last Modified: Fri, 24 Jan 2020 04:32:49 GMT  
		Size: 57.0 MB (57022552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a2d36704b34a5cd39360d7b836695b7ef414d6b65656282d4db792e7ad551a`  
		Last Modified: Fri, 24 Jan 2020 04:32:32 GMT  
		Size: 2.6 MB (2649295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cc0b4fccbbc586ba7c7f4a6c0959d2700e7b89c888ec3621be46d55bb5f8f30`  
		Last Modified: Fri, 24 Jan 2020 04:32:32 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f14981b9a86900e861c71d7561b9a8db07d13527df73fba80a572905a269ee`  
		Last Modified: Fri, 24 Jan 2020 04:32:31 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ee40068eea3b0191662548180291bf62bac98866564aa6479142abbcc0192c`  
		Last Modified: Fri, 24 Jan 2020 04:32:31 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d65a3c0d6a53e6db6e365bcb59a6b0bedb0e329ba9b8ceb035dabf1d7332b1`  
		Last Modified: Fri, 24 Jan 2020 04:32:55 GMT  
		Size: 38.4 MB (38403935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:c03e71e39f0374a047233095ddbb09db61c19f9d32958957d02723ab2f512573
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244300937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fde0c6eabd322f9553bcfafa3acb651bd26c2aa288f0bc16ca12cf44f464d41`
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
# Fri, 24 Jan 2020 01:40:45 GMT
ENV PHP_VERSION=7.2.27
# Fri, 24 Jan 2020 01:40:46 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Fri, 24 Jan 2020 01:40:48 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Fri, 24 Jan 2020 01:41:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 24 Jan 2020 01:41:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jan 2020 01:44:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 24 Jan 2020 01:44:26 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 24 Jan 2020 01:44:28 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jan 2020 01:44:29 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 24 Jan 2020 01:44:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jan 2020 01:44:31 GMT
STOPSIGNAL SIGWINCH
# Fri, 24 Jan 2020 01:44:31 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 24 Jan 2020 01:44:32 GMT
WORKDIR /var/www/html
# Fri, 24 Jan 2020 01:44:32 GMT
EXPOSE 80
# Fri, 24 Jan 2020 01:44:33 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 03:45:38 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 03:47:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 03:47:11 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 03:47:13 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 03:47:16 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 03:47:16 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 24 Jan 2020 03:47:17 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 24 Jan 2020 03:47:17 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Fri, 24 Jan 2020 03:47:19 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Fri, 24 Jan 2020 03:47:32 GMT
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
	-	`sha256:3af7fc8c1fada43905a4585b80be6a7f59869e0ac0c9cb19c6eac0ea64e5b6ac`  
		Last Modified: Fri, 24 Jan 2020 02:46:00 GMT  
		Size: 12.6 MB (12643956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe29be43e659f1f638ce2c0483d3b46a0c0b583f249332d771c31de1ce08398d`  
		Last Modified: Fri, 24 Jan 2020 02:45:58 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f11b5e345703533b6aa87455cd5a451296df2c2f89d39ac226b9c04c648a523`  
		Last Modified: Fri, 24 Jan 2020 02:45:59 GMT  
		Size: 13.5 MB (13536725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ec7bb197a5baf1d68c4d209daf5481a9da3c07d1b2d002c3b7579b27db6c8c`  
		Last Modified: Fri, 24 Jan 2020 02:45:56 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf686e3c7140108f25fd643a0fef4a051ca43e68996f2e5f9846300656c72dbe`  
		Last Modified: Fri, 24 Jan 2020 02:45:56 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e965c71c71193919e403147dde3b8ecef249fb12c1013c9d566068bd42036417`  
		Last Modified: Fri, 24 Jan 2020 02:45:56 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1787b9e736d36586a1d51fe2f516f1c04a5862c67aad27e65eaf8d8a0994cb`  
		Last Modified: Fri, 24 Jan 2020 02:45:57 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8531827bf8084e261a7e86dcc784c2285e125df84d24d465ceec8e690b24ce`  
		Last Modified: Fri, 24 Jan 2020 03:49:56 GMT  
		Size: 62.2 MB (62187204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a536b3059ca7d76c4d5ecee5dfe23df3aa3fed41d0a705bda74122f51fae6ec`  
		Last Modified: Fri, 24 Jan 2020 03:49:41 GMT  
		Size: 2.8 MB (2758682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edbf062ec9cdcf658cfec2307004ce510c5476545418dd1938ddfbdc2f41827`  
		Last Modified: Fri, 24 Jan 2020 03:49:36 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05cd70a0ec63ae6f2ea1817b8f4e8a6b39aad0b9c5b2764d2029ac0c0bc155f`  
		Last Modified: Fri, 24 Jan 2020 03:49:36 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c5f092fc344badbcab4ec4a23eff45726e6089512d302f2a253cadcb6ccce4`  
		Last Modified: Fri, 24 Jan 2020 03:49:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c290340bc1e5d05d8fc55ecc57c35829af4b5afe99bf7f46206f2b83ad0c66e`  
		Last Modified: Fri, 24 Jan 2020 03:50:08 GMT  
		Size: 38.4 MB (38404112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; 386

```console
$ docker pull mediawiki@sha256:cc0025c43e3cc00bca2d9b74f9dae2ac18ab2c33deff83f2510ae4983101282e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262400214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e75cb78c26e73eb09f6db6977abd8c42072aa54a79e123d80ab6dfe192cab607`
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
# Fri, 24 Jan 2020 01:21:22 GMT
ENV PHP_VERSION=7.2.27
# Fri, 24 Jan 2020 01:21:22 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Fri, 24 Jan 2020 01:21:22 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Fri, 24 Jan 2020 01:21:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 24 Jan 2020 01:21:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jan 2020 01:24:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 24 Jan 2020 01:24:51 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 24 Jan 2020 01:24:51 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jan 2020 01:24:52 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 24 Jan 2020 01:24:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jan 2020 01:24:52 GMT
STOPSIGNAL SIGWINCH
# Fri, 24 Jan 2020 01:24:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 24 Jan 2020 01:24:53 GMT
WORKDIR /var/www/html
# Fri, 24 Jan 2020 01:24:53 GMT
EXPOSE 80
# Fri, 24 Jan 2020 01:24:53 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 10:10:08 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 10:11:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 10:11:42 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 10:11:43 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 10:11:44 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 10:11:45 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 24 Jan 2020 10:11:45 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 24 Jan 2020 10:11:45 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Fri, 24 Jan 2020 10:11:46 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Fri, 24 Jan 2020 10:12:03 GMT
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
	-	`sha256:a39a9dec9dd465490f7f776a70b6d7fcc0c9ed93f140fc83b5c250d25b904ffa`  
		Last Modified: Fri, 24 Jan 2020 02:43:09 GMT  
		Size: 12.6 MB (12644533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfe7ed6407f9b24b8a8bd7a12731077682c3d7ffee99ff882d73b8770ca5ee8`  
		Last Modified: Fri, 24 Jan 2020 02:43:00 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09b6c401772c47c170a9440f58cba6e4406358f512dcb232cdb08b678a5f7ce`  
		Last Modified: Fri, 24 Jan 2020 02:43:11 GMT  
		Size: 14.2 MB (14169213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59d922f9bf8ab41f0c5e6af77b6aad6a7ce282bbcf687fdbfd1ab510fc2cb07`  
		Last Modified: Fri, 24 Jan 2020 02:42:59 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9259b0b395d5aeae0ff321de169aa51d94be1414b1e4754d352da2753e619ef8`  
		Last Modified: Fri, 24 Jan 2020 02:42:59 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a89431fcf33a2d103d3373ec3822ccf6baed58f301cbaa72e70ac9110caff8`  
		Last Modified: Fri, 24 Jan 2020 02:42:59 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f0051d00d58f456c22927f124b8724b600be621cd34abcd4ac547aa80d7a33`  
		Last Modified: Fri, 24 Jan 2020 02:42:59 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a81d5bcb3b7ee100a3081ba5f47134348fa460f9c5a7e9c31bb1281ac85a43`  
		Last Modified: Fri, 24 Jan 2020 10:14:37 GMT  
		Size: 66.3 MB (66341735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfac403792338af8cca9253a91ffe003eb2cba4bd9af620b2a3ea713b0456413`  
		Last Modified: Fri, 24 Jan 2020 10:13:42 GMT  
		Size: 2.8 MB (2775887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c334f54c17cc487b9c1d7db20b7f8a7f58c2a2363b26b9bb8af385007eaf149e`  
		Last Modified: Fri, 24 Jan 2020 10:13:41 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ab7005eb8b491067621435eb38e463370d88994aa90fc2259e5bf10b8d51d2`  
		Last Modified: Fri, 24 Jan 2020 10:13:40 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75de1b18da719acafecf757251b1bd3e6b3960ddda8fd4ebf46b1ae87a4db25`  
		Last Modified: Fri, 24 Jan 2020 10:13:40 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cdcc8471cdbbbc8e1b30919bbf15944932da961edbe7e8b4052e80f0e7e115`  
		Last Modified: Fri, 24 Jan 2020 10:14:15 GMT  
		Size: 38.4 MB (38403973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:87700cd260b606069a9de1b1ad06e8f1c338d7b903dbce5c157601c85547aa24
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272587226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c84286cac21d2feeaf06487d6e6edbff0b766776d1a6ed0b88386369f61f25`
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
# Fri, 24 Jan 2020 01:17:53 GMT
ENV PHP_VERSION=7.2.27
# Fri, 24 Jan 2020 01:17:57 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.27.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.27.tar.xz.asc/from/this/mirror
# Fri, 24 Jan 2020 01:17:59 GMT
ENV PHP_SHA256=7bd0fb9e3b63cfe53176d1f3565cd686f90b3926217158de5ba57091f49e4c32 PHP_MD5=
# Fri, 24 Jan 2020 01:18:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 24 Jan 2020 01:18:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jan 2020 01:22:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 24 Jan 2020 01:22:39 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 24 Jan 2020 01:22:48 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jan 2020 01:22:53 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 24 Jan 2020 01:22:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jan 2020 01:22:58 GMT
STOPSIGNAL SIGWINCH
# Fri, 24 Jan 2020 01:22:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 24 Jan 2020 01:23:01 GMT
WORKDIR /var/www/html
# Fri, 24 Jan 2020 01:23:03 GMT
EXPOSE 80
# Fri, 24 Jan 2020 01:23:05 GMT
CMD ["apache2-foreground"]
# Fri, 24 Jan 2020 09:37:03 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 09:38:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jan 2020 09:38:47 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 24 Jan 2020 09:38:57 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Jan 2020 09:39:07 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 24 Jan 2020 09:39:10 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 24 Jan 2020 09:39:12 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 24 Jan 2020 09:39:15 GMT
ENV MEDIAWIKI_VERSION=1.33.2
# Fri, 24 Jan 2020 09:39:19 GMT
ENV MEDIAWIKI_SHA512=bdbdd508360ab84a611dc1c57b1504fa5591d08ac24c511430bdb802999f8c7f7e323f1a9a2dd7a405291889f4bff8ca7a8b8911bfed0bd460444bfae52b271c
# Fri, 24 Jan 2020 09:39:36 GMT
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
	-	`sha256:4f5f4261eade962bad58ec7f712615d695dfba3bc49174e5dec74a9d33b136ad`  
		Last Modified: Fri, 24 Jan 2020 02:44:05 GMT  
		Size: 12.6 MB (12645005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c4cb21bfc01fd93a9e418cf7bc2327e279bb2df4649a3da6db84f72bb408c5`  
		Last Modified: Fri, 24 Jan 2020 02:44:03 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0996209acd92ef0fa07ed86c14082220cb0f713b198ba2a941b223fe0cf753d0`  
		Last Modified: Fri, 24 Jan 2020 02:44:05 GMT  
		Size: 14.9 MB (14882858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9131065afee7c0bee89bbc44fb4436e2b58ff0e21c79130e156400c68e26df4e`  
		Last Modified: Fri, 24 Jan 2020 02:44:01 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801e21322eb9a58aa48fa2c039c10045f27a8fd47d1f96e160a76658eacd6829`  
		Last Modified: Fri, 24 Jan 2020 02:44:00 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b79d68cb91344e97e77178c1de2c78953eed938b075a8ebb62b710a51c5801a`  
		Last Modified: Fri, 24 Jan 2020 02:44:00 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c034275e5ae4c2f35342f8f011f4369f4352a24db20dc39abee71d8e7b8cbc4d`  
		Last Modified: Fri, 24 Jan 2020 02:44:00 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4cf4fcdc96620f38b6c4e7ba9fc7d6c3b48b3e1e45380f99ce1689a3f8c4d4`  
		Last Modified: Fri, 24 Jan 2020 09:42:38 GMT  
		Size: 71.2 MB (71196565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736feba5e96217beb4a406d9b16e1ac6b1aac7994c3e81136f42425ff5edb934`  
		Last Modified: Fri, 24 Jan 2020 09:42:20 GMT  
		Size: 2.9 MB (2863841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22b3feb2464edd38b875ae5e32d1553865e630adccdcc56b8521a7e750e2939`  
		Last Modified: Fri, 24 Jan 2020 09:42:20 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff0358c49b4a654713b3aca245509a644d754165ff4646b1ff21c0d17c4fe73`  
		Last Modified: Fri, 24 Jan 2020 09:42:19 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d6353fc51ca544ce3c801c949e33066eca8d59d52ff49cae8b6a99c11d5aaa`  
		Last Modified: Fri, 24 Jan 2020 09:42:19 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b6b77c9ef786c6973d34cc5b15118148ef995c6de1d45741b79aad1d1543e4`  
		Last Modified: Fri, 24 Jan 2020 09:42:32 GMT  
		Size: 38.4 MB (38403891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
