## `wordpress:5-apache`

```console
$ docker pull wordpress@sha256:ba33cd91cc95b64b9b26b5755bc127fa4d7f37ee79d453179e702757ec338d3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `wordpress:5-apache` - linux; amd64

```console
$ docker pull wordpress@sha256:e206cd1d5888b601bb7b835b55181348375c4a494a2b1b4ad9c772de02b16f62
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.4 MB (187375077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee025cbcbc20b95a9e724abe0d8765d88effd253cecbacb7ab3b42dc1dceb462`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 15:46:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 15:46:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 15:46:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 15:47:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 15:47:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 15:56:05 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 22 Nov 2019 15:56:05 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 22 Nov 2019 15:56:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 22 Nov 2019 15:56:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 22 Nov 2019 15:56:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 22 Nov 2019 15:56:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 22 Nov 2019 15:56:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 22 Nov 2019 15:56:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 15:56:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 15:56:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 16:27:06 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 22 Nov 2019 16:27:06 GMT
ENV PHP_VERSION=7.3.12
# Fri, 22 Nov 2019 16:27:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.12.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.12.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 16:27:06 GMT
ENV PHP_SHA256=aafe5e9861ad828860c6af8c88cdc1488314785962328eb1783607c1fdd855df PHP_MD5=
# Fri, 22 Nov 2019 16:27:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 22 Nov 2019 16:27:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 16:33:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:22:01 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:22:02 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:22:03 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 06 Dec 2019 01:22:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:22:03 GMT
STOPSIGNAL SIGWINCH
# Fri, 06 Dec 2019 01:22:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:22:03 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:22:04 GMT
EXPOSE 80
# Fri, 06 Dec 2019 01:22:04 GMT
CMD ["apache2-foreground"]
# Fri, 06 Dec 2019 03:22:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:23:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:23:48 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 03:23:49 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 03:23:50 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 06 Dec 2019 03:23:50 GMT
VOLUME [/var/www/html]
# Fri, 06 Dec 2019 03:23:50 GMT
ENV WORDPRESS_VERSION=5.3
# Fri, 06 Dec 2019 03:23:50 GMT
ENV WORDPRESS_SHA1=e3edcb1131e539c2b2e10fed37f8b6683c824a98
# Fri, 06 Dec 2019 03:23:56 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 06 Dec 2019 03:23:57 GMT
COPY file:2413d0c63f9d7b1d114697b18317719a02eadaaa61fc5d0c1edd96c027bc57a4 in /usr/local/bin/ 
# Fri, 06 Dec 2019 03:23:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Dec 2019 03:23:57 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae4f9fcfeea62b9197d4d4597ac8cc5345bd9da718e89a49509af78476d2e40`  
		Last Modified: Fri, 22 Nov 2019 19:07:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f22fbbd07a4ea653467bc27962a5f8afccd9318c8f5c8b3b2afa58d8c9c2db`  
		Last Modified: Fri, 22 Nov 2019 19:07:55 GMT  
		Size: 76.7 MB (76652068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc7a63ad75ffb773427b460e6f531cca45c92111ba8bb214172a53e5e7ceba2`  
		Last Modified: Fri, 22 Nov 2019 19:07:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2427b8dd6e72b90d85f0e543ad1fcf471b7eb3d164ce0481b977323e6cf61d3`  
		Last Modified: Fri, 22 Nov 2019 19:08:12 GMT  
		Size: 18.7 MB (18675687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cac3b30184c5bb16912132a60d627de3cdfd089e40331aed9beb3bf7ae5303`  
		Last Modified: Fri, 22 Nov 2019 19:08:07 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e40015fc102e70720aea18a61991f1ebc600c4646b5622558c49a4d74166ae`  
		Last Modified: Fri, 22 Nov 2019 19:08:07 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3951eb02eb9d90ae1badc0a7e876ea7f99b42e2fc6fea15f13e1e45cb0f5a0ad`  
		Last Modified: Fri, 22 Nov 2019 19:09:26 GMT  
		Size: 12.4 MB (12433322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30c5ce4d8259231a0533058fdb117a6612f929d93db07e98de857cd6f49d489`  
		Last Modified: Fri, 22 Nov 2019 19:09:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2fc8e19e4d029111119a9772673c9058c8d5d0a1767d554e3789422c153a51`  
		Last Modified: Fri, 22 Nov 2019 19:09:28 GMT  
		Size: 14.1 MB (14066064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c746235d858f74f914cb020a967c6f081a37a9398e0a774e823b73a520d5e53`  
		Last Modified: Fri, 06 Dec 2019 01:27:48 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887411e72bcf0f6ccc73e439fc476d75bc5a586d2df4f0ae672ca48da1c7074c`  
		Last Modified: Fri, 06 Dec 2019 01:27:48 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba633920d4457b921eb682ff90f104069510e83984124f1e1c30eddb412af45`  
		Last Modified: Fri, 06 Dec 2019 01:27:48 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7007daa55e7fb41d856988597117346a618f26548823dcd08a6c083b083a55`  
		Last Modified: Fri, 06 Dec 2019 01:27:48 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d20187eeb14212723156207512bf63e24b9b4fbc9e1a68125f3877c06143d15`  
		Last Modified: Fri, 06 Dec 2019 03:37:15 GMT  
		Size: 16.7 MB (16696426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1b35074ec2159c9722b3bf761ba6613df2c87c0844d0555db4815dc053cf35`  
		Last Modified: Fri, 06 Dec 2019 03:37:13 GMT  
		Size: 9.5 MB (9519990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13668f53adae1fa604e9dcc93897845e19cd2a439b6e7e3f69bf79b964d4f04`  
		Last Modified: Fri, 06 Dec 2019 03:37:10 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38760061f7fb031381ab5cfd9c3ad1fb709edbca382d2487cfd91444aeeaf50b`  
		Last Modified: Fri, 06 Dec 2019 03:37:10 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9448b0eeecaebd341e1de46a4d9482b9d6217623f2951fca55eec2df4c6bf743`  
		Last Modified: Fri, 06 Dec 2019 03:37:10 GMT  
		Size: 19.5 KB (19471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f402ca3df6d4769cab44feb12b201e3d5cdbe9d120b6bc0ac8ac19b018111e`  
		Last Modified: Fri, 06 Dec 2019 03:37:13 GMT  
		Size: 12.2 MB (12209321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6515b8350ad015b6f18f47e9ca58ffd27759ba197d5ef83fa41fb3ed2eb13165`  
		Last Modified: Fri, 06 Dec 2019 03:37:10 GMT  
		Size: 3.9 KB (3898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-apache` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:6e219fb0979d232a56fc6d700e4a807671b41a131be138a12ac874c9ebddd009
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.1 MB (164080259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89c44cce696b2b732a38e3859365c2e83e819eaf49bd65fbc1fff4054a8aba09`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 22 Nov 2019 12:13:54 GMT
ADD file:94ed554e445cf749e10644dfa0d836103c120a6ea388bf6dc9f18f7c6b2f095a in / 
# Fri, 22 Nov 2019 12:13:56 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 12:28:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 12:28:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 12:29:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 12:29:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 12:29:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 12:34:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 22 Nov 2019 12:34:13 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 22 Nov 2019 12:34:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 22 Nov 2019 12:34:45 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 22 Nov 2019 12:34:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 22 Nov 2019 12:34:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 22 Nov 2019 12:34:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 22 Nov 2019 12:34:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 12:34:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 12:34:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 12:52:39 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 22 Nov 2019 12:52:40 GMT
ENV PHP_VERSION=7.3.12
# Fri, 22 Nov 2019 12:52:43 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.12.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.12.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 12:52:44 GMT
ENV PHP_SHA256=aafe5e9861ad828860c6af8c88cdc1488314785962328eb1783607c1fdd855df PHP_MD5=
# Fri, 22 Nov 2019 12:53:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 22 Nov 2019 12:53:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 12:56:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 00:53:26 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 06 Dec 2019 00:53:32 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 00:53:35 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 06 Dec 2019 00:53:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 00:53:38 GMT
STOPSIGNAL SIGWINCH
# Fri, 06 Dec 2019 00:53:41 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 06 Dec 2019 00:53:46 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 00:53:50 GMT
EXPOSE 80
# Fri, 06 Dec 2019 00:53:55 GMT
CMD ["apache2-foreground"]
# Fri, 06 Dec 2019 03:13:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:18:16 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:18:20 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 03:18:23 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 03:18:29 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 06 Dec 2019 03:18:33 GMT
VOLUME [/var/www/html]
# Fri, 13 Dec 2019 22:54:15 GMT
ENV WORDPRESS_VERSION=5.3.1
# Fri, 13 Dec 2019 22:54:16 GMT
ENV WORDPRESS_SHA1=3c635c9f6546782e0bb315784d4663d0e47f872e
# Fri, 13 Dec 2019 22:54:22 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 13 Dec 2019 22:54:23 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 13 Dec 2019 22:54:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Dec 2019 22:54:24 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:45ae7e8aa5bfd9e1b0db11d7fa5a56a8af11b69fc56707d763f89aa2c61b7e8f`  
		Last Modified: Fri, 22 Nov 2019 12:22:20 GMT  
		Size: 24.8 MB (24829480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058ca8d797488ba0c2d7679f80443f86906e5b266ac3f533defc5be84ba8ee3`  
		Last Modified: Fri, 22 Nov 2019 14:42:32 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d09ee579a05967b60dc35947a1a6eee96a599461e6aab3ef950c5f4fb60825`  
		Last Modified: Fri, 22 Nov 2019 14:42:52 GMT  
		Size: 58.8 MB (58799873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984298e877a210abb92274d4ba555ba6becc0f83aa91ca5bf71ac7b7edf0dcba`  
		Last Modified: Fri, 22 Nov 2019 14:42:32 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115b9774efa90b1ce522d52e1cba7b2f511d3c91785b479a189cf3e3aa9d399d`  
		Last Modified: Fri, 22 Nov 2019 14:43:21 GMT  
		Size: 18.0 MB (18024413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36c919440512071050f50afdb85f5c50ab4d8550c861dbd2aef35596bb916c5`  
		Last Modified: Fri, 22 Nov 2019 14:43:16 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a105ec5710bdc0958d0ae053f75986302ae5d5d441e291e5ed9c3824ae8ebe7`  
		Last Modified: Fri, 22 Nov 2019 14:43:16 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dce388e04bf3ffa5abe74eeff7048aa8cf09358368ede39ca0a1c2647587d2`  
		Last Modified: Fri, 22 Nov 2019 14:44:55 GMT  
		Size: 12.4 MB (12431115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33fd65a838f1f74a38bd75a26e97bf650cfb1a0d03ee028ec4939af9f56aa00`  
		Last Modified: Fri, 22 Nov 2019 14:44:53 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de19b8058491b5ffd4acbdc219c327bd484684e238ce92eff82f0634b0c7df1`  
		Last Modified: Fri, 22 Nov 2019 14:44:57 GMT  
		Size: 13.1 MB (13085515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddbfbd445609309c789e5535f27d88d2be5018b584d1765f9602b28b4da0958d`  
		Last Modified: Fri, 06 Dec 2019 01:07:41 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708cc7709cf2b49742f39020a53c7f083d6b09a456a7af3dc529d44d4f785ac3`  
		Last Modified: Fri, 06 Dec 2019 01:07:41 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e09044db0f705a485e4bbd2702accdf071c58006bd14b38325f065ce9c766a`  
		Last Modified: Fri, 06 Dec 2019 01:07:40 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e1ed04167044e32db6c408bc9b9c334a7ff42e308473c72d7ecbc7e1a6ea5c`  
		Last Modified: Fri, 06 Dec 2019 01:07:41 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ee1f980486ed02521fa64873cbc20fe3ca962a793c06206e075fe53fcc56b1`  
		Last Modified: Fri, 06 Dec 2019 03:38:53 GMT  
		Size: 16.3 MB (16271660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e7737d2a3ad4bb0e263ce50a514ff79654845049ff9d811692ef6a1ee2be17`  
		Last Modified: Fri, 06 Dec 2019 03:38:49 GMT  
		Size: 8.4 MB (8382135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dd1d5c9a03757d05c2e8a2879b363f55464a62e32dc9288abd6a28478468e1`  
		Last Modified: Fri, 06 Dec 2019 03:38:44 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f3daa6a7131fb6f812d6916730b38d71646775c7091c9d61e363afaec39048`  
		Last Modified: Fri, 06 Dec 2019 03:38:44 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3238e0db3a95b365fa3a60923f7591a40325815b804593051f1651ced4fb70d5`  
		Last Modified: Fri, 06 Dec 2019 03:38:43 GMT  
		Size: 19.5 KB (19494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e92e92b39251036a3f7e3ba7eb63489cf5760b8a6818cfc8bd7b8e0e14972c`  
		Last Modified: Fri, 13 Dec 2019 22:56:44 GMT  
		Size: 12.2 MB (12226382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794aa218427b107bdfa239021f7699a6259512717e35c4e375d8ad9f3f569e9`  
		Last Modified: Fri, 13 Dec 2019 22:56:38 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-apache` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:66683cf8a571a6d6468d4824d5a407dcb886e006b3924a1e98a0c6af3f82488e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160122559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e47667e141464163c23e15cd86e15c30c705bd6ce9b49935ce182fdf6f910cbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 15:30:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 15:30:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 15:31:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 15:31:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 15:31:46 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 15:35:38 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 22 Nov 2019 15:35:41 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 22 Nov 2019 15:36:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 22 Nov 2019 15:36:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 22 Nov 2019 15:36:37 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 22 Nov 2019 15:36:40 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 22 Nov 2019 15:36:42 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 22 Nov 2019 15:36:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 15:36:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 15:36:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 15:52:05 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 22 Nov 2019 15:52:06 GMT
ENV PHP_VERSION=7.3.12
# Fri, 22 Nov 2019 15:52:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.12.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.12.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 15:52:07 GMT
ENV PHP_SHA256=aafe5e9861ad828860c6af8c88cdc1488314785962328eb1783607c1fdd855df PHP_MD5=
# Fri, 22 Nov 2019 15:52:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 22 Nov 2019 15:52:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 15:55:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:18:52 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:18:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:19:00 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 06 Dec 2019 01:19:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:19:02 GMT
STOPSIGNAL SIGWINCH
# Fri, 06 Dec 2019 01:19:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:19:04 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:19:05 GMT
EXPOSE 80
# Fri, 06 Dec 2019 01:19:06 GMT
CMD ["apache2-foreground"]
# Fri, 06 Dec 2019 03:18:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:22:57 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:23:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 03:23:06 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 03:23:09 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 06 Dec 2019 03:23:10 GMT
VOLUME [/var/www/html]
# Fri, 06 Dec 2019 03:23:10 GMT
ENV WORDPRESS_VERSION=5.3
# Fri, 06 Dec 2019 03:23:11 GMT
ENV WORDPRESS_SHA1=e3edcb1131e539c2b2e10fed37f8b6683c824a98
# Fri, 06 Dec 2019 03:23:17 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 06 Dec 2019 03:23:19 GMT
COPY file:2413d0c63f9d7b1d114697b18317719a02eadaaa61fc5d0c1edd96c027bc57a4 in /usr/local/bin/ 
# Fri, 06 Dec 2019 03:23:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Dec 2019 03:23:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d332694ad538d1f749e4fdcacbe4a6623985ed44a42e43bce63a9722db08b2f`  
		Last Modified: Fri, 22 Nov 2019 17:35:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c8dc0f21f8205464804617dcf082c2798fa80a5e67d2ba4688e5ebaa9e107b`  
		Last Modified: Fri, 22 Nov 2019 17:35:41 GMT  
		Size: 59.5 MB (59501056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbced36a6afa723160f24df74e373efd1409afd61b9af9d53109c1c8b721c28`  
		Last Modified: Fri, 22 Nov 2019 17:35:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0108ae93c2b9ac952780f9e43e8a09801145c8ce7d93455a6d0058dba97bfb07`  
		Last Modified: Fri, 22 Nov 2019 17:36:08 GMT  
		Size: 17.5 MB (17482686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2cff43cd8b0a0143900fa6f392ac8e73488444adb3d9482ccf1ac532afd19e`  
		Last Modified: Fri, 22 Nov 2019 17:36:03 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e90528d14553280d36ab02a7f94a903f1973be8ed599a06659a14a0e3875b4e`  
		Last Modified: Fri, 22 Nov 2019 17:36:03 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da9578dddb59cf31bfab4f32e49895cc16af8db16dc7dd910a5077d8989363f`  
		Last Modified: Fri, 22 Nov 2019 17:37:45 GMT  
		Size: 12.4 MB (12431133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1886de8f440d9fbf57da1929afca59d8ce953b025be942933f14e658fe0264e`  
		Last Modified: Fri, 22 Nov 2019 17:37:44 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e269ad3b52ba5b04398e9106fc73220de3635964758debe82f03fcc41ea2b9b1`  
		Last Modified: Fri, 22 Nov 2019 17:37:45 GMT  
		Size: 12.4 MB (12386343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961c3928257f2cb17e58549753500d26f9c6837448398680af2987c15e3d23b3`  
		Last Modified: Fri, 06 Dec 2019 01:37:02 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d0e05dd079e27b6d3a32b58d130e47044b03e12d26b53435efa40bfb1f244e`  
		Last Modified: Fri, 06 Dec 2019 01:37:02 GMT  
		Size: 253.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe9b2f7638efeede4c685f55c2da8169f735d0b08dae46906a54d28cebb0e6d`  
		Last Modified: Fri, 06 Dec 2019 01:37:02 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af29ff4b62798dbed064b565d6aa562103a7f1db6f31b09dc9074dff66d043a`  
		Last Modified: Fri, 06 Dec 2019 01:37:02 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f014cbd6f36c028be17fe09bdd8c13ec36eb61065c0b028e925c4e4de4c96cc0`  
		Last Modified: Fri, 06 Dec 2019 03:56:35 GMT  
		Size: 15.9 MB (15850190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1c96ea0ee6f9bec5a406e26a8f488c4c38744781bb4d5ae5bd227f4b1c4e10`  
		Last Modified: Fri, 06 Dec 2019 03:56:31 GMT  
		Size: 7.5 MB (7533094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c828e9cbbb38c12a2400741430321b1b4d94be7efa97fa6d6857de9ea37658`  
		Last Modified: Fri, 06 Dec 2019 03:56:26 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bcd188720dda840d519ac906d3cd039a65c9d3560b8da5b90858dfcc4c50fd`  
		Last Modified: Fri, 06 Dec 2019 03:56:26 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15d45ee0e26b53da9f23f7c4d61b6d0f598fcf09ad0d5bd50a32bb986ef6c03`  
		Last Modified: Fri, 06 Dec 2019 03:56:26 GMT  
		Size: 19.5 KB (19484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4b9637a8112b6138fb674a51ee6b690ea178fa080acdbb334bf9a77fe6728d`  
		Last Modified: Fri, 06 Dec 2019 03:56:33 GMT  
		Size: 12.2 MB (12209318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab73bae4bdf4e6ed5b8aeef12e1f56f3d15e86608d581efccafcb0e96c182e9d`  
		Last Modified: Fri, 06 Dec 2019 03:56:26 GMT  
		Size: 3.9 KB (3898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-apache` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:519407e45d233db65180be7c667ea641b426b1bb18663af0cb014041259e0a3f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.8 MB (177780470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15f26cc09736404570c73416488cdd1f394858d3ebd62aff186feb07f717ad64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 14:29:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 14:30:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 14:30:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 14:30:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 14:30:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 14:35:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 22 Nov 2019 14:35:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 22 Nov 2019 14:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 22 Nov 2019 14:35:42 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 22 Nov 2019 14:35:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 22 Nov 2019 14:35:46 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 22 Nov 2019 14:35:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 22 Nov 2019 14:35:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 14:35:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 14:35:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 14:51:55 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 22 Nov 2019 14:51:55 GMT
ENV PHP_VERSION=7.3.12
# Fri, 22 Nov 2019 14:51:56 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.12.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.12.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 14:51:57 GMT
ENV PHP_SHA256=aafe5e9861ad828860c6af8c88cdc1488314785962328eb1783607c1fdd855df PHP_MD5=
# Fri, 22 Nov 2019 14:52:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 22 Nov 2019 14:52:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 14:55:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:14:50 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:14:54 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:14:57 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 06 Dec 2019 01:14:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:14:58 GMT
STOPSIGNAL SIGWINCH
# Fri, 06 Dec 2019 01:14:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:15:00 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:15:01 GMT
EXPOSE 80
# Fri, 06 Dec 2019 01:15:11 GMT
CMD ["apache2-foreground"]
# Fri, 06 Dec 2019 02:56:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:00:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:00:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 03:00:27 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 03:00:33 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 06 Dec 2019 03:00:33 GMT
VOLUME [/var/www/html]
# Fri, 13 Dec 2019 22:43:13 GMT
ENV WORDPRESS_VERSION=5.3.1
# Fri, 13 Dec 2019 22:43:14 GMT
ENV WORDPRESS_SHA1=3c635c9f6546782e0bb315784d4663d0e47f872e
# Fri, 13 Dec 2019 22:43:19 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 13 Dec 2019 22:43:20 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 13 Dec 2019 22:43:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Dec 2019 22:43:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f8c59bdaec8c1ab048fd2338d7e3089ffd471db8a7da2fa1b06ac9378eb2d`  
		Last Modified: Fri, 22 Nov 2019 16:35:55 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae19fe01dd7281aa7d623b1511e9f37b42de475fe01580853799b004a3cc54e`  
		Last Modified: Fri, 22 Nov 2019 16:36:16 GMT  
		Size: 70.3 MB (70334484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939a6e43e07c4339d2d353898d5f439d1903e980852de2083f6c0230629bd2e7`  
		Last Modified: Fri, 22 Nov 2019 16:35:56 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bc60aacdf354efd72e1ab6ae5a4adb77b31dc9d5d25c207002b742f6bfccee`  
		Last Modified: Fri, 22 Nov 2019 16:36:44 GMT  
		Size: 18.6 MB (18577599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e1bedfb04e22d79d41a7b599a1a482ebca0ab22e3c9bee5bbca9e093f607ad`  
		Last Modified: Fri, 22 Nov 2019 16:36:39 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8332b84412645f3a8c9fb823daaafe6ea375117e8924a55e3fbafe06e979b9ed`  
		Last Modified: Fri, 22 Nov 2019 16:36:39 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012fa89ca2bc4881a4e194e5132959af71c057cb8311250394093a88b662e3d4`  
		Last Modified: Fri, 22 Nov 2019 16:38:23 GMT  
		Size: 12.4 MB (12431913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0dfb13372af1d962c88127cbcfc3136a7184bc8a5306690d96e7216ae0c1469`  
		Last Modified: Fri, 22 Nov 2019 16:38:21 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbeabdc4805b38c73352fa077936eb5d6e65c48ae5f13a24b83e2c5bfeac7da`  
		Last Modified: Fri, 22 Nov 2019 16:38:22 GMT  
		Size: 13.8 MB (13753683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e492268eedfdd1a8dedf58cf158cdfeb22e160aca69923f6103ebbe087fe0fd`  
		Last Modified: Fri, 06 Dec 2019 01:33:12 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2ddafb0478165df4c781f5f7203ff050307fcc3645155a7c9b923fafe607f7`  
		Last Modified: Fri, 06 Dec 2019 01:33:12 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02565d248c3e1307bd4a46c4c0fdd370843faf36faf13f2b8ec2f01c7835181`  
		Last Modified: Fri, 06 Dec 2019 01:33:12 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8259639516c05be0baa633a86226c3b0c09c49fe5343fb12853ad9a8192802`  
		Last Modified: Fri, 06 Dec 2019 01:33:12 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efb6c94a4c93e28b3aba0d958c07a922ebcfe6f80ee40b8bbf5b264bbccd532`  
		Last Modified: Fri, 06 Dec 2019 03:30:55 GMT  
		Size: 16.6 MB (16641714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f6d83e6c7aebec5dcf4a2606d32c89c7034411f2b6dfadd2ab6ebe377f458a`  
		Last Modified: Fri, 06 Dec 2019 03:30:51 GMT  
		Size: 7.9 MB (7934215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3601f2116010ea509c7a753b8b50e616c8483138dcce6519af86e8f81fd1f5f9`  
		Last Modified: Fri, 06 Dec 2019 03:30:46 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec7c7d8a18071fb570f2a930d42140ad0c39f10b49f32f9df8e909692a8d688`  
		Last Modified: Fri, 06 Dec 2019 03:30:45 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b834909e81a97aa75c1eefe125853ff9385b030e755677ec6d9cf9b90fca09b8`  
		Last Modified: Fri, 06 Dec 2019 03:30:46 GMT  
		Size: 19.5 KB (19499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854d93d71296673a84537bddb466196886fcd3449f8f4ea10ef81006c5bf11c6`  
		Last Modified: Fri, 13 Dec 2019 22:47:04 GMT  
		Size: 12.2 MB (12226375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca0a34d95e27b324361cb3b148041fc255882b920e015bb51147849bac8ace89`  
		Last Modified: Fri, 13 Dec 2019 22:46:59 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-apache` - linux; 386

```console
$ docker pull wordpress@sha256:c31aced230484d99c767732d7310d5cc1decf02ce0178d6203407a46c869417e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.9 MB (192928769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b079b4ba29c5a6d8610fd9396889522fce307fa99ae075f631178b42f0ea8881`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 19:18:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 19:18:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 19:18:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 19:18:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 19:18:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 19:25:18 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 22 Nov 2019 19:25:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 22 Nov 2019 19:25:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 22 Nov 2019 19:25:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 22 Nov 2019 19:25:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 22 Nov 2019 19:25:33 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 22 Nov 2019 19:25:33 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 22 Nov 2019 19:25:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 19:25:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 19:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 19:50:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 22 Nov 2019 19:50:11 GMT
ENV PHP_VERSION=7.3.12
# Fri, 22 Nov 2019 19:50:11 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.12.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.12.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 19:50:11 GMT
ENV PHP_SHA256=aafe5e9861ad828860c6af8c88cdc1488314785962328eb1783607c1fdd855df PHP_MD5=
# Fri, 22 Nov 2019 19:50:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 22 Nov 2019 19:50:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 19:54:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 00:42:03 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 06 Dec 2019 00:42:04 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 00:42:04 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 06 Dec 2019 00:42:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 00:42:05 GMT
STOPSIGNAL SIGWINCH
# Fri, 06 Dec 2019 00:42:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 06 Dec 2019 00:42:05 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 00:42:05 GMT
EXPOSE 80
# Fri, 06 Dec 2019 00:42:06 GMT
CMD ["apache2-foreground"]
# Fri, 06 Dec 2019 02:38:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 02:40:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 02:40:43 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 02:40:43 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 02:40:44 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 06 Dec 2019 02:40:45 GMT
VOLUME [/var/www/html]
# Fri, 06 Dec 2019 02:40:45 GMT
ENV WORDPRESS_VERSION=5.3
# Fri, 06 Dec 2019 02:40:45 GMT
ENV WORDPRESS_SHA1=e3edcb1131e539c2b2e10fed37f8b6683c824a98
# Fri, 06 Dec 2019 02:40:56 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 06 Dec 2019 02:40:56 GMT
COPY file:2413d0c63f9d7b1d114697b18317719a02eadaaa61fc5d0c1edd96c027bc57a4 in /usr/local/bin/ 
# Fri, 06 Dec 2019 02:40:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Dec 2019 02:40:56 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed961f8f7a554aab7872678c1e2706e804ac741f6ab6db08d468f95281c88da`  
		Last Modified: Fri, 22 Nov 2019 22:13:02 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077599002175aec10526395f1b56a347a4e6d6b5a6bd9320c9b42bad0768df3c`  
		Last Modified: Fri, 22 Nov 2019 22:13:27 GMT  
		Size: 81.2 MB (81199104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59337e9a9db23ff3d6d91ee673a989078459ee463b0e7cd7a9875b071b3ca7b`  
		Last Modified: Fri, 22 Nov 2019 22:13:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2c84a0cef86b825298dd7dcbb3e5f090b732d1fa2432f1f461b179af31b29e`  
		Last Modified: Fri, 22 Nov 2019 22:13:47 GMT  
		Size: 19.1 MB (19111783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b85d477651158904ea8f20a72df0061b4d4f826bb5400a41690023afe75b209`  
		Last Modified: Fri, 22 Nov 2019 22:13:42 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f0906bfeac3fefec7a769654840d45ec2f3b82f66e18c4bdab5ece88ef11c3`  
		Last Modified: Fri, 22 Nov 2019 22:13:41 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9331888ab57ed163878952305eab755ff139908ee33b8d8f0715ee86b215cba`  
		Last Modified: Fri, 22 Nov 2019 22:15:08 GMT  
		Size: 12.4 MB (12432514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31895e53bba016ce55d5e748d9e33ab9096585f58a7cfd751db07b463a4e42d7`  
		Last Modified: Fri, 22 Nov 2019 22:15:06 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8b52e099cd8843ef34d1b5a02002e2a3c5e09635a9f7724e23da1446321563`  
		Last Modified: Fri, 22 Nov 2019 22:15:11 GMT  
		Size: 14.4 MB (14385312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07cf0cef349a0437fda2b7a316738e6a68c72bca472dfef02feecda914c4f6fc`  
		Last Modified: Fri, 06 Dec 2019 00:47:15 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4379da8c3ccb793af4a6f75557830b402a6d2201b1a2e5b570c9810ca70dfd95`  
		Last Modified: Fri, 06 Dec 2019 00:47:14 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8428e1e80ba1c81db88862808880cb19c6cd8e3e99d04bbba2365d165469e468`  
		Last Modified: Fri, 06 Dec 2019 00:47:14 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012d479fe93ca34409aabfc7561842475c9dc87cf9393274b030bc05ad8bf6fb`  
		Last Modified: Fri, 06 Dec 2019 00:47:14 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ffbb86bee017c6c93f8f07194c3bb23b9fc81eb7f4e1b98fb7ea8394ab93bc1`  
		Last Modified: Fri, 06 Dec 2019 02:56:37 GMT  
		Size: 17.0 MB (17016192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a56a9c57f08937796d2a5e0b3f95fe6f09e8e0640e18e698af11a006d001e6c`  
		Last Modified: Fri, 06 Dec 2019 02:56:34 GMT  
		Size: 8.8 MB (8798211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39fc15636fe7542e09603e607a0043c5284aeb9d550b4d00150f95a23fdfc1b0`  
		Last Modified: Fri, 06 Dec 2019 02:56:29 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6f9e9941ef815d270369f64b021e92e5da01f7488c4ba6262ae88f4eb6affd`  
		Last Modified: Fri, 06 Dec 2019 02:56:29 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8515bc0928368db05f730482931cb3aa59086adf18d689b2f6981ef20badff32`  
		Last Modified: Fri, 06 Dec 2019 02:56:29 GMT  
		Size: 19.5 KB (19476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8353441fcb432b89da83ae22cd3edf0591c738cc11567314de6713d15bf98f6e`  
		Last Modified: Fri, 06 Dec 2019 02:56:35 GMT  
		Size: 12.2 MB (12209322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1087e71077bbe99c93ff1f6376b6a9829242ca5858acee9cea36ce958d46ca`  
		Last Modified: Fri, 06 Dec 2019 02:56:30 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-apache` - linux; ppc64le

```console
$ docker pull wordpress@sha256:5dbe72623ee41d5a78fd241079aff34906d5acf2f0b105287ccf04a5502fe3ec
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.2 MB (199210547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f224d3325bdf7519bf56eab9bb74a34bda5b4c20612b97ee0d8f123823ac1c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:33 GMT
ADD file:56ee7f5cc8715d22f4efb9ec5b1c24fac7fdf8f6dc9c07c45625c4f89bdccac3 in / 
# Fri, 22 Nov 2019 14:55:37 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 15:54:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 15:54:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 15:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 15:56:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 15:56:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 16:01:54 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 22 Nov 2019 16:01:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 22 Nov 2019 16:02:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 22 Nov 2019 16:02:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 22 Nov 2019 16:02:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 22 Nov 2019 16:02:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 22 Nov 2019 16:02:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 22 Nov 2019 16:02:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 16:02:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 16:03:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 16:25:40 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 22 Nov 2019 16:25:42 GMT
ENV PHP_VERSION=7.3.12
# Fri, 22 Nov 2019 16:25:44 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.12.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.12.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 16:25:46 GMT
ENV PHP_SHA256=aafe5e9861ad828860c6af8c88cdc1488314785962328eb1783607c1fdd855df PHP_MD5=
# Fri, 22 Nov 2019 16:26:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 22 Nov 2019 16:26:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 16:31:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:23:37 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:23:42 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:23:47 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 06 Dec 2019 01:23:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:23:51 GMT
STOPSIGNAL SIGWINCH
# Fri, 06 Dec 2019 01:23:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:23:55 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:23:58 GMT
EXPOSE 80
# Fri, 06 Dec 2019 01:24:02 GMT
CMD ["apache2-foreground"]
# Fri, 06 Dec 2019 05:23:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 05:33:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 05:33:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 05:33:46 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 05:33:51 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 06 Dec 2019 05:33:54 GMT
VOLUME [/var/www/html]
# Fri, 06 Dec 2019 05:33:56 GMT
ENV WORDPRESS_VERSION=5.3
# Fri, 06 Dec 2019 05:33:58 GMT
ENV WORDPRESS_SHA1=e3edcb1131e539c2b2e10fed37f8b6683c824a98
# Fri, 06 Dec 2019 05:34:06 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 06 Dec 2019 05:34:07 GMT
COPY file:2413d0c63f9d7b1d114697b18317719a02eadaaa61fc5d0c1edd96c027bc57a4 in /usr/local/bin/ 
# Fri, 06 Dec 2019 05:34:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Dec 2019 05:34:12 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e190211f5678d77388755410611e5e6a755e195e7a1096473c675edc074a2389`  
		Last Modified: Fri, 22 Nov 2019 15:04:10 GMT  
		Size: 30.5 MB (30517327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2a4c8dd52eee84e0b2c048f8db6f8de263a31df8647418e2ff962d839741d`  
		Last Modified: Fri, 22 Nov 2019 18:52:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956265206842c78209185fe0d49498b925db99ec94ffa6658904bc0ac86171e3`  
		Last Modified: Fri, 22 Nov 2019 18:52:54 GMT  
		Size: 82.3 MB (82259548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922b0fcf8aed82cfcadde2a647ede9cae5dce14ec49dfb88d8885bbcef8b152a`  
		Last Modified: Fri, 22 Nov 2019 18:52:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c6bab88fcfc3d206f5d61512f6c8c2453e1f98b4a91ab6b4ef126192a1285`  
		Last Modified: Fri, 22 Nov 2019 18:53:49 GMT  
		Size: 19.8 MB (19811357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5a8529cb1520d100497f552f66c6e37da1220f8b2c02f1d727280599d6d430`  
		Last Modified: Fri, 22 Nov 2019 18:53:38 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f5924457d0781761e0005a01b80ea63b3a81533c91bea7f22cf217df1af323`  
		Last Modified: Fri, 22 Nov 2019 18:53:38 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72154f1be4192813b08b36ec288efd330999739167a781bbb6a47156a3c27370`  
		Last Modified: Fri, 22 Nov 2019 18:56:38 GMT  
		Size: 12.4 MB (12433070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f9a010ceb39c6ddd9ff7fb711adf48d316c2af0c62d359e661ed905ed17211`  
		Last Modified: Fri, 22 Nov 2019 18:56:36 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abe6899dfeb483c711720797053848f3f05a74dcba596bf66a243e4de11f6dd`  
		Last Modified: Fri, 22 Nov 2019 18:56:40 GMT  
		Size: 15.1 MB (15113690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0494032c8a3cdcb98695327b8f463564b2c665d83b39f08e1a79ff7f19863303`  
		Last Modified: Fri, 06 Dec 2019 01:42:37 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9098ebd0ee660729dfb2085986c5a377af60bba77dc962a121e8480619c00f`  
		Last Modified: Fri, 06 Dec 2019 01:42:37 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7ff66fec04e3097235b71c98b1f2b46cb7151df3baaf14ca8ad37626259e38`  
		Last Modified: Fri, 06 Dec 2019 01:42:37 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c0f2e6f3d4de7888c69c7bfa6c3dbc0580de5efe9264eaf42ffecb2e5e5dbe`  
		Last Modified: Fri, 06 Dec 2019 01:42:37 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ada2b700abdf3b00647304045727f5257c34a65fbdf205c9ab2a36ad9d0047`  
		Last Modified: Fri, 06 Dec 2019 06:29:14 GMT  
		Size: 17.5 MB (17450442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3b717f5ffb438382258eaa37d172e72ae8bd7f1dbe076867a540646c242fd0`  
		Last Modified: Fri, 06 Dec 2019 06:29:07 GMT  
		Size: 9.4 MB (9386110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681419fce87b899337de0406dc8a71264b00002e4faac126d1900121642e10bb`  
		Last Modified: Fri, 06 Dec 2019 06:28:57 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596b4c4337fb4a8df4cada81fdaaaf01988b47f49fe7c397e790cdab6eca98d7`  
		Last Modified: Fri, 06 Dec 2019 06:28:57 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2a7b6ae264b6cbb678033d7b253045a352aae752c9afa61a4938bbfb11e973`  
		Last Modified: Fri, 06 Dec 2019 06:28:57 GMT  
		Size: 19.5 KB (19488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e33f51967fb0b7cf068266bba39cf9135f49bec7278961765f00eb727d478f`  
		Last Modified: Fri, 06 Dec 2019 06:29:07 GMT  
		Size: 12.2 MB (12209322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f52af599852b38bd6bd722bc234a9aeaa9d6291560cc2195c12649de3910454`  
		Last Modified: Fri, 06 Dec 2019 06:28:57 GMT  
		Size: 3.9 KB (3899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
