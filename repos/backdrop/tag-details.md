<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `backdrop`

-	[`backdrop:1`](#backdrop1)
-	[`backdrop:1-apache`](#backdrop1-apache)
-	[`backdrop:1-fpm`](#backdrop1-fpm)
-	[`backdrop:1.21`](#backdrop121)
-	[`backdrop:1.21-apache`](#backdrop121-apache)
-	[`backdrop:1.21-fpm`](#backdrop121-fpm)
-	[`backdrop:1.21.4`](#backdrop1214)
-	[`backdrop:1.21.4-apache`](#backdrop1214-apache)
-	[`backdrop:1.21.4-fpm`](#backdrop1214-fpm)
-	[`backdrop:apache`](#backdropapache)
-	[`backdrop:fpm`](#backdropfpm)
-	[`backdrop:latest`](#backdroplatest)

## `backdrop:1`

```console
$ docker pull backdrop@sha256:f8a73bc6e121962e16a559ea19d9ecddd86ba6e06c3a1076a045089a20a57d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:1` - linux; amd64

```console
$ docker pull backdrop@sha256:79d166e914a528610e8ac5a57638d3b7eeca22b5bba19e5e38fd73c58c1c3e19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174331557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c020ca5ac8371986920c2cc852574e0dec788b104dd051b3a226c3349052370`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:12:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:12:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:12:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:29:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:03:55 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:04:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:04:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:05:59 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:06:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:06:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Jun 2022 23:06:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:06:00 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:06:00 GMT
EXPOSE 80
# Thu, 09 Jun 2022 23:06:00 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 01:49:36 GMT
RUN a2enmod rewrite
# Fri, 10 Jun 2022 01:50:31 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:50:31 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:50:34 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:50:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:50:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:50:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772088206f8568203e6d410d3b89fbe52c179aff6abed864eb98bbb88600a463`  
		Last Modified: Sat, 28 May 2022 09:51:08 GMT  
		Size: 19.2 MB (19247884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81c5474649ebdbc8488baf5cd66754f83eab0486a88885f482b0e7f964fdca`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a528527ae803d0d6a51823792cd9d053c716c464e181fe3ec3d727e54bb20`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344c792709d4e7f4afa7e649971be01278f6d6c5493960b7d273ca53baa33fef`  
		Last Modified: Thu, 09 Jun 2022 23:59:43 GMT  
		Size: 10.8 MB (10758865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9638273c35415584850d053ff0dceb792c0b27660e3b6a65d362d1844c2bc4`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec70638e42f38ff2ee5cd38c046b866641f774440b37d9a87a5b44bf3f87f15`  
		Last Modified: Thu, 09 Jun 2022 23:59:42 GMT  
		Size: 10.2 MB (10196959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f65f5bb3b0aa859ec22263310e7c741ae879d89cbe65875ab807becd2b47b`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55578a5ce5e8e0c1c142886375dcb25a36bc51a63022a7608728fb22f1447a32`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dd85b4dfa569330bd78e093419e92e53ac9b5cfe7f358d6bf7c8ab0ebb062d`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe783f7bb3462c718e445caac5a99184436d3feb0bd79ac96941e23df8a9a92a`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9df1fc0744f36fc399c45908866e8cf9c3d6d73b30376c92b906e0cf3dd377`  
		Last Modified: Fri, 10 Jun 2022 01:52:10 GMT  
		Size: 2.4 MB (2415102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17402dd1c5d82171bd169485c877a00fff3176ec4f520005d4581c69d3f1c2fb`  
		Last Modified: Fri, 10 Jun 2022 01:52:11 GMT  
		Size: 8.7 MB (8722847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dabfe686dbaa4a62a5be96d5738e3f7c6f192412fc272738833e8a3ca629cb`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:1` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:eab024819e18d2058ce6ffb1253f9d86fb574b3e79cd3e6b5bd7b8b7c6ae2ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.2 MB (167164028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b284515cf0b3bcb500aef83801c927e84bb401bfb2c73efe9589aed7837abb14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 06:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 06:35:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 06:35:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 06:35:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:05:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:05:17 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:05:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:05:19 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:05:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:07:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:07:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:07:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 08:07:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:28 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:07:29 GMT
EXPOSE 80
# Thu, 23 Jun 2022 08:07:30 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 21:02:56 GMT
RUN a2enmod rewrite
# Thu, 23 Jun 2022 21:04:02 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:04:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:04:03 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:04:04 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:04:08 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:04:09 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:04:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c146af8093559f8941c628d5ba6b3d917b6632be0ef8db3f94bd273e5f8e5e`  
		Last Modified: Thu, 23 Jun 2022 08:32:16 GMT  
		Size: 18.9 MB (18942958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c65506677c18dabf6680677a4a00f319c51d98d01385906b98cb2bd042d30b3`  
		Last Modified: Thu, 23 Jun 2022 08:32:13 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231191daad959d9fc1c3e70aa102000ecac8dd110ae7c5fd92c78a6c7fbafc4a`  
		Last Modified: Thu, 23 Jun 2022 08:32:14 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8766dc7144bf701c42e8cb04829bae7df122e874c6d1c1fc6c3d28af3df3ed`  
		Last Modified: Thu, 23 Jun 2022 08:43:49 GMT  
		Size: 10.5 MB (10543172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8320e583eb8b3eef52b7f7485be9206078705fa7c83ebbdf58828c46976c9a`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0751df93b68c12d7177068c0f698221012dc784c57c6bb060e31ae01b067dfdb`  
		Last Modified: Thu, 23 Jun 2022 08:43:48 GMT  
		Size: 10.0 MB (9998952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf10f28ca9517e7b1024947097349b2a6336ea34dab98ff5ef5c482c41ba9f7`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963139f3ad32863502ea64c536e229e41aae110d402e69e80caa11aeda2b424f`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f56943bfdf6d984c7f842a24ffb8214b4f2c125ec4e43149e069346ff21c43`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482a0088f4fcccdc8b25ec4e0fb7dca684416af37a60ec29d9642f590d1c3560`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b55b12ae706ec4b391b77fb212708796ace940f853a5f0470b38e18c34579b2`  
		Last Modified: Thu, 23 Jun 2022 21:06:14 GMT  
		Size: 2.2 MB (2165254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8394d2c16c073e488afc0a8227c3e05bd44de74400cf36a578b64da055f2ca`  
		Last Modified: Thu, 23 Jun 2022 21:06:16 GMT  
		Size: 8.7 MB (8721844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccb59cbdbee868f15c2773f93864618111b1aa9a4aebe6236359b3e852e8dc1`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:1-apache`

```console
$ docker pull backdrop@sha256:f8a73bc6e121962e16a559ea19d9ecddd86ba6e06c3a1076a045089a20a57d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:1-apache` - linux; amd64

```console
$ docker pull backdrop@sha256:79d166e914a528610e8ac5a57638d3b7eeca22b5bba19e5e38fd73c58c1c3e19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174331557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c020ca5ac8371986920c2cc852574e0dec788b104dd051b3a226c3349052370`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:12:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:12:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:12:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:29:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:03:55 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:04:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:04:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:05:59 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:06:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:06:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Jun 2022 23:06:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:06:00 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:06:00 GMT
EXPOSE 80
# Thu, 09 Jun 2022 23:06:00 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 01:49:36 GMT
RUN a2enmod rewrite
# Fri, 10 Jun 2022 01:50:31 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:50:31 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:50:34 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:50:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:50:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:50:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772088206f8568203e6d410d3b89fbe52c179aff6abed864eb98bbb88600a463`  
		Last Modified: Sat, 28 May 2022 09:51:08 GMT  
		Size: 19.2 MB (19247884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81c5474649ebdbc8488baf5cd66754f83eab0486a88885f482b0e7f964fdca`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a528527ae803d0d6a51823792cd9d053c716c464e181fe3ec3d727e54bb20`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344c792709d4e7f4afa7e649971be01278f6d6c5493960b7d273ca53baa33fef`  
		Last Modified: Thu, 09 Jun 2022 23:59:43 GMT  
		Size: 10.8 MB (10758865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9638273c35415584850d053ff0dceb792c0b27660e3b6a65d362d1844c2bc4`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec70638e42f38ff2ee5cd38c046b866641f774440b37d9a87a5b44bf3f87f15`  
		Last Modified: Thu, 09 Jun 2022 23:59:42 GMT  
		Size: 10.2 MB (10196959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f65f5bb3b0aa859ec22263310e7c741ae879d89cbe65875ab807becd2b47b`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55578a5ce5e8e0c1c142886375dcb25a36bc51a63022a7608728fb22f1447a32`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dd85b4dfa569330bd78e093419e92e53ac9b5cfe7f358d6bf7c8ab0ebb062d`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe783f7bb3462c718e445caac5a99184436d3feb0bd79ac96941e23df8a9a92a`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9df1fc0744f36fc399c45908866e8cf9c3d6d73b30376c92b906e0cf3dd377`  
		Last Modified: Fri, 10 Jun 2022 01:52:10 GMT  
		Size: 2.4 MB (2415102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17402dd1c5d82171bd169485c877a00fff3176ec4f520005d4581c69d3f1c2fb`  
		Last Modified: Fri, 10 Jun 2022 01:52:11 GMT  
		Size: 8.7 MB (8722847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dabfe686dbaa4a62a5be96d5738e3f7c6f192412fc272738833e8a3ca629cb`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:1-apache` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:eab024819e18d2058ce6ffb1253f9d86fb574b3e79cd3e6b5bd7b8b7c6ae2ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.2 MB (167164028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b284515cf0b3bcb500aef83801c927e84bb401bfb2c73efe9589aed7837abb14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 06:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 06:35:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 06:35:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 06:35:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:05:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:05:17 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:05:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:05:19 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:05:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:07:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:07:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:07:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 08:07:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:28 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:07:29 GMT
EXPOSE 80
# Thu, 23 Jun 2022 08:07:30 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 21:02:56 GMT
RUN a2enmod rewrite
# Thu, 23 Jun 2022 21:04:02 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:04:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:04:03 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:04:04 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:04:08 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:04:09 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:04:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c146af8093559f8941c628d5ba6b3d917b6632be0ef8db3f94bd273e5f8e5e`  
		Last Modified: Thu, 23 Jun 2022 08:32:16 GMT  
		Size: 18.9 MB (18942958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c65506677c18dabf6680677a4a00f319c51d98d01385906b98cb2bd042d30b3`  
		Last Modified: Thu, 23 Jun 2022 08:32:13 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231191daad959d9fc1c3e70aa102000ecac8dd110ae7c5fd92c78a6c7fbafc4a`  
		Last Modified: Thu, 23 Jun 2022 08:32:14 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8766dc7144bf701c42e8cb04829bae7df122e874c6d1c1fc6c3d28af3df3ed`  
		Last Modified: Thu, 23 Jun 2022 08:43:49 GMT  
		Size: 10.5 MB (10543172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8320e583eb8b3eef52b7f7485be9206078705fa7c83ebbdf58828c46976c9a`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0751df93b68c12d7177068c0f698221012dc784c57c6bb060e31ae01b067dfdb`  
		Last Modified: Thu, 23 Jun 2022 08:43:48 GMT  
		Size: 10.0 MB (9998952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf10f28ca9517e7b1024947097349b2a6336ea34dab98ff5ef5c482c41ba9f7`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963139f3ad32863502ea64c536e229e41aae110d402e69e80caa11aeda2b424f`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f56943bfdf6d984c7f842a24ffb8214b4f2c125ec4e43149e069346ff21c43`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482a0088f4fcccdc8b25ec4e0fb7dca684416af37a60ec29d9642f590d1c3560`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b55b12ae706ec4b391b77fb212708796ace940f853a5f0470b38e18c34579b2`  
		Last Modified: Thu, 23 Jun 2022 21:06:14 GMT  
		Size: 2.2 MB (2165254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8394d2c16c073e488afc0a8227c3e05bd44de74400cf36a578b64da055f2ca`  
		Last Modified: Thu, 23 Jun 2022 21:06:16 GMT  
		Size: 8.7 MB (8721844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccb59cbdbee868f15c2773f93864618111b1aa9a4aebe6236359b3e852e8dc1`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:1-fpm`

```console
$ docker pull backdrop@sha256:b873a38ba65356ddbf8e684d967806456859098cfdf9d84e50a64ba62ca41097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:1-fpm` - linux; amd64

```console
$ docker pull backdrop@sha256:e972c1e1f7b40a1f61990845838ad1878b76c7d31bfe092c5a40a28dbf6ff83c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170242929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77801adb9ebd00347b7bacbfd137886d183e2554220bff980607b213f383cc3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:27:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:01:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:01:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:08:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:08:45 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:08:45 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:08:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:08:46 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:08:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 09 Jun 2022 23:08:46 GMT
STOPSIGNAL SIGQUIT
# Thu, 09 Jun 2022 23:08:46 GMT
EXPOSE 9000
# Thu, 09 Jun 2022 23:08:46 GMT
CMD ["php-fpm"]
# Fri, 10 Jun 2022 01:51:38 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:51:38 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:51:38 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:51:38 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:51:41 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:51:41 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:51:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:51:41 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ae4909e013d6c9ba47bf5f505e50cfb156f69913a7d72ec7390aa0faeb3777`  
		Last Modified: Thu, 09 Jun 2022 23:59:00 GMT  
		Size: 10.7 MB (10737467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95442bcca7a2e1a29d317920308121f5c92ebda052c6aad6ae90729d73cb8ee9`  
		Last Modified: Thu, 09 Jun 2022 23:58:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d68ee1d2441e5f24572dcbad3e15601c94886c30a3adf79ff2db63bde4606`  
		Last Modified: Fri, 10 Jun 2022 00:00:10 GMT  
		Size: 25.4 MB (25396630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e25477785378c73db581fb8089c07a94886264839bcbd2d32d74b356bc9ebc`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae29a18256bb27c519d3140394afade3f6a0e1ccb08279f824e4257d226044f`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c566c8d5b21a27dcd8744b196148b5d59cf7d1146c3ac0887f2d22e6f469fbd1`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8575250f2bf8bcdb8a601a7e3c5474f688cedfc4e0f2348cec8124fa3f411f2b`  
		Last Modified: Fri, 10 Jun 2022 01:52:44 GMT  
		Size: 2.4 MB (2389845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c74b6b9c524b9cfca8911df221c0c7873e0d07f09457ad1e10cb16bc884d03`  
		Last Modified: Fri, 10 Jun 2022 01:52:45 GMT  
		Size: 8.7 MB (8722855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5b837e3f6d4f1820381b40e7aa08c04206fe1ecf11486add3e4babbaf36b0e`  
		Last Modified: Fri, 10 Jun 2022 01:52:43 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:1-fpm` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:b6f5ce0be872659bb100bcfc68307e28fcfc7cef5733a6e306026eca99dc3941
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.1 MB (163130320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4df60f59f68f3dc537eee832409a4b8d023a1afee88d0dd3018fc2ca5fd0ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:31:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:31:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:31:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:02:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:03:00 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:03:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:03:02 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:03:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:03:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:10:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:10:15 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:10:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:10:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:10:17 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:10:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Jun 2022 08:10:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jun 2022 08:10:20 GMT
EXPOSE 9000
# Thu, 23 Jun 2022 08:10:21 GMT
CMD ["php-fpm"]
# Thu, 23 Jun 2022 21:05:26 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:05:27 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:05:28 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:05:29 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:05:33 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:05:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:05:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:05:35 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3343549bd53bda328dd3b6a5488a1a92c86d260c73ff28e6b6a596fa1b521`  
		Last Modified: Thu, 23 Jun 2022 08:43:00 GMT  
		Size: 10.5 MB (10521113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b6c58fb818b8de29e436d358e87f11665f2ded5521370e61bbec68b1ddb494`  
		Last Modified: Thu, 23 Jun 2022 08:42:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d55d8e081af25f0bc7e97ae6b8c49840660259cf65b20366337a2670d1a3a1`  
		Last Modified: Thu, 23 Jun 2022 08:44:18 GMT  
		Size: 24.9 MB (24949587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f419449f189d35d6be08835101aeec77d7e0e0281b642b06a40e06e2a592667`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a2925453a4c8146fd5bbea9559d5c43da91dabe6ab0b0a6c413496f322b785`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b9a83719254b7a18c0cc13e03f834841bfa53fad61503f0ba887a4118cc526`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429e15ea917e05f1652db513507e8a1db34af024cbb28e8db5f1107688f944d1`  
		Last Modified: Thu, 23 Jun 2022 21:06:55 GMT  
		Size: 2.1 MB (2139603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470ef2c64313b66a3d97834c58b4be6388ce5b7afac7a50d06230ac57c02a6cc`  
		Last Modified: Thu, 23 Jun 2022 21:06:57 GMT  
		Size: 8.7 MB (8721845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5eb788bbd05267f8a8211286c7aa26df963d883f03d248415a1ecbc8bfc035`  
		Last Modified: Thu, 23 Jun 2022 21:06:54 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:1.21`

```console
$ docker pull backdrop@sha256:f8a73bc6e121962e16a559ea19d9ecddd86ba6e06c3a1076a045089a20a57d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:1.21` - linux; amd64

```console
$ docker pull backdrop@sha256:79d166e914a528610e8ac5a57638d3b7eeca22b5bba19e5e38fd73c58c1c3e19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174331557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c020ca5ac8371986920c2cc852574e0dec788b104dd051b3a226c3349052370`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:12:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:12:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:12:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:29:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:03:55 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:04:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:04:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:05:59 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:06:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:06:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Jun 2022 23:06:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:06:00 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:06:00 GMT
EXPOSE 80
# Thu, 09 Jun 2022 23:06:00 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 01:49:36 GMT
RUN a2enmod rewrite
# Fri, 10 Jun 2022 01:50:31 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:50:31 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:50:34 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:50:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:50:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:50:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772088206f8568203e6d410d3b89fbe52c179aff6abed864eb98bbb88600a463`  
		Last Modified: Sat, 28 May 2022 09:51:08 GMT  
		Size: 19.2 MB (19247884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81c5474649ebdbc8488baf5cd66754f83eab0486a88885f482b0e7f964fdca`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a528527ae803d0d6a51823792cd9d053c716c464e181fe3ec3d727e54bb20`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344c792709d4e7f4afa7e649971be01278f6d6c5493960b7d273ca53baa33fef`  
		Last Modified: Thu, 09 Jun 2022 23:59:43 GMT  
		Size: 10.8 MB (10758865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9638273c35415584850d053ff0dceb792c0b27660e3b6a65d362d1844c2bc4`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec70638e42f38ff2ee5cd38c046b866641f774440b37d9a87a5b44bf3f87f15`  
		Last Modified: Thu, 09 Jun 2022 23:59:42 GMT  
		Size: 10.2 MB (10196959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f65f5bb3b0aa859ec22263310e7c741ae879d89cbe65875ab807becd2b47b`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55578a5ce5e8e0c1c142886375dcb25a36bc51a63022a7608728fb22f1447a32`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dd85b4dfa569330bd78e093419e92e53ac9b5cfe7f358d6bf7c8ab0ebb062d`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe783f7bb3462c718e445caac5a99184436d3feb0bd79ac96941e23df8a9a92a`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9df1fc0744f36fc399c45908866e8cf9c3d6d73b30376c92b906e0cf3dd377`  
		Last Modified: Fri, 10 Jun 2022 01:52:10 GMT  
		Size: 2.4 MB (2415102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17402dd1c5d82171bd169485c877a00fff3176ec4f520005d4581c69d3f1c2fb`  
		Last Modified: Fri, 10 Jun 2022 01:52:11 GMT  
		Size: 8.7 MB (8722847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dabfe686dbaa4a62a5be96d5738e3f7c6f192412fc272738833e8a3ca629cb`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:1.21` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:eab024819e18d2058ce6ffb1253f9d86fb574b3e79cd3e6b5bd7b8b7c6ae2ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.2 MB (167164028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b284515cf0b3bcb500aef83801c927e84bb401bfb2c73efe9589aed7837abb14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 06:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 06:35:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 06:35:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 06:35:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:05:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:05:17 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:05:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:05:19 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:05:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:07:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:07:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:07:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 08:07:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:28 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:07:29 GMT
EXPOSE 80
# Thu, 23 Jun 2022 08:07:30 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 21:02:56 GMT
RUN a2enmod rewrite
# Thu, 23 Jun 2022 21:04:02 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:04:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:04:03 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:04:04 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:04:08 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:04:09 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:04:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c146af8093559f8941c628d5ba6b3d917b6632be0ef8db3f94bd273e5f8e5e`  
		Last Modified: Thu, 23 Jun 2022 08:32:16 GMT  
		Size: 18.9 MB (18942958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c65506677c18dabf6680677a4a00f319c51d98d01385906b98cb2bd042d30b3`  
		Last Modified: Thu, 23 Jun 2022 08:32:13 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231191daad959d9fc1c3e70aa102000ecac8dd110ae7c5fd92c78a6c7fbafc4a`  
		Last Modified: Thu, 23 Jun 2022 08:32:14 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8766dc7144bf701c42e8cb04829bae7df122e874c6d1c1fc6c3d28af3df3ed`  
		Last Modified: Thu, 23 Jun 2022 08:43:49 GMT  
		Size: 10.5 MB (10543172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8320e583eb8b3eef52b7f7485be9206078705fa7c83ebbdf58828c46976c9a`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0751df93b68c12d7177068c0f698221012dc784c57c6bb060e31ae01b067dfdb`  
		Last Modified: Thu, 23 Jun 2022 08:43:48 GMT  
		Size: 10.0 MB (9998952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf10f28ca9517e7b1024947097349b2a6336ea34dab98ff5ef5c482c41ba9f7`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963139f3ad32863502ea64c536e229e41aae110d402e69e80caa11aeda2b424f`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f56943bfdf6d984c7f842a24ffb8214b4f2c125ec4e43149e069346ff21c43`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482a0088f4fcccdc8b25ec4e0fb7dca684416af37a60ec29d9642f590d1c3560`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b55b12ae706ec4b391b77fb212708796ace940f853a5f0470b38e18c34579b2`  
		Last Modified: Thu, 23 Jun 2022 21:06:14 GMT  
		Size: 2.2 MB (2165254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8394d2c16c073e488afc0a8227c3e05bd44de74400cf36a578b64da055f2ca`  
		Last Modified: Thu, 23 Jun 2022 21:06:16 GMT  
		Size: 8.7 MB (8721844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccb59cbdbee868f15c2773f93864618111b1aa9a4aebe6236359b3e852e8dc1`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:1.21-apache`

```console
$ docker pull backdrop@sha256:f8a73bc6e121962e16a559ea19d9ecddd86ba6e06c3a1076a045089a20a57d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:1.21-apache` - linux; amd64

```console
$ docker pull backdrop@sha256:79d166e914a528610e8ac5a57638d3b7eeca22b5bba19e5e38fd73c58c1c3e19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174331557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c020ca5ac8371986920c2cc852574e0dec788b104dd051b3a226c3349052370`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:12:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:12:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:12:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:29:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:03:55 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:04:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:04:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:05:59 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:06:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:06:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Jun 2022 23:06:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:06:00 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:06:00 GMT
EXPOSE 80
# Thu, 09 Jun 2022 23:06:00 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 01:49:36 GMT
RUN a2enmod rewrite
# Fri, 10 Jun 2022 01:50:31 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:50:31 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:50:34 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:50:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:50:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:50:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772088206f8568203e6d410d3b89fbe52c179aff6abed864eb98bbb88600a463`  
		Last Modified: Sat, 28 May 2022 09:51:08 GMT  
		Size: 19.2 MB (19247884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81c5474649ebdbc8488baf5cd66754f83eab0486a88885f482b0e7f964fdca`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a528527ae803d0d6a51823792cd9d053c716c464e181fe3ec3d727e54bb20`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344c792709d4e7f4afa7e649971be01278f6d6c5493960b7d273ca53baa33fef`  
		Last Modified: Thu, 09 Jun 2022 23:59:43 GMT  
		Size: 10.8 MB (10758865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9638273c35415584850d053ff0dceb792c0b27660e3b6a65d362d1844c2bc4`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec70638e42f38ff2ee5cd38c046b866641f774440b37d9a87a5b44bf3f87f15`  
		Last Modified: Thu, 09 Jun 2022 23:59:42 GMT  
		Size: 10.2 MB (10196959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f65f5bb3b0aa859ec22263310e7c741ae879d89cbe65875ab807becd2b47b`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55578a5ce5e8e0c1c142886375dcb25a36bc51a63022a7608728fb22f1447a32`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dd85b4dfa569330bd78e093419e92e53ac9b5cfe7f358d6bf7c8ab0ebb062d`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe783f7bb3462c718e445caac5a99184436d3feb0bd79ac96941e23df8a9a92a`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9df1fc0744f36fc399c45908866e8cf9c3d6d73b30376c92b906e0cf3dd377`  
		Last Modified: Fri, 10 Jun 2022 01:52:10 GMT  
		Size: 2.4 MB (2415102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17402dd1c5d82171bd169485c877a00fff3176ec4f520005d4581c69d3f1c2fb`  
		Last Modified: Fri, 10 Jun 2022 01:52:11 GMT  
		Size: 8.7 MB (8722847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dabfe686dbaa4a62a5be96d5738e3f7c6f192412fc272738833e8a3ca629cb`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:1.21-apache` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:eab024819e18d2058ce6ffb1253f9d86fb574b3e79cd3e6b5bd7b8b7c6ae2ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.2 MB (167164028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b284515cf0b3bcb500aef83801c927e84bb401bfb2c73efe9589aed7837abb14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 06:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 06:35:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 06:35:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 06:35:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:05:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:05:17 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:05:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:05:19 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:05:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:07:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:07:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:07:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 08:07:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:28 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:07:29 GMT
EXPOSE 80
# Thu, 23 Jun 2022 08:07:30 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 21:02:56 GMT
RUN a2enmod rewrite
# Thu, 23 Jun 2022 21:04:02 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:04:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:04:03 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:04:04 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:04:08 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:04:09 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:04:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c146af8093559f8941c628d5ba6b3d917b6632be0ef8db3f94bd273e5f8e5e`  
		Last Modified: Thu, 23 Jun 2022 08:32:16 GMT  
		Size: 18.9 MB (18942958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c65506677c18dabf6680677a4a00f319c51d98d01385906b98cb2bd042d30b3`  
		Last Modified: Thu, 23 Jun 2022 08:32:13 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231191daad959d9fc1c3e70aa102000ecac8dd110ae7c5fd92c78a6c7fbafc4a`  
		Last Modified: Thu, 23 Jun 2022 08:32:14 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8766dc7144bf701c42e8cb04829bae7df122e874c6d1c1fc6c3d28af3df3ed`  
		Last Modified: Thu, 23 Jun 2022 08:43:49 GMT  
		Size: 10.5 MB (10543172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8320e583eb8b3eef52b7f7485be9206078705fa7c83ebbdf58828c46976c9a`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0751df93b68c12d7177068c0f698221012dc784c57c6bb060e31ae01b067dfdb`  
		Last Modified: Thu, 23 Jun 2022 08:43:48 GMT  
		Size: 10.0 MB (9998952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf10f28ca9517e7b1024947097349b2a6336ea34dab98ff5ef5c482c41ba9f7`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963139f3ad32863502ea64c536e229e41aae110d402e69e80caa11aeda2b424f`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f56943bfdf6d984c7f842a24ffb8214b4f2c125ec4e43149e069346ff21c43`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482a0088f4fcccdc8b25ec4e0fb7dca684416af37a60ec29d9642f590d1c3560`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b55b12ae706ec4b391b77fb212708796ace940f853a5f0470b38e18c34579b2`  
		Last Modified: Thu, 23 Jun 2022 21:06:14 GMT  
		Size: 2.2 MB (2165254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8394d2c16c073e488afc0a8227c3e05bd44de74400cf36a578b64da055f2ca`  
		Last Modified: Thu, 23 Jun 2022 21:06:16 GMT  
		Size: 8.7 MB (8721844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccb59cbdbee868f15c2773f93864618111b1aa9a4aebe6236359b3e852e8dc1`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:1.21-fpm`

```console
$ docker pull backdrop@sha256:b873a38ba65356ddbf8e684d967806456859098cfdf9d84e50a64ba62ca41097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:1.21-fpm` - linux; amd64

```console
$ docker pull backdrop@sha256:e972c1e1f7b40a1f61990845838ad1878b76c7d31bfe092c5a40a28dbf6ff83c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170242929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77801adb9ebd00347b7bacbfd137886d183e2554220bff980607b213f383cc3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:27:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:01:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:01:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:08:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:08:45 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:08:45 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:08:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:08:46 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:08:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 09 Jun 2022 23:08:46 GMT
STOPSIGNAL SIGQUIT
# Thu, 09 Jun 2022 23:08:46 GMT
EXPOSE 9000
# Thu, 09 Jun 2022 23:08:46 GMT
CMD ["php-fpm"]
# Fri, 10 Jun 2022 01:51:38 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:51:38 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:51:38 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:51:38 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:51:41 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:51:41 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:51:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:51:41 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ae4909e013d6c9ba47bf5f505e50cfb156f69913a7d72ec7390aa0faeb3777`  
		Last Modified: Thu, 09 Jun 2022 23:59:00 GMT  
		Size: 10.7 MB (10737467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95442bcca7a2e1a29d317920308121f5c92ebda052c6aad6ae90729d73cb8ee9`  
		Last Modified: Thu, 09 Jun 2022 23:58:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d68ee1d2441e5f24572dcbad3e15601c94886c30a3adf79ff2db63bde4606`  
		Last Modified: Fri, 10 Jun 2022 00:00:10 GMT  
		Size: 25.4 MB (25396630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e25477785378c73db581fb8089c07a94886264839bcbd2d32d74b356bc9ebc`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae29a18256bb27c519d3140394afade3f6a0e1ccb08279f824e4257d226044f`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c566c8d5b21a27dcd8744b196148b5d59cf7d1146c3ac0887f2d22e6f469fbd1`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8575250f2bf8bcdb8a601a7e3c5474f688cedfc4e0f2348cec8124fa3f411f2b`  
		Last Modified: Fri, 10 Jun 2022 01:52:44 GMT  
		Size: 2.4 MB (2389845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c74b6b9c524b9cfca8911df221c0c7873e0d07f09457ad1e10cb16bc884d03`  
		Last Modified: Fri, 10 Jun 2022 01:52:45 GMT  
		Size: 8.7 MB (8722855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5b837e3f6d4f1820381b40e7aa08c04206fe1ecf11486add3e4babbaf36b0e`  
		Last Modified: Fri, 10 Jun 2022 01:52:43 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:1.21-fpm` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:b6f5ce0be872659bb100bcfc68307e28fcfc7cef5733a6e306026eca99dc3941
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.1 MB (163130320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4df60f59f68f3dc537eee832409a4b8d023a1afee88d0dd3018fc2ca5fd0ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:31:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:31:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:31:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:02:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:03:00 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:03:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:03:02 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:03:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:03:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:10:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:10:15 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:10:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:10:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:10:17 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:10:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Jun 2022 08:10:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jun 2022 08:10:20 GMT
EXPOSE 9000
# Thu, 23 Jun 2022 08:10:21 GMT
CMD ["php-fpm"]
# Thu, 23 Jun 2022 21:05:26 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:05:27 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:05:28 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:05:29 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:05:33 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:05:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:05:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:05:35 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3343549bd53bda328dd3b6a5488a1a92c86d260c73ff28e6b6a596fa1b521`  
		Last Modified: Thu, 23 Jun 2022 08:43:00 GMT  
		Size: 10.5 MB (10521113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b6c58fb818b8de29e436d358e87f11665f2ded5521370e61bbec68b1ddb494`  
		Last Modified: Thu, 23 Jun 2022 08:42:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d55d8e081af25f0bc7e97ae6b8c49840660259cf65b20366337a2670d1a3a1`  
		Last Modified: Thu, 23 Jun 2022 08:44:18 GMT  
		Size: 24.9 MB (24949587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f419449f189d35d6be08835101aeec77d7e0e0281b642b06a40e06e2a592667`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a2925453a4c8146fd5bbea9559d5c43da91dabe6ab0b0a6c413496f322b785`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b9a83719254b7a18c0cc13e03f834841bfa53fad61503f0ba887a4118cc526`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429e15ea917e05f1652db513507e8a1db34af024cbb28e8db5f1107688f944d1`  
		Last Modified: Thu, 23 Jun 2022 21:06:55 GMT  
		Size: 2.1 MB (2139603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470ef2c64313b66a3d97834c58b4be6388ce5b7afac7a50d06230ac57c02a6cc`  
		Last Modified: Thu, 23 Jun 2022 21:06:57 GMT  
		Size: 8.7 MB (8721845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5eb788bbd05267f8a8211286c7aa26df963d883f03d248415a1ecbc8bfc035`  
		Last Modified: Thu, 23 Jun 2022 21:06:54 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:1.21.4`

```console
$ docker pull backdrop@sha256:f8a73bc6e121962e16a559ea19d9ecddd86ba6e06c3a1076a045089a20a57d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:1.21.4` - linux; amd64

```console
$ docker pull backdrop@sha256:79d166e914a528610e8ac5a57638d3b7eeca22b5bba19e5e38fd73c58c1c3e19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174331557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c020ca5ac8371986920c2cc852574e0dec788b104dd051b3a226c3349052370`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:12:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:12:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:12:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:29:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:03:55 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:04:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:04:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:05:59 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:06:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:06:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Jun 2022 23:06:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:06:00 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:06:00 GMT
EXPOSE 80
# Thu, 09 Jun 2022 23:06:00 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 01:49:36 GMT
RUN a2enmod rewrite
# Fri, 10 Jun 2022 01:50:31 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:50:31 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:50:34 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:50:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:50:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:50:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772088206f8568203e6d410d3b89fbe52c179aff6abed864eb98bbb88600a463`  
		Last Modified: Sat, 28 May 2022 09:51:08 GMT  
		Size: 19.2 MB (19247884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81c5474649ebdbc8488baf5cd66754f83eab0486a88885f482b0e7f964fdca`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a528527ae803d0d6a51823792cd9d053c716c464e181fe3ec3d727e54bb20`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344c792709d4e7f4afa7e649971be01278f6d6c5493960b7d273ca53baa33fef`  
		Last Modified: Thu, 09 Jun 2022 23:59:43 GMT  
		Size: 10.8 MB (10758865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9638273c35415584850d053ff0dceb792c0b27660e3b6a65d362d1844c2bc4`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec70638e42f38ff2ee5cd38c046b866641f774440b37d9a87a5b44bf3f87f15`  
		Last Modified: Thu, 09 Jun 2022 23:59:42 GMT  
		Size: 10.2 MB (10196959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f65f5bb3b0aa859ec22263310e7c741ae879d89cbe65875ab807becd2b47b`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55578a5ce5e8e0c1c142886375dcb25a36bc51a63022a7608728fb22f1447a32`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dd85b4dfa569330bd78e093419e92e53ac9b5cfe7f358d6bf7c8ab0ebb062d`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe783f7bb3462c718e445caac5a99184436d3feb0bd79ac96941e23df8a9a92a`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9df1fc0744f36fc399c45908866e8cf9c3d6d73b30376c92b906e0cf3dd377`  
		Last Modified: Fri, 10 Jun 2022 01:52:10 GMT  
		Size: 2.4 MB (2415102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17402dd1c5d82171bd169485c877a00fff3176ec4f520005d4581c69d3f1c2fb`  
		Last Modified: Fri, 10 Jun 2022 01:52:11 GMT  
		Size: 8.7 MB (8722847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dabfe686dbaa4a62a5be96d5738e3f7c6f192412fc272738833e8a3ca629cb`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:1.21.4` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:eab024819e18d2058ce6ffb1253f9d86fb574b3e79cd3e6b5bd7b8b7c6ae2ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.2 MB (167164028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b284515cf0b3bcb500aef83801c927e84bb401bfb2c73efe9589aed7837abb14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 06:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 06:35:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 06:35:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 06:35:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:05:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:05:17 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:05:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:05:19 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:05:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:07:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:07:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:07:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 08:07:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:28 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:07:29 GMT
EXPOSE 80
# Thu, 23 Jun 2022 08:07:30 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 21:02:56 GMT
RUN a2enmod rewrite
# Thu, 23 Jun 2022 21:04:02 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:04:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:04:03 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:04:04 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:04:08 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:04:09 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:04:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c146af8093559f8941c628d5ba6b3d917b6632be0ef8db3f94bd273e5f8e5e`  
		Last Modified: Thu, 23 Jun 2022 08:32:16 GMT  
		Size: 18.9 MB (18942958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c65506677c18dabf6680677a4a00f319c51d98d01385906b98cb2bd042d30b3`  
		Last Modified: Thu, 23 Jun 2022 08:32:13 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231191daad959d9fc1c3e70aa102000ecac8dd110ae7c5fd92c78a6c7fbafc4a`  
		Last Modified: Thu, 23 Jun 2022 08:32:14 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8766dc7144bf701c42e8cb04829bae7df122e874c6d1c1fc6c3d28af3df3ed`  
		Last Modified: Thu, 23 Jun 2022 08:43:49 GMT  
		Size: 10.5 MB (10543172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8320e583eb8b3eef52b7f7485be9206078705fa7c83ebbdf58828c46976c9a`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0751df93b68c12d7177068c0f698221012dc784c57c6bb060e31ae01b067dfdb`  
		Last Modified: Thu, 23 Jun 2022 08:43:48 GMT  
		Size: 10.0 MB (9998952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf10f28ca9517e7b1024947097349b2a6336ea34dab98ff5ef5c482c41ba9f7`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963139f3ad32863502ea64c536e229e41aae110d402e69e80caa11aeda2b424f`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f56943bfdf6d984c7f842a24ffb8214b4f2c125ec4e43149e069346ff21c43`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482a0088f4fcccdc8b25ec4e0fb7dca684416af37a60ec29d9642f590d1c3560`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b55b12ae706ec4b391b77fb212708796ace940f853a5f0470b38e18c34579b2`  
		Last Modified: Thu, 23 Jun 2022 21:06:14 GMT  
		Size: 2.2 MB (2165254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8394d2c16c073e488afc0a8227c3e05bd44de74400cf36a578b64da055f2ca`  
		Last Modified: Thu, 23 Jun 2022 21:06:16 GMT  
		Size: 8.7 MB (8721844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccb59cbdbee868f15c2773f93864618111b1aa9a4aebe6236359b3e852e8dc1`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:1.21.4-apache`

```console
$ docker pull backdrop@sha256:f8a73bc6e121962e16a559ea19d9ecddd86ba6e06c3a1076a045089a20a57d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:1.21.4-apache` - linux; amd64

```console
$ docker pull backdrop@sha256:79d166e914a528610e8ac5a57638d3b7eeca22b5bba19e5e38fd73c58c1c3e19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174331557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c020ca5ac8371986920c2cc852574e0dec788b104dd051b3a226c3349052370`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:12:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:12:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:12:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:29:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:03:55 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:04:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:04:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:05:59 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:06:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:06:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Jun 2022 23:06:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:06:00 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:06:00 GMT
EXPOSE 80
# Thu, 09 Jun 2022 23:06:00 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 01:49:36 GMT
RUN a2enmod rewrite
# Fri, 10 Jun 2022 01:50:31 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:50:31 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:50:34 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:50:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:50:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:50:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772088206f8568203e6d410d3b89fbe52c179aff6abed864eb98bbb88600a463`  
		Last Modified: Sat, 28 May 2022 09:51:08 GMT  
		Size: 19.2 MB (19247884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81c5474649ebdbc8488baf5cd66754f83eab0486a88885f482b0e7f964fdca`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a528527ae803d0d6a51823792cd9d053c716c464e181fe3ec3d727e54bb20`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344c792709d4e7f4afa7e649971be01278f6d6c5493960b7d273ca53baa33fef`  
		Last Modified: Thu, 09 Jun 2022 23:59:43 GMT  
		Size: 10.8 MB (10758865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9638273c35415584850d053ff0dceb792c0b27660e3b6a65d362d1844c2bc4`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec70638e42f38ff2ee5cd38c046b866641f774440b37d9a87a5b44bf3f87f15`  
		Last Modified: Thu, 09 Jun 2022 23:59:42 GMT  
		Size: 10.2 MB (10196959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f65f5bb3b0aa859ec22263310e7c741ae879d89cbe65875ab807becd2b47b`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55578a5ce5e8e0c1c142886375dcb25a36bc51a63022a7608728fb22f1447a32`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dd85b4dfa569330bd78e093419e92e53ac9b5cfe7f358d6bf7c8ab0ebb062d`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe783f7bb3462c718e445caac5a99184436d3feb0bd79ac96941e23df8a9a92a`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9df1fc0744f36fc399c45908866e8cf9c3d6d73b30376c92b906e0cf3dd377`  
		Last Modified: Fri, 10 Jun 2022 01:52:10 GMT  
		Size: 2.4 MB (2415102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17402dd1c5d82171bd169485c877a00fff3176ec4f520005d4581c69d3f1c2fb`  
		Last Modified: Fri, 10 Jun 2022 01:52:11 GMT  
		Size: 8.7 MB (8722847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dabfe686dbaa4a62a5be96d5738e3f7c6f192412fc272738833e8a3ca629cb`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:1.21.4-apache` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:eab024819e18d2058ce6ffb1253f9d86fb574b3e79cd3e6b5bd7b8b7c6ae2ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.2 MB (167164028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b284515cf0b3bcb500aef83801c927e84bb401bfb2c73efe9589aed7837abb14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 06:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 06:35:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 06:35:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 06:35:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:05:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:05:17 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:05:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:05:19 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:05:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:07:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:07:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:07:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 08:07:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:28 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:07:29 GMT
EXPOSE 80
# Thu, 23 Jun 2022 08:07:30 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 21:02:56 GMT
RUN a2enmod rewrite
# Thu, 23 Jun 2022 21:04:02 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:04:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:04:03 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:04:04 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:04:08 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:04:09 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:04:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c146af8093559f8941c628d5ba6b3d917b6632be0ef8db3f94bd273e5f8e5e`  
		Last Modified: Thu, 23 Jun 2022 08:32:16 GMT  
		Size: 18.9 MB (18942958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c65506677c18dabf6680677a4a00f319c51d98d01385906b98cb2bd042d30b3`  
		Last Modified: Thu, 23 Jun 2022 08:32:13 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231191daad959d9fc1c3e70aa102000ecac8dd110ae7c5fd92c78a6c7fbafc4a`  
		Last Modified: Thu, 23 Jun 2022 08:32:14 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8766dc7144bf701c42e8cb04829bae7df122e874c6d1c1fc6c3d28af3df3ed`  
		Last Modified: Thu, 23 Jun 2022 08:43:49 GMT  
		Size: 10.5 MB (10543172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8320e583eb8b3eef52b7f7485be9206078705fa7c83ebbdf58828c46976c9a`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0751df93b68c12d7177068c0f698221012dc784c57c6bb060e31ae01b067dfdb`  
		Last Modified: Thu, 23 Jun 2022 08:43:48 GMT  
		Size: 10.0 MB (9998952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf10f28ca9517e7b1024947097349b2a6336ea34dab98ff5ef5c482c41ba9f7`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963139f3ad32863502ea64c536e229e41aae110d402e69e80caa11aeda2b424f`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f56943bfdf6d984c7f842a24ffb8214b4f2c125ec4e43149e069346ff21c43`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482a0088f4fcccdc8b25ec4e0fb7dca684416af37a60ec29d9642f590d1c3560`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b55b12ae706ec4b391b77fb212708796ace940f853a5f0470b38e18c34579b2`  
		Last Modified: Thu, 23 Jun 2022 21:06:14 GMT  
		Size: 2.2 MB (2165254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8394d2c16c073e488afc0a8227c3e05bd44de74400cf36a578b64da055f2ca`  
		Last Modified: Thu, 23 Jun 2022 21:06:16 GMT  
		Size: 8.7 MB (8721844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccb59cbdbee868f15c2773f93864618111b1aa9a4aebe6236359b3e852e8dc1`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:1.21.4-fpm`

```console
$ docker pull backdrop@sha256:b873a38ba65356ddbf8e684d967806456859098cfdf9d84e50a64ba62ca41097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:1.21.4-fpm` - linux; amd64

```console
$ docker pull backdrop@sha256:e972c1e1f7b40a1f61990845838ad1878b76c7d31bfe092c5a40a28dbf6ff83c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170242929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77801adb9ebd00347b7bacbfd137886d183e2554220bff980607b213f383cc3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:27:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:01:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:01:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:08:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:08:45 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:08:45 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:08:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:08:46 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:08:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 09 Jun 2022 23:08:46 GMT
STOPSIGNAL SIGQUIT
# Thu, 09 Jun 2022 23:08:46 GMT
EXPOSE 9000
# Thu, 09 Jun 2022 23:08:46 GMT
CMD ["php-fpm"]
# Fri, 10 Jun 2022 01:51:38 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:51:38 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:51:38 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:51:38 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:51:41 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:51:41 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:51:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:51:41 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ae4909e013d6c9ba47bf5f505e50cfb156f69913a7d72ec7390aa0faeb3777`  
		Last Modified: Thu, 09 Jun 2022 23:59:00 GMT  
		Size: 10.7 MB (10737467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95442bcca7a2e1a29d317920308121f5c92ebda052c6aad6ae90729d73cb8ee9`  
		Last Modified: Thu, 09 Jun 2022 23:58:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d68ee1d2441e5f24572dcbad3e15601c94886c30a3adf79ff2db63bde4606`  
		Last Modified: Fri, 10 Jun 2022 00:00:10 GMT  
		Size: 25.4 MB (25396630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e25477785378c73db581fb8089c07a94886264839bcbd2d32d74b356bc9ebc`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae29a18256bb27c519d3140394afade3f6a0e1ccb08279f824e4257d226044f`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c566c8d5b21a27dcd8744b196148b5d59cf7d1146c3ac0887f2d22e6f469fbd1`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8575250f2bf8bcdb8a601a7e3c5474f688cedfc4e0f2348cec8124fa3f411f2b`  
		Last Modified: Fri, 10 Jun 2022 01:52:44 GMT  
		Size: 2.4 MB (2389845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c74b6b9c524b9cfca8911df221c0c7873e0d07f09457ad1e10cb16bc884d03`  
		Last Modified: Fri, 10 Jun 2022 01:52:45 GMT  
		Size: 8.7 MB (8722855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5b837e3f6d4f1820381b40e7aa08c04206fe1ecf11486add3e4babbaf36b0e`  
		Last Modified: Fri, 10 Jun 2022 01:52:43 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:1.21.4-fpm` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:b6f5ce0be872659bb100bcfc68307e28fcfc7cef5733a6e306026eca99dc3941
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.1 MB (163130320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4df60f59f68f3dc537eee832409a4b8d023a1afee88d0dd3018fc2ca5fd0ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:31:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:31:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:31:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:02:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:03:00 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:03:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:03:02 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:03:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:03:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:10:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:10:15 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:10:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:10:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:10:17 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:10:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Jun 2022 08:10:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jun 2022 08:10:20 GMT
EXPOSE 9000
# Thu, 23 Jun 2022 08:10:21 GMT
CMD ["php-fpm"]
# Thu, 23 Jun 2022 21:05:26 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:05:27 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:05:28 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:05:29 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:05:33 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:05:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:05:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:05:35 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3343549bd53bda328dd3b6a5488a1a92c86d260c73ff28e6b6a596fa1b521`  
		Last Modified: Thu, 23 Jun 2022 08:43:00 GMT  
		Size: 10.5 MB (10521113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b6c58fb818b8de29e436d358e87f11665f2ded5521370e61bbec68b1ddb494`  
		Last Modified: Thu, 23 Jun 2022 08:42:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d55d8e081af25f0bc7e97ae6b8c49840660259cf65b20366337a2670d1a3a1`  
		Last Modified: Thu, 23 Jun 2022 08:44:18 GMT  
		Size: 24.9 MB (24949587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f419449f189d35d6be08835101aeec77d7e0e0281b642b06a40e06e2a592667`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a2925453a4c8146fd5bbea9559d5c43da91dabe6ab0b0a6c413496f322b785`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b9a83719254b7a18c0cc13e03f834841bfa53fad61503f0ba887a4118cc526`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429e15ea917e05f1652db513507e8a1db34af024cbb28e8db5f1107688f944d1`  
		Last Modified: Thu, 23 Jun 2022 21:06:55 GMT  
		Size: 2.1 MB (2139603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470ef2c64313b66a3d97834c58b4be6388ce5b7afac7a50d06230ac57c02a6cc`  
		Last Modified: Thu, 23 Jun 2022 21:06:57 GMT  
		Size: 8.7 MB (8721845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5eb788bbd05267f8a8211286c7aa26df963d883f03d248415a1ecbc8bfc035`  
		Last Modified: Thu, 23 Jun 2022 21:06:54 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:apache`

```console
$ docker pull backdrop@sha256:f8a73bc6e121962e16a559ea19d9ecddd86ba6e06c3a1076a045089a20a57d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:apache` - linux; amd64

```console
$ docker pull backdrop@sha256:79d166e914a528610e8ac5a57638d3b7eeca22b5bba19e5e38fd73c58c1c3e19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174331557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c020ca5ac8371986920c2cc852574e0dec788b104dd051b3a226c3349052370`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:12:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:12:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:12:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:29:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:03:55 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:04:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:04:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:05:59 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:06:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:06:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Jun 2022 23:06:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:06:00 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:06:00 GMT
EXPOSE 80
# Thu, 09 Jun 2022 23:06:00 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 01:49:36 GMT
RUN a2enmod rewrite
# Fri, 10 Jun 2022 01:50:31 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:50:31 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:50:34 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:50:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:50:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:50:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772088206f8568203e6d410d3b89fbe52c179aff6abed864eb98bbb88600a463`  
		Last Modified: Sat, 28 May 2022 09:51:08 GMT  
		Size: 19.2 MB (19247884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81c5474649ebdbc8488baf5cd66754f83eab0486a88885f482b0e7f964fdca`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a528527ae803d0d6a51823792cd9d053c716c464e181fe3ec3d727e54bb20`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344c792709d4e7f4afa7e649971be01278f6d6c5493960b7d273ca53baa33fef`  
		Last Modified: Thu, 09 Jun 2022 23:59:43 GMT  
		Size: 10.8 MB (10758865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9638273c35415584850d053ff0dceb792c0b27660e3b6a65d362d1844c2bc4`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec70638e42f38ff2ee5cd38c046b866641f774440b37d9a87a5b44bf3f87f15`  
		Last Modified: Thu, 09 Jun 2022 23:59:42 GMT  
		Size: 10.2 MB (10196959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f65f5bb3b0aa859ec22263310e7c741ae879d89cbe65875ab807becd2b47b`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55578a5ce5e8e0c1c142886375dcb25a36bc51a63022a7608728fb22f1447a32`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dd85b4dfa569330bd78e093419e92e53ac9b5cfe7f358d6bf7c8ab0ebb062d`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe783f7bb3462c718e445caac5a99184436d3feb0bd79ac96941e23df8a9a92a`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9df1fc0744f36fc399c45908866e8cf9c3d6d73b30376c92b906e0cf3dd377`  
		Last Modified: Fri, 10 Jun 2022 01:52:10 GMT  
		Size: 2.4 MB (2415102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17402dd1c5d82171bd169485c877a00fff3176ec4f520005d4581c69d3f1c2fb`  
		Last Modified: Fri, 10 Jun 2022 01:52:11 GMT  
		Size: 8.7 MB (8722847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dabfe686dbaa4a62a5be96d5738e3f7c6f192412fc272738833e8a3ca629cb`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:apache` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:eab024819e18d2058ce6ffb1253f9d86fb574b3e79cd3e6b5bd7b8b7c6ae2ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.2 MB (167164028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b284515cf0b3bcb500aef83801c927e84bb401bfb2c73efe9589aed7837abb14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 06:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 06:35:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 06:35:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 06:35:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:05:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:05:17 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:05:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:05:19 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:05:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:07:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:07:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:07:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 08:07:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:28 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:07:29 GMT
EXPOSE 80
# Thu, 23 Jun 2022 08:07:30 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 21:02:56 GMT
RUN a2enmod rewrite
# Thu, 23 Jun 2022 21:04:02 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:04:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:04:03 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:04:04 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:04:08 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:04:09 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:04:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c146af8093559f8941c628d5ba6b3d917b6632be0ef8db3f94bd273e5f8e5e`  
		Last Modified: Thu, 23 Jun 2022 08:32:16 GMT  
		Size: 18.9 MB (18942958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c65506677c18dabf6680677a4a00f319c51d98d01385906b98cb2bd042d30b3`  
		Last Modified: Thu, 23 Jun 2022 08:32:13 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231191daad959d9fc1c3e70aa102000ecac8dd110ae7c5fd92c78a6c7fbafc4a`  
		Last Modified: Thu, 23 Jun 2022 08:32:14 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8766dc7144bf701c42e8cb04829bae7df122e874c6d1c1fc6c3d28af3df3ed`  
		Last Modified: Thu, 23 Jun 2022 08:43:49 GMT  
		Size: 10.5 MB (10543172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8320e583eb8b3eef52b7f7485be9206078705fa7c83ebbdf58828c46976c9a`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0751df93b68c12d7177068c0f698221012dc784c57c6bb060e31ae01b067dfdb`  
		Last Modified: Thu, 23 Jun 2022 08:43:48 GMT  
		Size: 10.0 MB (9998952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf10f28ca9517e7b1024947097349b2a6336ea34dab98ff5ef5c482c41ba9f7`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963139f3ad32863502ea64c536e229e41aae110d402e69e80caa11aeda2b424f`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f56943bfdf6d984c7f842a24ffb8214b4f2c125ec4e43149e069346ff21c43`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482a0088f4fcccdc8b25ec4e0fb7dca684416af37a60ec29d9642f590d1c3560`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b55b12ae706ec4b391b77fb212708796ace940f853a5f0470b38e18c34579b2`  
		Last Modified: Thu, 23 Jun 2022 21:06:14 GMT  
		Size: 2.2 MB (2165254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8394d2c16c073e488afc0a8227c3e05bd44de74400cf36a578b64da055f2ca`  
		Last Modified: Thu, 23 Jun 2022 21:06:16 GMT  
		Size: 8.7 MB (8721844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccb59cbdbee868f15c2773f93864618111b1aa9a4aebe6236359b3e852e8dc1`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:fpm`

```console
$ docker pull backdrop@sha256:b873a38ba65356ddbf8e684d967806456859098cfdf9d84e50a64ba62ca41097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:fpm` - linux; amd64

```console
$ docker pull backdrop@sha256:e972c1e1f7b40a1f61990845838ad1878b76c7d31bfe092c5a40a28dbf6ff83c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.2 MB (170242929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77801adb9ebd00347b7bacbfd137886d183e2554220bff980607b213f383cc3e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:09:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:27:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:01:46 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:01:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:01:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:08:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:08:45 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:08:45 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:08:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:08:46 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:08:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 09 Jun 2022 23:08:46 GMT
STOPSIGNAL SIGQUIT
# Thu, 09 Jun 2022 23:08:46 GMT
EXPOSE 9000
# Thu, 09 Jun 2022 23:08:46 GMT
CMD ["php-fpm"]
# Fri, 10 Jun 2022 01:51:38 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:51:38 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:51:38 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:51:38 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:51:41 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:51:41 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:51:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:51:41 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ae4909e013d6c9ba47bf5f505e50cfb156f69913a7d72ec7390aa0faeb3777`  
		Last Modified: Thu, 09 Jun 2022 23:59:00 GMT  
		Size: 10.7 MB (10737467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95442bcca7a2e1a29d317920308121f5c92ebda052c6aad6ae90729d73cb8ee9`  
		Last Modified: Thu, 09 Jun 2022 23:58:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2d68ee1d2441e5f24572dcbad3e15601c94886c30a3adf79ff2db63bde4606`  
		Last Modified: Fri, 10 Jun 2022 00:00:10 GMT  
		Size: 25.4 MB (25396630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e25477785378c73db581fb8089c07a94886264839bcbd2d32d74b356bc9ebc`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae29a18256bb27c519d3140394afade3f6a0e1ccb08279f824e4257d226044f`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c566c8d5b21a27dcd8744b196148b5d59cf7d1146c3ac0887f2d22e6f469fbd1`  
		Last Modified: Fri, 10 Jun 2022 00:00:07 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8575250f2bf8bcdb8a601a7e3c5474f688cedfc4e0f2348cec8124fa3f411f2b`  
		Last Modified: Fri, 10 Jun 2022 01:52:44 GMT  
		Size: 2.4 MB (2389845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c74b6b9c524b9cfca8911df221c0c7873e0d07f09457ad1e10cb16bc884d03`  
		Last Modified: Fri, 10 Jun 2022 01:52:45 GMT  
		Size: 8.7 MB (8722855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5b837e3f6d4f1820381b40e7aa08c04206fe1ecf11486add3e4babbaf36b0e`  
		Last Modified: Fri, 10 Jun 2022 01:52:43 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:fpm` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:b6f5ce0be872659bb100bcfc68307e28fcfc7cef5733a6e306026eca99dc3941
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.1 MB (163130320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4df60f59f68f3dc537eee832409a4b8d023a1afee88d0dd3018fc2ca5fd0ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:31:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:31:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:31:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:02:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:03:00 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:03:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:03:02 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:03:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:03:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:10:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:10:15 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:10:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:10:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:10:17 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:10:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Jun 2022 08:10:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Jun 2022 08:10:20 GMT
EXPOSE 9000
# Thu, 23 Jun 2022 08:10:21 GMT
CMD ["php-fpm"]
# Thu, 23 Jun 2022 21:05:26 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:05:27 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:05:28 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:05:29 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:05:33 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz 	&& echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c - 	&& tar -xz --strip-components=1 -f backdrop.tar.gz 	&& rm backdrop.tar.gz 	&& chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:05:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:05:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:05:35 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3343549bd53bda328dd3b6a5488a1a92c86d260c73ff28e6b6a596fa1b521`  
		Last Modified: Thu, 23 Jun 2022 08:43:00 GMT  
		Size: 10.5 MB (10521113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b6c58fb818b8de29e436d358e87f11665f2ded5521370e61bbec68b1ddb494`  
		Last Modified: Thu, 23 Jun 2022 08:42:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16d55d8e081af25f0bc7e97ae6b8c49840660259cf65b20366337a2670d1a3a1`  
		Last Modified: Thu, 23 Jun 2022 08:44:18 GMT  
		Size: 24.9 MB (24949587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f419449f189d35d6be08835101aeec77d7e0e0281b642b06a40e06e2a592667`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a2925453a4c8146fd5bbea9559d5c43da91dabe6ab0b0a6c413496f322b785`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b9a83719254b7a18c0cc13e03f834841bfa53fad61503f0ba887a4118cc526`  
		Last Modified: Thu, 23 Jun 2022 08:44:15 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429e15ea917e05f1652db513507e8a1db34af024cbb28e8db5f1107688f944d1`  
		Last Modified: Thu, 23 Jun 2022 21:06:55 GMT  
		Size: 2.1 MB (2139603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470ef2c64313b66a3d97834c58b4be6388ce5b7afac7a50d06230ac57c02a6cc`  
		Last Modified: Thu, 23 Jun 2022 21:06:57 GMT  
		Size: 8.7 MB (8721845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5eb788bbd05267f8a8211286c7aa26df963d883f03d248415a1ecbc8bfc035`  
		Last Modified: Thu, 23 Jun 2022 21:06:54 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `backdrop:latest`

```console
$ docker pull backdrop@sha256:f8a73bc6e121962e16a559ea19d9ecddd86ba6e06c3a1076a045089a20a57d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `backdrop:latest` - linux; amd64

```console
$ docker pull backdrop@sha256:79d166e914a528610e8ac5a57638d3b7eeca22b5bba19e5e38fd73c58c1c3e19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174331557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c020ca5ac8371986920c2cc852574e0dec788b104dd051b3a226c3349052370`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:12:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:12:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:12:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:29:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_VERSION=7.4.30
# Thu, 09 Jun 2022 23:03:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 09 Jun 2022 23:03:55 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 09 Jun 2022 23:04:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Jun 2022 23:04:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Jun 2022 23:05:59 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:05:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Jun 2022 23:06:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Jun 2022 23:06:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Jun 2022 23:06:00 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Jun 2022 23:06:00 GMT
WORKDIR /var/www/html
# Thu, 09 Jun 2022 23:06:00 GMT
EXPOSE 80
# Thu, 09 Jun 2022 23:06:00 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 01:49:36 GMT
RUN a2enmod rewrite
# Fri, 10 Jun 2022 01:50:31 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Fri, 10 Jun 2022 01:50:31 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_VERSION=1.21.4
# Fri, 10 Jun 2022 01:50:31 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Fri, 10 Jun 2022 01:50:34 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Fri, 10 Jun 2022 01:50:34 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Fri, 10 Jun 2022 01:50:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Jun 2022 01:50:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772088206f8568203e6d410d3b89fbe52c179aff6abed864eb98bbb88600a463`  
		Last Modified: Sat, 28 May 2022 09:51:08 GMT  
		Size: 19.2 MB (19247884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81c5474649ebdbc8488baf5cd66754f83eab0486a88885f482b0e7f964fdca`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a528527ae803d0d6a51823792cd9d053c716c464e181fe3ec3d727e54bb20`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344c792709d4e7f4afa7e649971be01278f6d6c5493960b7d273ca53baa33fef`  
		Last Modified: Thu, 09 Jun 2022 23:59:43 GMT  
		Size: 10.8 MB (10758865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9638273c35415584850d053ff0dceb792c0b27660e3b6a65d362d1844c2bc4`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec70638e42f38ff2ee5cd38c046b866641f774440b37d9a87a5b44bf3f87f15`  
		Last Modified: Thu, 09 Jun 2022 23:59:42 GMT  
		Size: 10.2 MB (10196959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f65f5bb3b0aa859ec22263310e7c741ae879d89cbe65875ab807becd2b47b`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55578a5ce5e8e0c1c142886375dcb25a36bc51a63022a7608728fb22f1447a32`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1dd85b4dfa569330bd78e093419e92e53ac9b5cfe7f358d6bf7c8ab0ebb062d`  
		Last Modified: Thu, 09 Jun 2022 23:59:40 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe783f7bb3462c718e445caac5a99184436d3feb0bd79ac96941e23df8a9a92a`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9df1fc0744f36fc399c45908866e8cf9c3d6d73b30376c92b906e0cf3dd377`  
		Last Modified: Fri, 10 Jun 2022 01:52:10 GMT  
		Size: 2.4 MB (2415102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17402dd1c5d82171bd169485c877a00fff3176ec4f520005d4581c69d3f1c2fb`  
		Last Modified: Fri, 10 Jun 2022 01:52:11 GMT  
		Size: 8.7 MB (8722847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dabfe686dbaa4a62a5be96d5738e3f7c6f192412fc272738833e8a3ca629cb`  
		Last Modified: Fri, 10 Jun 2022 01:52:09 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `backdrop:latest` - linux; arm64 variant v8

```console
$ docker pull backdrop@sha256:eab024819e18d2058ce6ffb1253f9d86fb574b3e79cd3e6b5bd7b8b7c6ae2ecf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.2 MB (167164028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b284515cf0b3bcb500aef83801c927e84bb401bfb2c73efe9589aed7837abb14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:43 GMT
ADD file:134be48af13f80f3474bf1b080ca781feb7b972148d482849862e55eb2acd61c in / 
# Thu, 23 Jun 2022 00:40:44 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 06:30:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Jun 2022 06:30:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Jun 2022 06:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 06:31:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Jun 2022 06:31:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Jun 2022 06:35:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Jun 2022 06:35:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Jun 2022 06:35:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Jun 2022 06:35:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Jun 2022 06:35:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Jun 2022 06:35:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Jun 2022 08:05:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jun 2022 08:05:17 GMT
ENV PHP_VERSION=7.4.30
# Thu, 23 Jun 2022 08:05:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Thu, 23 Jun 2022 08:05:19 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Thu, 23 Jun 2022 08:05:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Jun 2022 08:05:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 23 Jun 2022 08:07:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jun 2022 08:07:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jun 2022 08:07:26 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Jun 2022 08:07:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Jun 2022 08:07:28 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 08:07:29 GMT
EXPOSE 80
# Thu, 23 Jun 2022 08:07:30 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jun 2022 21:02:56 GMT
RUN a2enmod rewrite
# Thu, 23 Jun 2022 21:04:02 GMT
RUN apt-get update && apt-get install -y libzip-dev libonig-dev libpng-dev libjpeg-dev libpq-dev 	&& rm -rf /var/lib/apt/lists/* 	&& docker-php-ext-configure gd --with-jpeg=/usr 	&& docker-php-ext-install gd mbstring pdo pdo_mysql pdo_pgsql zip
# Thu, 23 Jun 2022 21:04:02 GMT
WORKDIR /var/www/html
# Thu, 23 Jun 2022 21:04:03 GMT
ENV BACKDROP_VERSION=1.21.4
# Thu, 23 Jun 2022 21:04:04 GMT
ENV BACKDROP_MD5=1540d9a42f429e29acc2e6a41cb4897c
# Thu, 23 Jun 2022 21:04:08 GMT
RUN curl -fSL "https://github.com/backdrop/backdrop/archive/${BACKDROP_VERSION}.tar.gz" -o backdrop.tar.gz   && echo "${BACKDROP_MD5} *backdrop.tar.gz" | md5sum -c -   && tar -xz --strip-components=1 -f backdrop.tar.gz   && rm backdrop.tar.gz   && chown -R www-data:www-data sites
# Thu, 23 Jun 2022 21:04:09 GMT
COPY file:dc282a331b642ab4cd043a874f505e04001cc1bdcf4f846fb117f413030d2835 in /entrypoint.sh 
# Thu, 23 Jun 2022 21:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jun 2022 21:04:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3b157c852f2736e12f09046f214fe5f6a0b1652bd860269b3988c92a197026e8`  
		Last Modified: Thu, 23 Jun 2022 00:47:22 GMT  
		Size: 30.1 MB (30065720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9064b3648c6a5f2cda0032f67b6f6465e24ae3a39b2e047c4322e4108aa647a`  
		Last Modified: Thu, 23 Jun 2022 08:31:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cda30062909c4a13c42faa2236e16b41c16f6483668beb8238555a45c37874`  
		Last Modified: Thu, 23 Jun 2022 08:31:41 GMT  
		Size: 86.7 MB (86719420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab96a6881fbce99f8cfaf433c36e67957f8655d9a2c83df569e1384e222b883`  
		Last Modified: Thu, 23 Jun 2022 08:31:27 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c146af8093559f8941c628d5ba6b3d917b6632be0ef8db3f94bd273e5f8e5e`  
		Last Modified: Thu, 23 Jun 2022 08:32:16 GMT  
		Size: 18.9 MB (18942958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c65506677c18dabf6680677a4a00f319c51d98d01385906b98cb2bd042d30b3`  
		Last Modified: Thu, 23 Jun 2022 08:32:13 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231191daad959d9fc1c3e70aa102000ecac8dd110ae7c5fd92c78a6c7fbafc4a`  
		Last Modified: Thu, 23 Jun 2022 08:32:14 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8766dc7144bf701c42e8cb04829bae7df122e874c6d1c1fc6c3d28af3df3ed`  
		Last Modified: Thu, 23 Jun 2022 08:43:49 GMT  
		Size: 10.5 MB (10543172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8320e583eb8b3eef52b7f7485be9206078705fa7c83ebbdf58828c46976c9a`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0751df93b68c12d7177068c0f698221012dc784c57c6bb060e31ae01b067dfdb`  
		Last Modified: Thu, 23 Jun 2022 08:43:48 GMT  
		Size: 10.0 MB (9998952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf10f28ca9517e7b1024947097349b2a6336ea34dab98ff5ef5c482c41ba9f7`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963139f3ad32863502ea64c536e229e41aae110d402e69e80caa11aeda2b424f`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f56943bfdf6d984c7f842a24ffb8214b4f2c125ec4e43149e069346ff21c43`  
		Last Modified: Thu, 23 Jun 2022 08:43:46 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482a0088f4fcccdc8b25ec4e0fb7dca684416af37a60ec29d9642f590d1c3560`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b55b12ae706ec4b391b77fb212708796ace940f853a5f0470b38e18c34579b2`  
		Last Modified: Thu, 23 Jun 2022 21:06:14 GMT  
		Size: 2.2 MB (2165254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8394d2c16c073e488afc0a8227c3e05bd44de74400cf36a578b64da055f2ca`  
		Last Modified: Thu, 23 Jun 2022 21:06:16 GMT  
		Size: 8.7 MB (8721844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccb59cbdbee868f15c2773f93864618111b1aa9a4aebe6236359b3e852e8dc1`  
		Last Modified: Thu, 23 Jun 2022 21:06:13 GMT  
		Size: 950.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
