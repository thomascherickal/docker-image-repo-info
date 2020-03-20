## `yourls:1-apache`

```console
$ docker pull yourls@sha256:5e7244cdf1374ab425f5504ff8f1f3ea9161ba7b0f06d9171ca6c4e6b2b34057
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `yourls:1-apache` - linux; amd64

```console
$ docker pull yourls@sha256:d448fdc100e75b8461ecb2c9ea468398d7cba45deb559d2bc7929ecaa487c0b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.7 MB (151697450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49021aded3bedb7fee2b4351f4af3494a4a57351f79e14f4690c30b14b5dbc2e`
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
# Wed, 26 Feb 2020 13:28:07 GMT
ENV PHP_VERSION=7.2.28
# Wed, 26 Feb 2020 13:28:07 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.28.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.28.tar.xz.asc/from/this/mirror
# Wed, 26 Feb 2020 13:28:07 GMT
ENV PHP_SHA256=afe1863301da572dee2e0bad8014813bcced162f980ddc8ec8e41fd72263eb2d PHP_MD5=
# Wed, 26 Feb 2020 13:28:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Feb 2020 13:28:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Feb 2020 13:32:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 26 Feb 2020 13:32:25 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Wed, 26 Feb 2020 13:32:26 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Feb 2020 13:32:27 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 26 Feb 2020 13:32:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Feb 2020 13:32:27 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Feb 2020 13:32:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Feb 2020 13:32:28 GMT
WORKDIR /var/www/html
# Wed, 26 Feb 2020 13:32:28 GMT
EXPOSE 80
# Wed, 26 Feb 2020 13:32:28 GMT
CMD ["apache2-foreground"]
# Thu, 27 Feb 2020 04:29:20 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 27 Feb 2020 04:29:20 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 27 Feb 2020 04:29:21 GMT
RUN a2enmod rewrite expires
# Thu, 27 Feb 2020 04:29:21 GMT
ENV YOURLS_VERSION=1.7.6
# Thu, 27 Feb 2020 04:29:22 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Thu, 27 Feb 2020 04:29:23 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 27 Feb 2020 04:29:23 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 27 Feb 2020 04:29:24 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 27 Feb 2020 04:29:24 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 27 Feb 2020 04:29:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Feb 2020 04:29:24 GMT
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
	-	`sha256:ece88053da019ccd4a1f142a1a8d1190b4f0d60c90c3ab27e61f26db947955d5`  
		Last Modified: Wed, 26 Feb 2020 14:18:01 GMT  
		Size: 12.7 MB (12650384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2131b538da35b5d922ed61b3fc06567313579fcc407f6ce7dd81888b4299ce2`  
		Last Modified: Wed, 26 Feb 2020 14:18:00 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26c9457b1ed2300f841e0748bba4858a13a2e0b59ed10488bcf02fdac6db93d`  
		Last Modified: Wed, 26 Feb 2020 14:18:02 GMT  
		Size: 13.8 MB (13841761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4ecf09518619aed232d745c7b05f2f99471e25c389cd729a8bf37b6563c0d0`  
		Last Modified: Wed, 26 Feb 2020 14:17:59 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a41f34ff2f01ab7056284c63c8edff70781dce76e719f554b9754625b85c72d`  
		Last Modified: Wed, 26 Feb 2020 14:17:59 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6669ed2ef9ebc8bd17b3b1b33f31ab4221ffa68beab552e3994df52878ca90d`  
		Last Modified: Wed, 26 Feb 2020 14:17:59 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0441670f3790406b187c0d67b266046d96c5069b88f050be7340c5b1d1fff5ef`  
		Last Modified: Wed, 26 Feb 2020 14:17:59 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6750caf73333db498380ccccfd1f2ad26602d420b24b51d7bded24faaf75d`  
		Last Modified: Thu, 27 Feb 2020 04:30:13 GMT  
		Size: 291.7 KB (291680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2cd7865b0319f792b1bd01f97b33aced6d7d31f4d2bc87d57d6fd6436e11b1`  
		Last Modified: Thu, 27 Feb 2020 04:30:13 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89daf489582b2617213ac15387e30da8f02cf97eb30a0ce1b79b3a12b3ad44cd`  
		Last Modified: Thu, 27 Feb 2020 04:30:12 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4112212b0d794df560d7d659f6feb1cb17080a468bbacf41828ba89a94373b2`  
		Last Modified: Thu, 27 Feb 2020 04:30:13 GMT  
		Size: 2.5 MB (2485193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2732fd542476b9f19b925b7f1b4cae26ef32a0d5a74c75838f2c1ef6b8aca24`  
		Last Modified: Thu, 27 Feb 2020 04:30:13 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322d29298b879f25943ef23a3cc9243556d3bf6d892ab6b77797500802659a3e`  
		Last Modified: Thu, 27 Feb 2020 04:30:12 GMT  
		Size: 1.9 KB (1857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029bf62e14d168717cdc5cd1d6d596176f559d85b27cc15e69509bd63a706386`  
		Last Modified: Thu, 27 Feb 2020 04:30:12 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v5

```console
$ docker pull yourls@sha256:5f731c21b4f0da90471d7c111e4496e4489716738182aeccfc1877b9644b8b80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.0 MB (129989279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26c86334c5517776c91653119013c5bff83969890cb6b7e2636e923fc85ae762`
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
# Fri, 20 Mar 2020 03:26:54 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Fri, 20 Mar 2020 03:26:56 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 03:26:59 GMT
RUN a2enmod rewrite expires
# Fri, 20 Mar 2020 03:27:00 GMT
ENV YOURLS_VERSION=1.7.6
# Fri, 20 Mar 2020 03:27:00 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Fri, 20 Mar 2020 03:27:04 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 20 Mar 2020 03:27:04 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Fri, 20 Mar 2020 03:27:05 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Fri, 20 Mar 2020 03:27:06 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 20 Mar 2020 03:27:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 03:27:07 GMT
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
	-	`sha256:d39338e977ad66f2a7bb989ed56ec8fc4f41bdedc6d37bafa72f97eaf90da0dd`  
		Last Modified: Fri, 20 Mar 2020 03:28:25 GMT  
		Size: 275.0 KB (275007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178d8d576b758fe5e23e04481810a9f1c36d56ff6150afdc2826560bdb706adf`  
		Last Modified: Fri, 20 Mar 2020 03:28:25 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0e3e3be135f9a81f08502432d2ae202290d8b908d194fbef6577e9ea075747`  
		Last Modified: Fri, 20 Mar 2020 03:28:23 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99544fe657cb7dff756a794f755e65017ba74c36c5c2ef53a30f99bfd87e565`  
		Last Modified: Fri, 20 Mar 2020 03:28:23 GMT  
		Size: 2.5 MB (2485220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf8bfc46272eadcea2a3ec33a84b3812a4669d65952535673cf84c3bf494474`  
		Last Modified: Fri, 20 Mar 2020 03:28:23 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b845d1636739cd5567aa75b8eaa416f503d0de435996b853135be6f8c4f54e8`  
		Last Modified: Fri, 20 Mar 2020 03:28:23 GMT  
		Size: 1.9 KB (1862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049c745dd020b6dc0304a8496daaf15d414e80cc358f9e648707fb87fd3b1378`  
		Last Modified: Fri, 20 Mar 2020 03:28:23 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm variant v7

```console
$ docker pull yourls@sha256:0b18b23ecb82151953edc2c25ae26a5282304c54f16daa53d3398d3f464b6a05
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127258783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd0438114e15e86f16d2434075a54a04c03026f73705f6f17f0450313ed2de04`
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
# Fri, 20 Mar 2020 03:26:18 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Fri, 20 Mar 2020 03:26:21 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 03:26:24 GMT
RUN a2enmod rewrite expires
# Fri, 20 Mar 2020 03:26:25 GMT
ENV YOURLS_VERSION=1.7.6
# Fri, 20 Mar 2020 03:26:25 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Fri, 20 Mar 2020 03:26:31 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 20 Mar 2020 03:26:32 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Fri, 20 Mar 2020 03:26:32 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Fri, 20 Mar 2020 03:26:33 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 20 Mar 2020 03:26:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 03:26:34 GMT
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
	-	`sha256:99d5684b35d97051ed46480288a8ff10b28c88c5007985651a4f4c41ccf3fe38`  
		Last Modified: Fri, 20 Mar 2020 03:28:51 GMT  
		Size: 247.7 KB (247729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d8beece02de1240a94cda7ab543947ad63453d5a1cb19b44f77c91da5cf83a`  
		Last Modified: Fri, 20 Mar 2020 03:28:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db10c629793c3f42cf7f8c8bee4afd4d03a84bf75a0d44d14f757808e72a887a`  
		Last Modified: Fri, 20 Mar 2020 03:28:50 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd368f0898e091f71fb5a6c1b741273d4f6559eb2809c2d8b2a037fc75a0a5f8`  
		Last Modified: Fri, 20 Mar 2020 03:28:50 GMT  
		Size: 2.5 MB (2485216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94a363e3f22ec79081b3ca9e838e64396003f36e4b97cd187b65cafc773dd05`  
		Last Modified: Fri, 20 Mar 2020 03:28:49 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ee491784f31a32d1d99fec6b1e79d68e9209a95c2e010d6bf5add29ce8ff8b`  
		Last Modified: Fri, 20 Mar 2020 03:28:49 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6e045681746baf77521396b15ad34bec4c45b051a2d370b818c951bcc01350`  
		Last Modified: Fri, 20 Mar 2020 03:28:49 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:41d64ad284cc7bba479ee604c5ff5c0f599963565d224c350df644de44a0f915
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.7 MB (143726362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b403ffce51a5b046586159b91ea1e0716c4e3a308afa81004492d9481fa8e37a`
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
# Fri, 20 Mar 2020 04:02:10 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Fri, 20 Mar 2020 04:02:14 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 04:02:16 GMT
RUN a2enmod rewrite expires
# Fri, 20 Mar 2020 04:02:17 GMT
ENV YOURLS_VERSION=1.7.6
# Fri, 20 Mar 2020 04:02:18 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Fri, 20 Mar 2020 04:02:21 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 20 Mar 2020 04:02:22 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Fri, 20 Mar 2020 04:02:23 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Fri, 20 Mar 2020 04:02:23 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 20 Mar 2020 04:02:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 04:02:25 GMT
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
	-	`sha256:b369ba3b7866e74030dd23fe2030bd929ca053b81c939fb67470615c208eacd0`  
		Last Modified: Fri, 20 Mar 2020 04:05:02 GMT  
		Size: 284.3 KB (284283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84c8395fb29cbc2d6ed937e3589c34c64b261d7bb7da4a22fb10e1ca7676c9c`  
		Last Modified: Fri, 20 Mar 2020 04:05:02 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce57d5f8f2f13dd059b467cb88cdee1bcea9f4f1d3bd0d46fec6f0f13674aa3b`  
		Last Modified: Fri, 20 Mar 2020 04:05:00 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4644e7187b2662904eba3cd0739fbaec53f4e28ac83e8df064aad63b32de6c7b`  
		Last Modified: Fri, 20 Mar 2020 04:05:00 GMT  
		Size: 2.5 MB (2485223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b8c455c2a243c06764d3ac3781c6d0c1d7ceb91ad9480ce198381828e2d26e`  
		Last Modified: Fri, 20 Mar 2020 04:05:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb81d983efe0002e535b9db6171aa34346f839f0d089004f744919636f1513f`  
		Last Modified: Fri, 20 Mar 2020 04:05:00 GMT  
		Size: 1.9 KB (1862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faffd1cddc7ad96ec2f3b3a0e547e406455a4eb39da9dbfc999b84a82f2d67f3`  
		Last Modified: Fri, 20 Mar 2020 04:05:00 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; 386

```console
$ docker pull yourls@sha256:048a15d08a7e3c216bdc3348fffb4d270c8447fc4d66cd84ca19a822fdfce6a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.7 MB (157671557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f4426a94da17ec67fcbee544a25f9489a7e8f4ceed741ad400de77cda42fdf`
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
# Wed, 26 Feb 2020 18:33:02 GMT
ENV PHP_VERSION=7.2.28
# Wed, 26 Feb 2020 18:33:02 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.28.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.28.tar.xz.asc/from/this/mirror
# Wed, 26 Feb 2020 18:33:02 GMT
ENV PHP_SHA256=afe1863301da572dee2e0bad8014813bcced162f980ddc8ec8e41fd72263eb2d PHP_MD5=
# Wed, 26 Feb 2020 18:33:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Feb 2020 18:33:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Feb 2020 18:38:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 26 Feb 2020 18:38:15 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Wed, 26 Feb 2020 18:38:17 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Feb 2020 18:38:19 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 26 Feb 2020 18:38:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Feb 2020 18:38:19 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Feb 2020 18:38:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Feb 2020 18:38:20 GMT
WORKDIR /var/www/html
# Wed, 26 Feb 2020 18:38:20 GMT
EXPOSE 80
# Wed, 26 Feb 2020 18:38:21 GMT
CMD ["apache2-foreground"]
# Wed, 26 Feb 2020 23:03:12 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Wed, 26 Feb 2020 23:03:14 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 26 Feb 2020 23:03:16 GMT
RUN a2enmod rewrite expires
# Wed, 26 Feb 2020 23:03:16 GMT
ENV YOURLS_VERSION=1.7.6
# Wed, 26 Feb 2020 23:03:17 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Wed, 26 Feb 2020 23:03:20 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 26 Feb 2020 23:03:20 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Wed, 26 Feb 2020 23:03:21 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Wed, 26 Feb 2020 23:03:22 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 26 Feb 2020 23:03:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 26 Feb 2020 23:03:22 GMT
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
	-	`sha256:b703bf1f8b17a356d8e0046ff9b6cd299d8e15c60df0af6569b19520312bdb73`  
		Last Modified: Wed, 26 Feb 2020 19:31:12 GMT  
		Size: 12.6 MB (12649681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9efd28f914eff42eab84152834ebd9bc49f4a6e5c7693e95e96253b13a5a3b31`  
		Last Modified: Wed, 26 Feb 2020 19:31:10 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b9fe56f56a9fd8cbb5d0f4e977740344fa842ea2874c08d5b8ea1aad387f32`  
		Last Modified: Wed, 26 Feb 2020 19:31:14 GMT  
		Size: 14.2 MB (14168817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6799e323cedb410eec62fc2bfb9613a10f010f8b1f045d6d433ec6a5689bea`  
		Last Modified: Wed, 26 Feb 2020 19:31:09 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a652a6f500629f367d22c3c8deb9845a2d4ea3451ffc55b8c431de8bf780bb`  
		Last Modified: Wed, 26 Feb 2020 19:31:09 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f660ea49e87617cedbb6af0adb7e642516f12a69d139d0f7405bca2eaf432768`  
		Last Modified: Wed, 26 Feb 2020 19:31:09 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf3d9afbc4d851fac9c145c2ec61f8ed6ecb91f67019313d934fecab7aa991f`  
		Last Modified: Wed, 26 Feb 2020 19:31:09 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff67e7b54aeb5d36995ea7cd9d6bf6a8721125979c883c3646f826149bb2f01`  
		Last Modified: Wed, 26 Feb 2020 23:05:03 GMT  
		Size: 300.3 KB (300335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d00a3f18095190692a032eacb90c04af5ccd168c85806ea83a388de3f9304`  
		Last Modified: Wed, 26 Feb 2020 23:05:03 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a87c777d27f5fb879beeb9103bf5dbed3409452b842086ae2911eb9fa99fb7`  
		Last Modified: Wed, 26 Feb 2020 23:05:01 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b5ff5e415e59619eb140526d8d1d88dcf9c4a232814c183c25b26af9c9227c`  
		Last Modified: Wed, 26 Feb 2020 23:05:03 GMT  
		Size: 2.5 MB (2485191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90428182e2a9ccd93665ca65b34fc52fbf504d279856f91348a7166be7bf05e4`  
		Last Modified: Wed, 26 Feb 2020 23:05:01 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad245f56c2c0b7e06a487f4f1cdda07d468251e92aa4bb16f7bdd99263ad745`  
		Last Modified: Wed, 26 Feb 2020 23:05:01 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0038a1db9cbec3b936843dc7fbf355cb4f1e11ee4147f3dabf741f884e13582`  
		Last Modified: Wed, 26 Feb 2020 23:05:01 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-apache` - linux; ppc64le

```console
$ docker pull yourls@sha256:6530171d367844b999d86d45f1b4546aeb9a4131ef6a83e0de8077439e94fed8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.9 MB (162939729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a894a81b251c398535e7d4f82a1fb65ab612f151a70f463b4eccca4ed750f1`
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
# Wed, 26 Feb 2020 15:06:28 GMT
ENV PHP_VERSION=7.2.28
# Wed, 26 Feb 2020 15:06:31 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.28.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.28.tar.xz.asc/from/this/mirror
# Wed, 26 Feb 2020 15:06:33 GMT
ENV PHP_SHA256=afe1863301da572dee2e0bad8014813bcced162f980ddc8ec8e41fd72263eb2d PHP_MD5=
# Wed, 26 Feb 2020 15:07:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Feb 2020 15:07:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Feb 2020 15:11:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 26 Feb 2020 15:11:38 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Wed, 26 Feb 2020 15:11:42 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Feb 2020 15:11:49 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Wed, 26 Feb 2020 15:11:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Feb 2020 15:11:54 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Feb 2020 15:11:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Feb 2020 15:11:57 GMT
WORKDIR /var/www/html
# Wed, 26 Feb 2020 15:12:01 GMT
EXPOSE 80
# Wed, 26 Feb 2020 15:12:03 GMT
CMD ["apache2-foreground"]
# Thu, 27 Feb 2020 06:11:16 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 27 Feb 2020 06:11:34 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 27 Feb 2020 06:11:48 GMT
RUN a2enmod rewrite expires
# Thu, 27 Feb 2020 06:11:58 GMT
ENV YOURLS_VERSION=1.7.6
# Thu, 27 Feb 2020 06:12:03 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Thu, 27 Feb 2020 06:12:14 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 27 Feb 2020 06:12:16 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 27 Feb 2020 06:12:18 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 27 Feb 2020 06:12:20 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 27 Feb 2020 06:12:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 Feb 2020 06:12:28 GMT
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
	-	`sha256:7cda918969800c590c9c0759fe31840fe70a5ca587073d4fdf4017159c95c293`  
		Last Modified: Wed, 26 Feb 2020 16:06:56 GMT  
		Size: 12.7 MB (12650200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689ccd3ac68f40c014e8190effeffdc3d75b9230c25acd4a3f6848affb268e99`  
		Last Modified: Wed, 26 Feb 2020 16:06:54 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d02195c2c489c030399eab8127c099cda0de1b8c3bfabd99f1439c0be1d7ed2`  
		Last Modified: Wed, 26 Feb 2020 16:06:55 GMT  
		Size: 14.9 MB (14882372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d395dd2afa4c4b256007012ad7b263ff95dc29fe2e3db76eb4e725a731d11b8`  
		Last Modified: Wed, 26 Feb 2020 16:06:51 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cedb3db9b6ba1b3b456285b323f814f6a6b652fbb57f94c90abadb85c1422a99`  
		Last Modified: Wed, 26 Feb 2020 16:06:52 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8357f7f258c164f8e9ee5716976fcfe1bae60f8379ef077f96cf9fec3c2a3c3`  
		Last Modified: Wed, 26 Feb 2020 16:06:52 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab2a462d2829cad4ef37ce456bdedcad7665523a4faf4e075b2241dbba1580cb`  
		Last Modified: Wed, 26 Feb 2020 16:06:52 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b31eab8096b0ddfd66fd3a6eeeec635b4986878d471277098376b671bc176959`  
		Last Modified: Thu, 27 Feb 2020 06:14:33 GMT  
		Size: 322.8 KB (322764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfafda644a9ff95c71e1a093db578630f11bca2dd280693fc1e7c6e5c89277e0`  
		Last Modified: Thu, 27 Feb 2020 06:14:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c9e20b0aff108752d5635936ecd048c487ab7e1a3b43e3d9c93070cb226184`  
		Last Modified: Thu, 27 Feb 2020 06:14:29 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495a10275f276aca9fd49807656bcde7dd1cf78b773d505a56cce91b37331a06`  
		Last Modified: Thu, 27 Feb 2020 06:14:30 GMT  
		Size: 2.5 MB (2485213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c572f14a218c0f48fd5ae54387b7491fca731fda5c0312758933f021608ba76`  
		Last Modified: Thu, 27 Feb 2020 06:14:30 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f834923b55ee2862b6dd34704b0ab5e3d7ac6d2f0bb2d6e9c2b76fde154095`  
		Last Modified: Thu, 27 Feb 2020 06:14:29 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adfea4797dc91ca983170029244a68eae5e5d40d52673fbe8d8f48803df1f1c`  
		Last Modified: Thu, 27 Feb 2020 06:14:29 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
