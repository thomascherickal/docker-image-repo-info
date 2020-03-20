## `wordpress:5-php7.2-apache`

```console
$ docker pull wordpress@sha256:7ac666bbd91a137b2e0ecadc0fc01edab2519d781deb5f0e314c51ce15aa0133
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `wordpress:5-php7.2-apache` - linux; amd64

```console
$ docker pull wordpress@sha256:73d94a93f1fef9320953627f67d99ad78855a3832c81e79adca38d083f2b2c85
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.4 MB (187356309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc9201cb2a320a6700926e0ea3b5a8e1abacb375c8d06cbe4732cafdd61c9b59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:59:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 11:59:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:59:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 11:59:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 12:07:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Feb 2020 12:07:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Feb 2020 12:07:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Feb 2020 12:07:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Feb 2020 12:07:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Feb 2020 12:07:27 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 26 Feb 2020 12:07:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 26 Feb 2020 12:07:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 12:07:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 12:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 13:28:07 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 20 Mar 2020 01:27:54 GMT
ENV PHP_VERSION=7.2.29
# Fri, 20 Mar 2020 01:27:55 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.29.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.29.tar.xz.asc/from/this/mirror
# Fri, 20 Mar 2020 01:27:55 GMT
ENV PHP_SHA256=b117de74136bf4b439d663be9cf0c8e06a260c1f340f6b75ccadb609153a7fe8 PHP_MD5=
# Fri, 20 Mar 2020 01:28:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 01:28:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 20 Mar 2020 01:33:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 20 Mar 2020 01:33:56 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 20 Mar 2020 01:33:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 20 Mar 2020 01:33:57 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 20 Mar 2020 01:33:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 20 Mar 2020 01:33:58 GMT
STOPSIGNAL SIGWINCH
# Fri, 20 Mar 2020 01:33:58 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 20 Mar 2020 01:33:58 GMT
WORKDIR /var/www/html
# Fri, 20 Mar 2020 01:33:58 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:33:58 GMT
CMD ["apache2-foreground"]
# Fri, 20 Mar 2020 05:38:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:40:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:40:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 05:40:41 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 05:40:42 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 20 Mar 2020 05:40:43 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 05:40:43 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 05:40:43 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 05:40:52 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 05:40:52 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 05:40:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 05:40:52 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2a5d8fa5852468a297ff0881d1804da6f72f49f9307031dfeff2602022170d`  
		Last Modified: Wed, 26 Feb 2020 14:14:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d59ec4ae241b4fb63be2a1f6852dad2846c086b03d4335ed97e812f74698b84`  
		Last Modified: Wed, 26 Feb 2020 14:14:21 GMT  
		Size: 76.7 MB (76651455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42331ef4d446806549ef08fef2deaf4f9297cb292ffab7e2c127f5f73a98bce`  
		Last Modified: Wed, 26 Feb 2020 14:14:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:408b7b7ee112e80a519e6c56b225149858651768f402a4f081f3848f6219ae28`  
		Last Modified: Wed, 26 Feb 2020 14:14:41 GMT  
		Size: 18.7 MB (18675660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570cd47896d53252df21a7a828e45593bd1f6d12af51de544e1525e6a5b304ce`  
		Last Modified: Wed, 26 Feb 2020 14:14:36 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2419413b2a166ee6840435bf1cbaa81866de4ca976fe0637efe6f4ac1e9df275`  
		Last Modified: Wed, 26 Feb 2020 14:14:36 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:912711f6b2eb42fe0e6ae39be2049e96312c4237f64274d1598fd5889bb8ea82`  
		Last Modified: Fri, 20 Mar 2020 03:22:13 GMT  
		Size: 12.6 MB (12646614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f800a8d50dc1eb4f98cca550f238061fac3db13f38a2122c02e74b80bdb05222`  
		Last Modified: Fri, 20 Mar 2020 03:22:11 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060632780c840891965b65b82fe9fda2c2668bc88d75241da5f7cb0f690ba765`  
		Last Modified: Fri, 20 Mar 2020 03:22:15 GMT  
		Size: 13.8 MB (13842125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a05acdedc4e8dd9cae322948b2fbe1c648c75259d729784f6665a307eb741`  
		Last Modified: Fri, 20 Mar 2020 03:22:10 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cd5023146c243b780eed227b956f986c1f0349b0fccc36520520eb88f2cecb`  
		Last Modified: Fri, 20 Mar 2020 03:22:10 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b64119066d1c09788ebf0740d9fb2ef1a16c818ec41ce9f04594031bec23b5e`  
		Last Modified: Fri, 20 Mar 2020 03:22:10 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2dde7ae0cf1fa9f744960f6f637cec7c24f56db22aa3851e96138754c7326a`  
		Last Modified: Fri, 20 Mar 2020 03:22:11 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515beb53efc1b5418b924ba235b59fda4c14f4121adb19fa088de35da64d6a35`  
		Last Modified: Fri, 20 Mar 2020 06:00:26 GMT  
		Size: 16.7 MB (16704518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c4f01de4ae36659e2416a48bff296c90e5c7f886d057639013ba8048b4390c`  
		Last Modified: Fri, 20 Mar 2020 06:00:24 GMT  
		Size: 9.5 MB (9486710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffff94c1270ff3bf9918655eb70f379f4c4857b23baa3b847d9523d694ff14a`  
		Last Modified: Fri, 20 Mar 2020 06:00:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b8bbe6783dc25d372abe134093a47d949f61a83b3b1a3c1428232250d30892`  
		Last Modified: Fri, 20 Mar 2020 06:00:20 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d26c1e77e3ea6717421bc087792bdc05ddf4ddcacdac6a8014f20bd123ede`  
		Last Modified: Fri, 20 Mar 2020 06:00:21 GMT  
		Size: 19.5 KB (19479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58ddfd579c51b203b25a577addb711fe75e0ebbfda7234e35e7d8275a97fe2a`  
		Last Modified: Fri, 20 Mar 2020 06:00:24 GMT  
		Size: 12.2 MB (12227873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6141cb1995b3d32882f8e55abde031112bf6ea3099d6a51fc172979ad83d20`  
		Last Modified: Fri, 20 Mar 2020 06:00:21 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.2-apache` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:77a007db8d106bbf7595613011fc7e05d7a09a761a610faf3d9a11b6656a20d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.1 MB (164109494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:785ed0a12f27e1ae4578dd823b214a172f81a9b1da1c192bcdc8cf440092be5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:32:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 04:32:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 04:33:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:33:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 04:33:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 04:38:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Feb 2020 04:38:03 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Feb 2020 04:38:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Feb 2020 04:38:34 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Feb 2020 04:38:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Feb 2020 04:38:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 26 Feb 2020 04:38:40 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 26 Feb 2020 04:38:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 04:38:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 04:38:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 05:33:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 19 Mar 2020 23:03:20 GMT
ENV PHP_VERSION=7.2.29
# Thu, 19 Mar 2020 23:03:21 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.29.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.29.tar.xz.asc/from/this/mirror
# Thu, 19 Mar 2020 23:03:23 GMT
ENV PHP_SHA256=b117de74136bf4b439d663be9cf0c8e06a260c1f340f6b75ccadb609153a7fe8 PHP_MD5=
# Thu, 19 Mar 2020 23:03:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Mar 2020 23:03:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:07:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Mar 2020 23:07:47 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:07:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Mar 2020 23:07:52 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 19 Mar 2020 23:07:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Mar 2020 23:07:54 GMT
STOPSIGNAL SIGWINCH
# Thu, 19 Mar 2020 23:07:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:07:56 GMT
WORKDIR /var/www/html
# Thu, 19 Mar 2020 23:07:57 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:07:58 GMT
CMD ["apache2-foreground"]
# Fri, 20 Mar 2020 02:45:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 02:50:18 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 02:50:26 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 02:50:31 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 02:50:39 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 20 Mar 2020 02:50:43 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 02:50:47 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 02:50:49 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 02:51:03 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 02:51:06 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 02:51:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 02:51:12 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d924f652197b083a9a110930b7548ba9fe1fcc87e963cd10516dd54b172a9804`  
		Last Modified: Wed, 26 Feb 2020 06:04:05 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd86ee1863629868607b0a8c088897c302f5f1e23d0bd51a610f0d5aae26bdcf`  
		Last Modified: Wed, 26 Feb 2020 06:04:26 GMT  
		Size: 58.8 MB (58799831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e751ab6d9f11edd9376e6fa63465ad0c6a006fc52c130bdf4f5b8ff05ffe936`  
		Last Modified: Wed, 26 Feb 2020 06:04:04 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29c6f074c8b56a4ced1fc26a03ebbaf23a55333eafec2cc5bfe35d18b28d508`  
		Last Modified: Wed, 26 Feb 2020 06:04:59 GMT  
		Size: 18.0 MB (18024359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c312669fae45780587f8489022310772f13d0279f13e1e169b91bac753d015`  
		Last Modified: Wed, 26 Feb 2020 06:04:53 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349ecc709c43cc8747f1d8ad4b055f5bece773687c9ec100f662d8e872681ff4`  
		Last Modified: Wed, 26 Feb 2020 06:04:53 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd4aa871ac78448b1239ae49ebaf6b83e60f3f651c59b110e7c99baef60b1f1`  
		Last Modified: Thu, 19 Mar 2020 23:44:45 GMT  
		Size: 12.6 MB (12644402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ec6c8dcb630a125494c79ae4ddb0f1d191794287f6d2569f60f4e727d3b326`  
		Last Modified: Thu, 19 Mar 2020 23:44:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3b680bf565379507a4d41f60b538ee7fc31095beaff8f184aa3c862d394e6e`  
		Last Modified: Thu, 19 Mar 2020 23:44:46 GMT  
		Size: 12.9 MB (12920546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b43915bb3e73953f42b6ed335344e4131c733c0ba348d2320bc16e31bf1b14`  
		Last Modified: Thu, 19 Mar 2020 23:44:41 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad8e312add2edca7dd963dab263edeec558d2c7ba4b241118d43b75f995de73`  
		Last Modified: Thu, 19 Mar 2020 23:44:42 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d0a1c5223a7475566022090117e58ba6c74615e00b5b14dce3df80b12908dd`  
		Last Modified: Thu, 19 Mar 2020 23:44:41 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6cd5286366ece5007e033beaba85d2a597f10b70026c4299a985c0ceab5467`  
		Last Modified: Thu, 19 Mar 2020 23:44:41 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d870a7c66cdca4d9e0c2ba1ed767b60d45f2bbef6b55466b4cb5e7ced1eb9eb9`  
		Last Modified: Fri, 20 Mar 2020 03:23:20 GMT  
		Size: 16.3 MB (16279479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ab758f21f29438ae52222cc6532888a89c10266a4a0df718b40d3db20950c8`  
		Last Modified: Fri, 20 Mar 2020 03:23:16 GMT  
		Size: 8.4 MB (8353056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e22a2bd1777325a9dd8924ed161417b86fc1111b373ee884e2b551c6c00104`  
		Last Modified: Fri, 20 Mar 2020 03:23:11 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fd9950f0eb47852a6305e7e8588f60f199fc2ac91e4ac7a2906c89479aaafd`  
		Last Modified: Fri, 20 Mar 2020 03:23:11 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e329ef56eed209bc17f7c8f1f2dac67f7817b62f3291750abfb947aa23e5b427`  
		Last Modified: Fri, 20 Mar 2020 03:23:11 GMT  
		Size: 19.5 KB (19477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a0952161e887e51328696b8f7187e8cbf40a8c059d6fdc6100ba4753e29cfb`  
		Last Modified: Fri, 20 Mar 2020 03:23:17 GMT  
		Size: 12.2 MB (12227880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc7d2fcd140736ac16493f46e5170abbe4d24f9f5a8f468104cc3bd1efc4a0c`  
		Last Modified: Fri, 20 Mar 2020 03:23:11 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.2-apache` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:c5c1ff967f6ab393784fd9c30f507cc1c04a82914327f69839664fa4191a39c0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160142980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa01a9324e3a52092a0a92d202aaf90201e0a1e0353c66cbb65ba812bb894910`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:11 GMT
ADD file:2488038744e2e15217e67dd7f4bec5dcc7e9abe8a1010fe720a5ba7cbe7ab0eb in / 
# Wed, 26 Feb 2020 00:52:13 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:27:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 14:27:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 14:27:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:27:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 14:28:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 14:31:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Feb 2020 14:31:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Feb 2020 14:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Feb 2020 14:32:10 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Feb 2020 14:32:13 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Feb 2020 14:32:15 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 26 Feb 2020 14:32:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 26 Feb 2020 14:32:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 14:32:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 14:32:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 15:25:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 19 Mar 2020 23:39:07 GMT
ENV PHP_VERSION=7.2.29
# Thu, 19 Mar 2020 23:39:08 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.29.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.29.tar.xz.asc/from/this/mirror
# Thu, 19 Mar 2020 23:39:09 GMT
ENV PHP_SHA256=b117de74136bf4b439d663be9cf0c8e06a260c1f340f6b75ccadb609153a7fe8 PHP_MD5=
# Thu, 19 Mar 2020 23:39:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Mar 2020 23:39:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Mar 2020 23:43:04 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:43:06 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Mar 2020 23:43:08 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 19 Mar 2020 23:43:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Mar 2020 23:43:09 GMT
STOPSIGNAL SIGWINCH
# Thu, 19 Mar 2020 23:43:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:43:10 GMT
WORKDIR /var/www/html
# Thu, 19 Mar 2020 23:43:11 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:43:11 GMT
CMD ["apache2-foreground"]
# Fri, 20 Mar 2020 05:35:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:38:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:38:43 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 05:38:46 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 05:38:49 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 20 Mar 2020 05:38:50 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 05:38:51 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 05:38:52 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 05:38:58 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 05:39:01 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 05:39:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 05:39:03 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:fff3167bf8c79dc08baf67eb607823aadcbee2033f9620cc502e2c49423f605b`  
		Last Modified: Wed, 26 Feb 2020 01:07:32 GMT  
		Size: 22.7 MB (22699783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cd5cd61b6f8de3cb9b8eaf9920ee92db196f4c73365a731f08c51fdec97be4`  
		Last Modified: Wed, 26 Feb 2020 15:55:26 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b7e5098979c0c6921b0ba0a8f1e1625ffe7a6f8b565feae67a7a293e74e9db`  
		Last Modified: Wed, 26 Feb 2020 15:55:46 GMT  
		Size: 59.5 MB (59501205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2e6e500bc14a91c0e209ad61d4cab4947d2f99c2be6908475b8c3d61189f25`  
		Last Modified: Wed, 26 Feb 2020 15:55:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96129b300ee13117f2e91bbbeb1b1c0f050ff559195f3868d9dea095e9cc0040`  
		Last Modified: Wed, 26 Feb 2020 15:56:21 GMT  
		Size: 17.5 MB (17482498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9609adc074bde9ab5e5e3e4ad529f15389d8713a0e08d313f25bb5b6728d477e`  
		Last Modified: Wed, 26 Feb 2020 15:56:16 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c123cbb02068e03e45997be8582ae08b24d8ff8ec2716c611db76465f9c1d46`  
		Last Modified: Wed, 26 Feb 2020 15:56:16 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1cefa35dce57c6f2b7dfbb43793c9bfc6796fbc68c1ac150c234f02099d023`  
		Last Modified: Fri, 20 Mar 2020 00:44:44 GMT  
		Size: 12.6 MB (12644397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6992bd8afb72adf1acb0eedb8c0d8bdccb8cc723d042d5b7ffd325fce10591`  
		Last Modified: Fri, 20 Mar 2020 00:44:42 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7999bce9db2e76322b20317512313f45543ec63139b601662158f5edf1d5fd4`  
		Last Modified: Fri, 20 Mar 2020 00:44:45 GMT  
		Size: 12.2 MB (12188333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39256ff231e0f4026a4df2dbce7939baddcfee971089cb8b167ad9a668f9c103`  
		Last Modified: Fri, 20 Mar 2020 00:44:40 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e45f1d97ae0136de028dd570b65c223ef8d23dcf6ead3ac3f278a033427d30`  
		Last Modified: Fri, 20 Mar 2020 00:44:40 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac4975ba5c1a566696ab983b000e1b1b801848b4c3a4ad7caab288660d6015d`  
		Last Modified: Fri, 20 Mar 2020 00:44:41 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae5ae9e20ea0cfff97242b58fa5fa4a8627a99a05f795abe5e271e7358a5723`  
		Last Modified: Fri, 20 Mar 2020 00:44:40 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f8c85370365b28e0129b09709a32b23d0bc831b753381dde6cb6e58140e283`  
		Last Modified: Fri, 20 Mar 2020 06:10:20 GMT  
		Size: 15.9 MB (15854928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3536c09c410f71644893453cd9ccecdb000b7b9bb52cce99cf0d4d4d5337e6ca`  
		Last Modified: Fri, 20 Mar 2020 06:10:17 GMT  
		Size: 7.5 MB (7514290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7834bc7d9794ad095e9235f583e48037c0ffa71aea871587fe75fc632e368dc9`  
		Last Modified: Fri, 20 Mar 2020 06:10:13 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78dcd8b1df29e615087ae9847edc1093f3f19ea9ab2b253d5c7a675c33613ba1`  
		Last Modified: Fri, 20 Mar 2020 06:10:13 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca5a604f51bea55d9fb0b34d8fe12ac981b9194e573eb278fe62a8a7dcab9df`  
		Last Modified: Fri, 20 Mar 2020 06:10:12 GMT  
		Size: 19.5 KB (19485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5712f567c51554730f5b04f99db4d4bf4d0c403e15f08d65e8faf18a422f8e1e`  
		Last Modified: Fri, 20 Mar 2020 06:10:18 GMT  
		Size: 12.2 MB (12227877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1df556945eba387f5356d3c234f4da36f7d612e5bffedc27a8eeff141e405f6`  
		Last Modified: Fri, 20 Mar 2020 06:10:13 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.2-apache` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:f49df36f435a5e8ede76b7a7d8ec0a55d823e40c5878e217fa86c403d669bda4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.7 MB (177749585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f94cf9616e6cf321e14558bff94824ddc60dad58cd5cdda06c01df44d42cacba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:55:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 11:55:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 11:56:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:56:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 11:56:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 12:00:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Feb 2020 12:00:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Feb 2020 12:00:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Feb 2020 12:00:37 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Feb 2020 12:00:42 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Feb 2020 12:00:43 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 26 Feb 2020 12:00:45 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 26 Feb 2020 12:00:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 12:00:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 12:00:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 12:55:15 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 19 Mar 2020 23:48:34 GMT
ENV PHP_VERSION=7.2.29
# Thu, 19 Mar 2020 23:48:35 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.29.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.29.tar.xz.asc/from/this/mirror
# Thu, 19 Mar 2020 23:48:36 GMT
ENV PHP_SHA256=b117de74136bf4b439d663be9cf0c8e06a260c1f340f6b75ccadb609153a7fe8 PHP_MD5=
# Thu, 19 Mar 2020 23:48:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Mar 2020 23:48:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:52:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Mar 2020 23:52:32 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:52:37 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Mar 2020 23:52:41 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 19 Mar 2020 23:52:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Mar 2020 23:52:46 GMT
STOPSIGNAL SIGWINCH
# Thu, 19 Mar 2020 23:52:46 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:52:47 GMT
WORKDIR /var/www/html
# Thu, 19 Mar 2020 23:52:48 GMT
EXPOSE 80
# Thu, 19 Mar 2020 23:52:49 GMT
CMD ["apache2-foreground"]
# Fri, 20 Mar 2020 05:15:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:18:57 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:19:00 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 05:19:02 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 05:19:06 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 20 Mar 2020 05:19:08 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 05:19:09 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 05:19:10 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 05:19:17 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 05:19:18 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 05:19:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 05:19:20 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe4ded10aa84b08ce645b2a064c692746e119bd7bdbeb50d004635ceec99237`  
		Last Modified: Wed, 26 Feb 2020 13:27:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a0cd710bad4e7ac9d5be343f0970fef306eeb91d1a80f7ad1849724764c4bc`  
		Last Modified: Wed, 26 Feb 2020 13:27:20 GMT  
		Size: 70.3 MB (70334994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4988beed3268a0092cad73bf3915a3dd39e2d730a4d549bb9c333b6bcc9cba6`  
		Last Modified: Wed, 26 Feb 2020 13:27:02 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc30c8501c0e3a4b5a426b2a6c45f8983ada2b381ad4d0a04176bde5e40fba47`  
		Last Modified: Wed, 26 Feb 2020 13:27:52 GMT  
		Size: 18.6 MB (18577731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b336db5f954338dd131a8f39e8ab21b9fc15388d0a0a55810c6189bc630eff50`  
		Last Modified: Wed, 26 Feb 2020 13:27:48 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebc6705a5b21871b470803bcf2ecb06da02f9567cf7399546bfd562e3e587397`  
		Last Modified: Wed, 26 Feb 2020 13:27:47 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26e077f67d612e39e85704cd85e06e76c478fe39ba438e999b980a62ea1e367`  
		Last Modified: Fri, 20 Mar 2020 00:57:19 GMT  
		Size: 12.6 MB (12645284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9430b6c2a0099f83def8648951b8c2de1ffd3e13adda6e9f2763380f4940141d`  
		Last Modified: Fri, 20 Mar 2020 00:57:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775f2840c46c8ef1b5f1a87c095611695aabd84498daa8ad48b98cbeb61ac8a4`  
		Last Modified: Fri, 20 Mar 2020 00:57:15 GMT  
		Size: 13.5 MB (13537657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719d5246982b9758c4ab72c65119b9f46d3f9e870222b3d98c244da5853ef5a2`  
		Last Modified: Fri, 20 Mar 2020 00:57:11 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9096fdd66ddccfe0c5d790c55c9c1763b3c87917b2ec52c7a940cd67498809eb`  
		Last Modified: Fri, 20 Mar 2020 00:57:11 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894a2408564bd90f1bf030b06de3793bbb6473b9d546d0cd55f4a35be788b6e1`  
		Last Modified: Fri, 20 Mar 2020 00:57:11 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843d5c7c90f8bc40502f81d7a4995148b7ef83cfe6fbeea1935dc88d2cd3184e`  
		Last Modified: Fri, 20 Mar 2020 00:57:12 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a898a7f9d65f398950ebff2254d739bbf1fb705aa9d8d623b0faaa8fe877b94`  
		Last Modified: Fri, 20 Mar 2020 05:51:51 GMT  
		Size: 16.6 MB (16648695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616697e7015de54934df556d463c6d1407056aa6148098639dde07eac8a4b321`  
		Last Modified: Fri, 20 Mar 2020 05:51:47 GMT  
		Size: 7.9 MB (7896115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43635b9e84c897c63320bb0c31c81717978ac6e65b920b82ac1f16f679f42887`  
		Last Modified: Fri, 20 Mar 2020 05:51:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3b7b223bc1055a9ec5cf341f0df3d5443015ea43cfc4dd9045df6db4df724`  
		Last Modified: Fri, 20 Mar 2020 05:51:44 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be549e8387812c9c0f27ab44f78def65b27845a94e8333e0c284b7b411a4e757`  
		Last Modified: Fri, 20 Mar 2020 05:51:44 GMT  
		Size: 19.5 KB (19486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6f7d38963f314e216885c5a835dfa3125cca1ed5d9a80d90535f1e440a1aec`  
		Last Modified: Fri, 20 Mar 2020 05:51:49 GMT  
		Size: 12.2 MB (12227876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6f94587e5707e49efd8599a303cf4d3e24cdba810cb6c171b1dff67a210669`  
		Last Modified: Fri, 20 Mar 2020 05:51:44 GMT  
		Size: 3.9 KB (3893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.2-apache` - linux; 386

```console
$ docker pull wordpress@sha256:d4c781191a2afec5126e17df60f8d862686ba5f944b21c5b8bb64079acbb50df
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.9 MB (192881008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:541bb58447fde731220f3fffacbecf22f7cb9420aa7194b095dc7c8571a4f4dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 17:09:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 17:09:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 17:10:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:10:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 17:10:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 17:17:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Feb 2020 17:17:15 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Feb 2020 17:17:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Feb 2020 17:17:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Feb 2020 17:17:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Feb 2020 17:17:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 26 Feb 2020 17:17:30 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 26 Feb 2020 17:17:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 17:17:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 17:17:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 18:33:01 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 20 Mar 2020 01:43:50 GMT
ENV PHP_VERSION=7.2.29
# Fri, 20 Mar 2020 01:43:50 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.29.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.29.tar.xz.asc/from/this/mirror
# Fri, 20 Mar 2020 01:43:51 GMT
ENV PHP_SHA256=b117de74136bf4b439d663be9cf0c8e06a260c1f340f6b75ccadb609153a7fe8 PHP_MD5=
# Fri, 20 Mar 2020 01:44:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 01:44:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 20 Mar 2020 01:50:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 20 Mar 2020 01:50:07 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 20 Mar 2020 01:50:07 GMT
RUN docker-php-ext-enable sodium
# Fri, 20 Mar 2020 01:50:08 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 20 Mar 2020 01:50:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 20 Mar 2020 01:50:09 GMT
STOPSIGNAL SIGWINCH
# Fri, 20 Mar 2020 01:50:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 20 Mar 2020 01:50:09 GMT
WORKDIR /var/www/html
# Fri, 20 Mar 2020 01:50:09 GMT
EXPOSE 80
# Fri, 20 Mar 2020 01:50:10 GMT
CMD ["apache2-foreground"]
# Fri, 20 Mar 2020 05:48:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:50:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:50:49 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 05:50:50 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 05:50:50 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 20 Mar 2020 05:50:51 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 05:50:51 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 05:50:51 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 05:51:00 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 05:51:01 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 05:51:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 05:51:01 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63da883d1acf485a7b1cc92daec610b51a3619bad1c74646d2349d702e66678`  
		Last Modified: Wed, 26 Feb 2020 19:26:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6194ab862f4a0b8d6069fe53227b0a99ede3c9572bdd3a7a53f1c345933b00e`  
		Last Modified: Wed, 26 Feb 2020 19:27:12 GMT  
		Size: 81.2 MB (81198469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3174e482c145c56e48af068bfededb0f4176a4d233274aba6343c48fb2a056`  
		Last Modified: Wed, 26 Feb 2020 19:26:48 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb27e395c764f0a3f9ca49eef31ccb24f7377992fcad9029712199a1d534f6b1`  
		Last Modified: Wed, 26 Feb 2020 19:27:37 GMT  
		Size: 19.1 MB (19111905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d40ce7d32639c19d1581dd9c9188e567ef2cee34ea4b58599f1af4176db1ad`  
		Last Modified: Wed, 26 Feb 2020 19:27:31 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6162014f44f172cc8fc99b9f701119b8a665a64373699f9fcbde48f91d0a5e`  
		Last Modified: Wed, 26 Feb 2020 19:27:31 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb99561799f9adf32f7553e7fb1ac6ebb5f8043d84764d92ac9a0713fa2e2fcc`  
		Last Modified: Fri, 20 Mar 2020 03:42:16 GMT  
		Size: 12.6 MB (12645813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0095e4d6173b3366ed152d5cd3ebbeabcb921caed94ef1c296a232a759968ec9`  
		Last Modified: Fri, 20 Mar 2020 03:42:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1989449df345af348f62bba27379b12af23df3d4254048a799e37e67234c3a`  
		Last Modified: Fri, 20 Mar 2020 03:42:18 GMT  
		Size: 14.2 MB (14168968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d010cce2369cdcaf308f3cc1e4e27e4bf7723758333173bb1ef12f414b77b2`  
		Last Modified: Fri, 20 Mar 2020 03:42:13 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe6ab864ce7b12c1cf91acee49ae2047fa231409abfbaa9fda5ec96095540f4`  
		Last Modified: Fri, 20 Mar 2020 03:42:13 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8623a6dec2a2eee1450116ad7094009d6e30d01f396e527748eb28ea76e886`  
		Last Modified: Fri, 20 Mar 2020 03:42:13 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011ecb7c2d6b23b33c5635c246473b7fead474370ec914b8826d48db202f512d`  
		Last Modified: Fri, 20 Mar 2020 03:42:13 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aef9ed7d2e6770a1884bc3fe651e1e2c34ce3204e9b7fc18415cedd66ed9465`  
		Last Modified: Fri, 20 Mar 2020 06:12:08 GMT  
		Size: 17.0 MB (17022442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69851b790a8cb99265697639db2abb8b1de2b1d1e81a99469af65bf66580f515`  
		Last Modified: Fri, 20 Mar 2020 06:12:05 GMT  
		Size: 8.7 MB (8728351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07adaf21a5e628eb4ba348f0dcdc741ee17db0490812b150079690912845434a`  
		Last Modified: Fri, 20 Mar 2020 06:12:00 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d490a44b49d075ed3333a8e678c5102066c29a46330f32e3cac755ad4a43fdcd`  
		Last Modified: Fri, 20 Mar 2020 06:11:59 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cd794d1353fd81120b2e81b08a79165861185cc7b5d62a57a39600fe34cef3`  
		Last Modified: Fri, 20 Mar 2020 06:12:00 GMT  
		Size: 19.5 KB (19476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9aa661028cec7a442c7261a672f9e333bff042b8b23e33e77c01a2dac6aab5d`  
		Last Modified: Fri, 20 Mar 2020 06:12:06 GMT  
		Size: 12.2 MB (12227873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecdd1366887c7f0c0ab44bec286d8fba0ad6634a550a4504cd14136a28c199b`  
		Last Modified: Fri, 20 Mar 2020 06:12:02 GMT  
		Size: 3.9 KB (3889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.2-apache` - linux; ppc64le

```console
$ docker pull wordpress@sha256:358b06cf34208a1684858892076daf22a6263eeab2c5cf97222f0c46829c87b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.2 MB (199179509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2609a8198c95c8194b915cf02e9568d97ed4cacd1f5159beef394746b99deab9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 13:39:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 13:39:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 13:40:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 13:41:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 13:41:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 13:46:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Feb 2020 13:46:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Feb 2020 13:47:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Feb 2020 13:47:40 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Feb 2020 13:47:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Feb 2020 13:47:51 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 26 Feb 2020 13:47:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 26 Feb 2020 13:47:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 13:47:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 13:48:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 15:06:25 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 20 Mar 2020 00:18:16 GMT
ENV PHP_VERSION=7.2.29
# Fri, 20 Mar 2020 00:18:18 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.29.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.29.tar.xz.asc/from/this/mirror
# Fri, 20 Mar 2020 00:18:20 GMT
ENV PHP_SHA256=b117de74136bf4b439d663be9cf0c8e06a260c1f340f6b75ccadb609153a7fe8 PHP_MD5=
# Fri, 20 Mar 2020 00:19:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Mar 2020 00:19:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 20 Mar 2020 00:24:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 20 Mar 2020 00:24:31 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 20 Mar 2020 00:24:42 GMT
RUN docker-php-ext-enable sodium
# Fri, 20 Mar 2020 00:24:57 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 20 Mar 2020 00:25:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 20 Mar 2020 00:25:06 GMT
STOPSIGNAL SIGWINCH
# Fri, 20 Mar 2020 00:25:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 20 Mar 2020 00:25:14 GMT
WORKDIR /var/www/html
# Fri, 20 Mar 2020 00:25:20 GMT
EXPOSE 80
# Fri, 20 Mar 2020 00:25:22 GMT
CMD ["apache2-foreground"]
# Fri, 20 Mar 2020 07:36:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 07:44:37 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 07:44:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 07:44:56 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 07:45:09 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 20 Mar 2020 07:45:15 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 07:45:21 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 07:45:26 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 07:45:39 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 07:45:42 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 07:45:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 07:45:51 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57d9b8bc2eac5c6f4f9993a4c4b7bd08403a98d069eb7b3678d6fe8396f488`  
		Last Modified: Wed, 26 Feb 2020 15:58:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420ef5ae09970b307979254c32570cf02e8b0979b1bc6df0941e38eb670262a5`  
		Last Modified: Wed, 26 Feb 2020 15:59:12 GMT  
		Size: 82.3 MB (82259740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72af4000b0056d6328c78e7b5aa5de14c173ffd361612045bc4e3013bcb0fa8f`  
		Last Modified: Wed, 26 Feb 2020 15:58:44 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13063450f1fae407e2f5dfdaed0b40346c05f6a566b8261e9ec40c87da0a99ec`  
		Last Modified: Wed, 26 Feb 2020 16:00:17 GMT  
		Size: 19.8 MB (19811388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a750c8efaa8db87f2ee0ca169c14c7c764305e2a1f42ea0d221317adba5575a0`  
		Last Modified: Wed, 26 Feb 2020 16:00:05 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97334fa51526e6efd5eb2ef129e6f2af39c1b0d21c418ccf2559d7922a53522`  
		Last Modified: Wed, 26 Feb 2020 16:00:07 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f984ed018c5cac14970fd016d3840e74901b884c6c7b1ceb39376d2543f31acd`  
		Last Modified: Fri, 20 Mar 2020 02:23:49 GMT  
		Size: 12.6 MB (12646276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f4728af6593fb8d9d09984f5fd21d130f38c59c939080060feb16fb08aaa3b`  
		Last Modified: Fri, 20 Mar 2020 02:23:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2292ebedbdf661ab20d071c5a7bf85521aacc3102d0e868cfa1784c1623a151e`  
		Last Modified: Fri, 20 Mar 2020 02:23:47 GMT  
		Size: 14.9 MB (14882934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc8856df249d0ffce0ed98bc59a6cd5f52a81d47577ab30d5842e9219199eb49`  
		Last Modified: Fri, 20 Mar 2020 02:23:41 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828d9b6dfbfbb0fee54dade974f888600aa338f329da9d4d3b4fa361207d2d24`  
		Last Modified: Fri, 20 Mar 2020 02:23:41 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff0102c496ba29837fd36bb8fd7eb8c0deb3f223a35ab9a86ddceed91c65b04`  
		Last Modified: Fri, 20 Mar 2020 02:23:42 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15a9eb2f04e938f3fcadf810d4e6cdffae0c390b10e309798a285ab71df4e03`  
		Last Modified: Fri, 20 Mar 2020 02:23:41 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32611c302028a2213aba9121228b963dfa8c14ac394b92301c76b82c8c8ec3cd`  
		Last Modified: Fri, 20 Mar 2020 09:02:06 GMT  
		Size: 17.5 MB (17455445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dadccefd960504a813cc9ab7339426d27545502460cb8d5c2f919b61d3aa16d2`  
		Last Modified: Fri, 20 Mar 2020 09:02:03 GMT  
		Size: 9.3 MB (9347740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f911ad2bc2393ff1bc716129affa782f98d835a5b12caec25be3ff02b43cbc`  
		Last Modified: Fri, 20 Mar 2020 09:01:58 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1773896e03ca960cd51e0fcda2abd5bc310f63db43baa8d3770eea81cab943`  
		Last Modified: Fri, 20 Mar 2020 09:01:57 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f2bd4e5f3bd3cf1077e1feff20b75939084752af5a8b89bcaa113bc86c7c45`  
		Last Modified: Fri, 20 Mar 2020 09:01:57 GMT  
		Size: 19.5 KB (19492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ded59b4623543e8a626c74fe3583b39472456f19b44b113dd1677edadb567b`  
		Last Modified: Fri, 20 Mar 2020 09:02:01 GMT  
		Size: 12.2 MB (12227878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efe11d5d9d17047c00aa80647d8752ed70ad3befacbee4faa4d20cedd447e72`  
		Last Modified: Fri, 20 Mar 2020 09:01:58 GMT  
		Size: 3.9 KB (3891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
