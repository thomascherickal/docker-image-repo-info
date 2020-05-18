<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `mediawiki`

-	[`mediawiki:1.31`](#mediawiki131)
-	[`mediawiki:1.31.7`](#mediawiki1317)
-	[`mediawiki:1.33`](#mediawiki133)
-	[`mediawiki:1.33.3`](#mediawiki1333)
-	[`mediawiki:1.34`](#mediawiki134)
-	[`mediawiki:1.34.1`](#mediawiki1341)
-	[`mediawiki:latest`](#mediawikilatest)
-	[`mediawiki:legacy`](#mediawikilegacy)
-	[`mediawiki:legacylts`](#mediawikilegacylts)
-	[`mediawiki:lts`](#mediawikilts)
-	[`mediawiki:stable`](#mediawikistable)

## `mediawiki:1.31`

```console
$ docker pull mediawiki@sha256:5176842e2050332682288e83db7c341a83bfe4570f3fcd1ad898904a19c922e8
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
$ docker pull mediawiki@sha256:f675c8e6ca0a2dba64611b2a916e768145eba50a2689ef9c965a9dbb45b73556
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251882389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb9f6a83f744e7bf771f96d0dcd49a573b37cd4a7680aa88123402323e52c84b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 14:23:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 14:23:53 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 14:24:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 14:24:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 14:28:04 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 14:28:06 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 14:28:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 14:28:06 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 14:28:06 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:06 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 14:28:07 GMT
EXPOSE 80
# Fri, 15 May 2020 14:28:07 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:10:39 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:12:41 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 16:12:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e342cb20e11a1dd9d7c623fa9432bd079fde2b090476b3134baf0c21d40612a`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 12.6 MB (12648389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c591e1fe994da44df77bd8b6ad18ed428e3d1e7f76c83349d61cf8fa06beab4d`  
		Last Modified: Fri, 15 May 2020 15:11:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e231d94c7c66658f89cc128cad35ec1e8e08f2bba42fd7ca4c2d1933d66910ac`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 13.8 MB (13820369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16787fbb561735285d261bea91186df225573e4b193a7592d4ec49acc32d084`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf849c308b829343ad910dacfe26fea7cf2dfa9dbdc0b3f3a08e1c98222a0162`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d8b80f0c7f4669d6b6e1ed2ecff96de24ee0f969520b367f94df418d5156e0`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca082ed920d4a38e00a209eb7e17c1a8ae106cfe67ecf14accca6b19cb4f447`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea1efaf50e775702242a3eff9784b093e3600ed495d0d6a17a3a58801ff95a1`  
		Last Modified: Fri, 15 May 2020 16:13:49 GMT  
		Size: 64.4 MB (64438938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c31e8e8dd500a452bf4fb65bef4b53cb90b55104201023790cd8eb3b11fd1c9`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 2.8 MB (2780306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33dc37249be4cc31520a2516d4f67ade63354dc7ff49ad6b0e8673902bd54c3`  
		Last Modified: Fri, 15 May 2020 16:14:03 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f85ce9298260b76daa7b6ddcbe7e22e66d75a11e19000d172ee8fdf5ecd3a0c`  
		Last Modified: Fri, 15 May 2020 16:14:03 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b607dca168b949fbdad65fc55f6d5c9147a80b459ef8b31078ef8ad5658d6a`  
		Last Modified: Fri, 15 May 2020 16:14:14 GMT  
		Size: 35.8 MB (35761633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:181b23f356406ec27652ae93cdf04257f37209d4d3b8c53d4118accfc612ec29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226437533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cbd3309a5ba147b5c72762e94f49d101f5ee0c15ec30d55001f6ecfaea0f0b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:55:21 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 May 2020 23:55:22 GMT
ENV PHP_VERSION=7.2.31
# Thu, 14 May 2020 23:55:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Thu, 14 May 2020 23:55:25 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Thu, 14 May 2020 23:55:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:55:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:59:14 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:59:19 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:59:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:59:20 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:59:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:22 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:59:23 GMT
EXPOSE 80
# Thu, 14 May 2020 23:59:23 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:50:28 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:52:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:53:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:53:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:53:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 01:53:20 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 01:53:21 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 01:53:21 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 01:53:42 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6825e5831098a7455da6208d36a8631cf5e2823f499953e959a93d2825d216`  
		Last Modified: Fri, 15 May 2020 00:36:52 GMT  
		Size: 12.6 MB (12646387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c90c04c008327b286591e8e09268bce6fb4e7f4f23f3ecd5e756a8b4e5542`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a57b44810b99bff28e6eae7a26a7e63ee4096f279fbe1bfcf664e6273e41714`  
		Last Modified: Fri, 15 May 2020 00:36:53 GMT  
		Size: 12.9 MB (12893543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7a380e949112ca73a08930f495f01082945469b745a50ff5117e6694418b9`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019bfed0e017e52b99ae6700fd766ea74dcd69819f030e640cc2038a720a060e`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec0f544a95469ff33ebce02ed759bdab577bee1ecc6b52e27535b50190afe9d`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059248e2c7e804da9d7b61c6e9d1ca5845709a53347be8b1cd7323c6a38fcc26`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9be3987479af508dffc0cc23bcbacd781b00f13a165a4c554683d6ffde9d4b`  
		Last Modified: Fri, 15 May 2020 01:55:01 GMT  
		Size: 60.8 MB (60766733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57931c4fa281330d8a2a1e6f7ec30e9d57ca8dd99fda7147cdc0822b0be9d29e`  
		Last Modified: Fri, 15 May 2020 01:54:41 GMT  
		Size: 2.7 MB (2699845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d629bc11e6a1afbc207740507c6b99bc2ad69d629a6d4d3440e21e27e628b6`  
		Last Modified: Fri, 15 May 2020 01:55:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8221e24aea8426213ec533916ababeecfaeb20ca923a35facbf59429b2cb2716`  
		Last Modified: Fri, 15 May 2020 01:55:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a1ef64a11d60ac8a94e89b261e655dba843b0a07ab48eae4e2ac406b1be330`  
		Last Modified: Fri, 15 May 2020 01:55:27 GMT  
		Size: 35.8 MB (35762057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:bb45aad9d109c0cff5afb8609036166897fffbeaadcc796e3781ee83ece22187
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.0 MB (219970207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75d2cc7515ec9a1b95fd63c3e6b3010cbf907687f0250ec968f04fd67a427e61`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:35:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 05:35:19 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 05:35:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 05:35:21 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 05:35:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:35:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:38:37 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:38:40 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:38:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:38:42 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:38:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:43 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:38:43 GMT
EXPOSE 80
# Fri, 15 May 2020 05:38:44 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:37:32 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:39:55 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:39:56 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 07:39:57 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 07:39:57 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 07:39:58 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 07:40:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398113638833857603dca55979da57419d2a5572563cafe1334991af81967142`  
		Last Modified: Fri, 15 May 2020 06:10:24 GMT  
		Size: 12.6 MB (12646418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7959af5842bab4cdea3f1bb587ccf5276a5a9ec306f7549e37c48681732acc`  
		Last Modified: Fri, 15 May 2020 06:10:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ff876ade20645d6ddc3d2b59a603be87a04f0b62827c4665c3f132b44bb823`  
		Last Modified: Fri, 15 May 2020 06:10:25 GMT  
		Size: 12.2 MB (12163941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89eb8d735c9a88db8e9415f7968d824dea1e8ce48775e1f518eac6711f83aa5`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6835a065ff97b202cd23f0f4b753c4d136a169058eacad5989eff11767d592a`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385d20ac491870d83092377014337cc2858d8a8ad5fa34cc5ceb8127c81268d0`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8d5374463d9560454a440a6420fb6b8dfdac2ffe2094ce4390ada18219a7d`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36abbaec8998eb3a82a64613df5bc8258ec9a97630ef2e66abf147adbe44f836`  
		Last Modified: Fri, 15 May 2020 07:41:32 GMT  
		Size: 57.1 MB (57061094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44693c5b4c0ba701dc090f4d812ec58b9769563cd6a75d28d816fe64d1597d1c`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 2.6 MB (2641042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0bbdc1a3038c8e8bb6c476e51757e9e6127183edb412c913d112965f251144`  
		Last Modified: Fri, 15 May 2020 07:41:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5da091af18cb7439249bb6314c3caf4f208a378f3506025bd0aa5bb2fe7524`  
		Last Modified: Fri, 15 May 2020 07:41:42 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7dcf2d8bad80dde7b446926234306961b3c6ffd1ed2cc6ec1fc8944c964c`  
		Last Modified: Fri, 15 May 2020 07:42:01 GMT  
		Size: 35.8 MB (35762010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:787472e32803f153474046c3d6e8567242c5e4958aaa6be6fff30f3d3ee19eec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241693952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecc258368bab8df819d24c9023f2720c8393c3e4e16473cc708f030a2179dee`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:43:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 15:43:10 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 15:43:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 15:43:12 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 15:43:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:43:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:46:26 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:46:30 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:46:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:46:32 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:46:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:34 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:46:35 GMT
EXPOSE 80
# Fri, 15 May 2020 15:46:36 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:50:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:53:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:53:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:53:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 19:53:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 19:53:14 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 19:53:16 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 19:53:30 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87c94fdf28f180d95beba9bf62a84566232ed0ccc85839454cfe7f70498d39`  
		Last Modified: Fri, 15 May 2020 16:20:17 GMT  
		Size: 12.6 MB (12647169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd1d4d985393bba996ffbfdeeb1fc32bcb60b185e25e89516dc194d45c9bfee`  
		Last Modified: Fri, 15 May 2020 16:20:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfd1ad71cc2afd1e01539eec4fa66cb9041b028439a810dc8ef3462d6bfd9e3`  
		Last Modified: Fri, 15 May 2020 16:20:09 GMT  
		Size: 13.5 MB (13517080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1a76aeff57626d8acad75f39da3a39cc866b022ed90a6c743ba8e03ebf5bf`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91781f686504a79cb5c3a9ac44c847e82581db2bac375061f90aa7f401a1d38a`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a4c663a05696bf7ccb08382bef8932d7007cc3efae03cd914f100d1d33a074`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a5c61103dcbd74aed611a358358a9362c4e6da5b98ee8319bbb5b12552c697`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea3f778184af99b72385b780d7c9b4fbb5c9a001a764eada8da384a5bfbb5df`  
		Last Modified: Fri, 15 May 2020 19:54:38 GMT  
		Size: 62.2 MB (62238977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1daf0fab3fde127e7446d705cb687ab4511d7dc90edd8be244ccd98520a784f`  
		Last Modified: Fri, 15 May 2020 19:54:22 GMT  
		Size: 2.8 MB (2750463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d0ac654d18ee14a8dbed833a764067c883bf569686ffbb5891fca9eda6ae0b`  
		Last Modified: Fri, 15 May 2020 19:54:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa07d03ce00c5da6acb550c3867ca2ff5d5393ade79556196636b2e30478644`  
		Last Modified: Fri, 15 May 2020 19:54:45 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66840e504bf2520d1897c55db6fdc79c9149f3c1519209f0b703b3522211c877`  
		Last Modified: Fri, 15 May 2020 19:55:01 GMT  
		Size: 35.8 MB (35762208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31` - linux; 386

```console
$ docker pull mediawiki@sha256:1e6922f6fde549dddba1148486f1297f31b67bba9f38527dd5ed2e652b0fd540
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.8 MB (259785687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38de43bfa9877383e56d982f373037f3daa9c872b5946fab8954d1f316cd370d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:29:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 13:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:30:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:35:35 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:35:37 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:35:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:35:37 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:35:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:38 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:35:38 GMT
EXPOSE 80
# Fri, 15 May 2020 13:35:38 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:41:07 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:42:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:43:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:43:04 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:43:04 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 15:43:04 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 15:43:05 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 15:43:05 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 15:43:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14739e799f47da9c256b708f19578335422750fa82325e096a0fdbd0063dcd8`  
		Last Modified: Fri, 15 May 2020 14:35:18 GMT  
		Size: 12.6 MB (12647664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6602cc810aeb39612ffd93aaf08e6a834bd6a23306b89e007274aa317a9388e7`  
		Last Modified: Fri, 15 May 2020 14:35:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590038160b7b9aa93fbc6ca56843fce86d0f211c74e6f1ace6517f9743938740`  
		Last Modified: Fri, 15 May 2020 14:35:26 GMT  
		Size: 14.1 MB (14142560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f027994bbcc3b11ce489c8b38b2e60498e299fa93b3e7be031676c5cb44e5f37`  
		Last Modified: Fri, 15 May 2020 14:35:14 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aec20265c263a1cad53ad047b72af420de2ec322def253cc491fae7b2d9e6c4`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36479c1104bd5c974f4cf08ae38eb1c21dd1bc34c302c6134a0a5741b51d4efc`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5822ef93d09deb9b8d52cfb9e2ccda9b23b28b42c4c22de223caf7866f0b6081`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1ae57a5c23c1e2e03c3ff891870e6c4bcc5c08d9f12dc4f8d9632fe23a2cbd`  
		Last Modified: Fri, 15 May 2020 15:44:16 GMT  
		Size: 66.4 MB (66394484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a6b6b20b38b12032d751706bf19192545484b51348ea74aaff21a34cecd016`  
		Last Modified: Fri, 15 May 2020 15:43:56 GMT  
		Size: 2.8 MB (2767085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5300867f21fc2a48e18e2ca2d1cd7cf8c9e58670d402c7dca32d274035621e7`  
		Last Modified: Fri, 15 May 2020 15:44:22 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85f24a2d3c21d4a59299f89483535ba8cde0a2a00863559627e656945cb6144`  
		Last Modified: Fri, 15 May 2020 15:44:22 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495ece39a90aeb76c551073eb6bc952a847cb5194d17827b46d0f137204e9061`  
		Last Modified: Fri, 15 May 2020 15:44:40 GMT  
		Size: 35.8 MB (35761567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:1bff05c73642df000737e01db2fb4e09810834d0a4f84560a06da2a5bf70eb2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.0 MB (269988737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53d1b5abae3037bac89d9935218a2749efe7220bd3c01f115a902959b2606bfa`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 10:39:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Mon, 18 May 2020 10:39:45 GMT
ENV PHP_VERSION=7.2.31
# Mon, 18 May 2020 10:39:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Mon, 18 May 2020 10:39:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Mon, 18 May 2020 10:42:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 10:42:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 10:47:07 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:17 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 10:47:26 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 10:47:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 10:47:34 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 10:47:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:39 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 10:47:41 GMT
EXPOSE 80
# Mon, 18 May 2020 10:47:43 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:51:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:53:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:56:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:56:27 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:56:31 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Mon, 18 May 2020 19:56:33 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Mon, 18 May 2020 19:56:39 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Mon, 18 May 2020 19:56:42 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Mon, 18 May 2020 19:57:43 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422d598ad54ce6e95730222751503d9b698243cf90a702ad65e2d4631964790b`  
		Last Modified: Mon, 18 May 2020 12:30:00 GMT  
		Size: 12.6 MB (12648662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1981bd0a5f519849b6b58bcf91970f04a47d652e69fe60ac7ab816477283bb`  
		Last Modified: Mon, 18 May 2020 12:29:50 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a723077ecd7e1721f12f36dabd59b626018e3ed70e28d2933f8033c0885179`  
		Last Modified: Mon, 18 May 2020 12:30:08 GMT  
		Size: 14.9 MB (14857939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931596f7dd07359c094e8c5ce6911e9b4f4dd67bb1a11dec735da42f2507236d`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 2.2 KB (2235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cc1daefd84c15ae993c001ad437714bec6b0c7193b7974dd4bbc496d4d3741`  
		Last Modified: Mon, 18 May 2020 12:29:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666d43f8152a6bbf980f795024b39f5011f8a9f8c55f5d4053c973e9c4a1b43`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b330e8c37cbe3045afe862d0defb2365a798a12fceb4484dc2d0683819efa295`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922138725c394061a32405f8fb772954e20eb97e25a5d36c3f6655fc435f6b8`  
		Last Modified: Mon, 18 May 2020 20:02:56 GMT  
		Size: 71.3 MB (71260606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5203e563f1cf9a02c440e94ed4f6afb43648404a70e0916a8db25357f6809f1b`  
		Last Modified: Mon, 18 May 2020 20:01:30 GMT  
		Size: 2.9 MB (2855225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90beeed004f02c7c0a8ff240d4d4327a23ceb8a4171df2bcbfd5727e0dede5a3`  
		Last Modified: Mon, 18 May 2020 20:03:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705f0367663dcd4a8656e85075b3278da811124d25393476ef6b77d59112b04`  
		Last Modified: Mon, 18 May 2020 20:03:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f49dc71c3af4a18627392c2d8c683f005b09a5803bb6522cc4e1fed74f5d0e`  
		Last Modified: Mon, 18 May 2020 20:04:35 GMT  
		Size: 35.8 MB (35762126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:1.31.7`

```console
$ docker pull mediawiki@sha256:5176842e2050332682288e83db7c341a83bfe4570f3fcd1ad898904a19c922e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:1.31.7` - linux; amd64

```console
$ docker pull mediawiki@sha256:f675c8e6ca0a2dba64611b2a916e768145eba50a2689ef9c965a9dbb45b73556
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251882389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb9f6a83f744e7bf771f96d0dcd49a573b37cd4a7680aa88123402323e52c84b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 14:23:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 14:23:53 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 14:24:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 14:24:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 14:28:04 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 14:28:06 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 14:28:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 14:28:06 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 14:28:06 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:06 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 14:28:07 GMT
EXPOSE 80
# Fri, 15 May 2020 14:28:07 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:10:39 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:12:41 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 16:12:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e342cb20e11a1dd9d7c623fa9432bd079fde2b090476b3134baf0c21d40612a`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 12.6 MB (12648389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c591e1fe994da44df77bd8b6ad18ed428e3d1e7f76c83349d61cf8fa06beab4d`  
		Last Modified: Fri, 15 May 2020 15:11:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e231d94c7c66658f89cc128cad35ec1e8e08f2bba42fd7ca4c2d1933d66910ac`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 13.8 MB (13820369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16787fbb561735285d261bea91186df225573e4b193a7592d4ec49acc32d084`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf849c308b829343ad910dacfe26fea7cf2dfa9dbdc0b3f3a08e1c98222a0162`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d8b80f0c7f4669d6b6e1ed2ecff96de24ee0f969520b367f94df418d5156e0`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca082ed920d4a38e00a209eb7e17c1a8ae106cfe67ecf14accca6b19cb4f447`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea1efaf50e775702242a3eff9784b093e3600ed495d0d6a17a3a58801ff95a1`  
		Last Modified: Fri, 15 May 2020 16:13:49 GMT  
		Size: 64.4 MB (64438938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c31e8e8dd500a452bf4fb65bef4b53cb90b55104201023790cd8eb3b11fd1c9`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 2.8 MB (2780306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33dc37249be4cc31520a2516d4f67ade63354dc7ff49ad6b0e8673902bd54c3`  
		Last Modified: Fri, 15 May 2020 16:14:03 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f85ce9298260b76daa7b6ddcbe7e22e66d75a11e19000d172ee8fdf5ecd3a0c`  
		Last Modified: Fri, 15 May 2020 16:14:03 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b607dca168b949fbdad65fc55f6d5c9147a80b459ef8b31078ef8ad5658d6a`  
		Last Modified: Fri, 15 May 2020 16:14:14 GMT  
		Size: 35.8 MB (35761633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31.7` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:181b23f356406ec27652ae93cdf04257f37209d4d3b8c53d4118accfc612ec29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226437533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cbd3309a5ba147b5c72762e94f49d101f5ee0c15ec30d55001f6ecfaea0f0b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:55:21 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 May 2020 23:55:22 GMT
ENV PHP_VERSION=7.2.31
# Thu, 14 May 2020 23:55:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Thu, 14 May 2020 23:55:25 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Thu, 14 May 2020 23:55:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:55:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:59:14 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:59:19 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:59:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:59:20 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:59:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:22 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:59:23 GMT
EXPOSE 80
# Thu, 14 May 2020 23:59:23 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:50:28 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:52:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:53:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:53:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:53:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 01:53:20 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 01:53:21 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 01:53:21 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 01:53:42 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6825e5831098a7455da6208d36a8631cf5e2823f499953e959a93d2825d216`  
		Last Modified: Fri, 15 May 2020 00:36:52 GMT  
		Size: 12.6 MB (12646387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c90c04c008327b286591e8e09268bce6fb4e7f4f23f3ecd5e756a8b4e5542`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a57b44810b99bff28e6eae7a26a7e63ee4096f279fbe1bfcf664e6273e41714`  
		Last Modified: Fri, 15 May 2020 00:36:53 GMT  
		Size: 12.9 MB (12893543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7a380e949112ca73a08930f495f01082945469b745a50ff5117e6694418b9`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019bfed0e017e52b99ae6700fd766ea74dcd69819f030e640cc2038a720a060e`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec0f544a95469ff33ebce02ed759bdab577bee1ecc6b52e27535b50190afe9d`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059248e2c7e804da9d7b61c6e9d1ca5845709a53347be8b1cd7323c6a38fcc26`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9be3987479af508dffc0cc23bcbacd781b00f13a165a4c554683d6ffde9d4b`  
		Last Modified: Fri, 15 May 2020 01:55:01 GMT  
		Size: 60.8 MB (60766733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57931c4fa281330d8a2a1e6f7ec30e9d57ca8dd99fda7147cdc0822b0be9d29e`  
		Last Modified: Fri, 15 May 2020 01:54:41 GMT  
		Size: 2.7 MB (2699845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d629bc11e6a1afbc207740507c6b99bc2ad69d629a6d4d3440e21e27e628b6`  
		Last Modified: Fri, 15 May 2020 01:55:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8221e24aea8426213ec533916ababeecfaeb20ca923a35facbf59429b2cb2716`  
		Last Modified: Fri, 15 May 2020 01:55:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a1ef64a11d60ac8a94e89b261e655dba843b0a07ab48eae4e2ac406b1be330`  
		Last Modified: Fri, 15 May 2020 01:55:27 GMT  
		Size: 35.8 MB (35762057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31.7` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:bb45aad9d109c0cff5afb8609036166897fffbeaadcc796e3781ee83ece22187
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.0 MB (219970207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75d2cc7515ec9a1b95fd63c3e6b3010cbf907687f0250ec968f04fd67a427e61`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:35:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 05:35:19 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 05:35:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 05:35:21 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 05:35:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:35:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:38:37 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:38:40 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:38:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:38:42 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:38:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:43 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:38:43 GMT
EXPOSE 80
# Fri, 15 May 2020 05:38:44 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:37:32 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:39:55 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:39:56 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 07:39:57 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 07:39:57 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 07:39:58 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 07:40:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398113638833857603dca55979da57419d2a5572563cafe1334991af81967142`  
		Last Modified: Fri, 15 May 2020 06:10:24 GMT  
		Size: 12.6 MB (12646418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7959af5842bab4cdea3f1bb587ccf5276a5a9ec306f7549e37c48681732acc`  
		Last Modified: Fri, 15 May 2020 06:10:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ff876ade20645d6ddc3d2b59a603be87a04f0b62827c4665c3f132b44bb823`  
		Last Modified: Fri, 15 May 2020 06:10:25 GMT  
		Size: 12.2 MB (12163941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89eb8d735c9a88db8e9415f7968d824dea1e8ce48775e1f518eac6711f83aa5`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6835a065ff97b202cd23f0f4b753c4d136a169058eacad5989eff11767d592a`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385d20ac491870d83092377014337cc2858d8a8ad5fa34cc5ceb8127c81268d0`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8d5374463d9560454a440a6420fb6b8dfdac2ffe2094ce4390ada18219a7d`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36abbaec8998eb3a82a64613df5bc8258ec9a97630ef2e66abf147adbe44f836`  
		Last Modified: Fri, 15 May 2020 07:41:32 GMT  
		Size: 57.1 MB (57061094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44693c5b4c0ba701dc090f4d812ec58b9769563cd6a75d28d816fe64d1597d1c`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 2.6 MB (2641042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0bbdc1a3038c8e8bb6c476e51757e9e6127183edb412c913d112965f251144`  
		Last Modified: Fri, 15 May 2020 07:41:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5da091af18cb7439249bb6314c3caf4f208a378f3506025bd0aa5bb2fe7524`  
		Last Modified: Fri, 15 May 2020 07:41:42 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7dcf2d8bad80dde7b446926234306961b3c6ffd1ed2cc6ec1fc8944c964c`  
		Last Modified: Fri, 15 May 2020 07:42:01 GMT  
		Size: 35.8 MB (35762010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31.7` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:787472e32803f153474046c3d6e8567242c5e4958aaa6be6fff30f3d3ee19eec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241693952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecc258368bab8df819d24c9023f2720c8393c3e4e16473cc708f030a2179dee`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:43:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 15:43:10 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 15:43:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 15:43:12 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 15:43:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:43:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:46:26 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:46:30 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:46:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:46:32 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:46:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:34 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:46:35 GMT
EXPOSE 80
# Fri, 15 May 2020 15:46:36 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:50:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:53:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:53:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:53:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 19:53:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 19:53:14 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 19:53:16 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 19:53:30 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87c94fdf28f180d95beba9bf62a84566232ed0ccc85839454cfe7f70498d39`  
		Last Modified: Fri, 15 May 2020 16:20:17 GMT  
		Size: 12.6 MB (12647169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd1d4d985393bba996ffbfdeeb1fc32bcb60b185e25e89516dc194d45c9bfee`  
		Last Modified: Fri, 15 May 2020 16:20:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfd1ad71cc2afd1e01539eec4fa66cb9041b028439a810dc8ef3462d6bfd9e3`  
		Last Modified: Fri, 15 May 2020 16:20:09 GMT  
		Size: 13.5 MB (13517080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1a76aeff57626d8acad75f39da3a39cc866b022ed90a6c743ba8e03ebf5bf`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91781f686504a79cb5c3a9ac44c847e82581db2bac375061f90aa7f401a1d38a`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a4c663a05696bf7ccb08382bef8932d7007cc3efae03cd914f100d1d33a074`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a5c61103dcbd74aed611a358358a9362c4e6da5b98ee8319bbb5b12552c697`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea3f778184af99b72385b780d7c9b4fbb5c9a001a764eada8da384a5bfbb5df`  
		Last Modified: Fri, 15 May 2020 19:54:38 GMT  
		Size: 62.2 MB (62238977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1daf0fab3fde127e7446d705cb687ab4511d7dc90edd8be244ccd98520a784f`  
		Last Modified: Fri, 15 May 2020 19:54:22 GMT  
		Size: 2.8 MB (2750463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d0ac654d18ee14a8dbed833a764067c883bf569686ffbb5891fca9eda6ae0b`  
		Last Modified: Fri, 15 May 2020 19:54:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa07d03ce00c5da6acb550c3867ca2ff5d5393ade79556196636b2e30478644`  
		Last Modified: Fri, 15 May 2020 19:54:45 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66840e504bf2520d1897c55db6fdc79c9149f3c1519209f0b703b3522211c877`  
		Last Modified: Fri, 15 May 2020 19:55:01 GMT  
		Size: 35.8 MB (35762208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31.7` - linux; 386

```console
$ docker pull mediawiki@sha256:1e6922f6fde549dddba1148486f1297f31b67bba9f38527dd5ed2e652b0fd540
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.8 MB (259785687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38de43bfa9877383e56d982f373037f3daa9c872b5946fab8954d1f316cd370d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:29:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 13:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:30:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:35:35 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:35:37 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:35:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:35:37 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:35:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:38 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:35:38 GMT
EXPOSE 80
# Fri, 15 May 2020 13:35:38 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:41:07 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:42:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:43:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:43:04 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:43:04 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 15:43:04 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 15:43:05 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 15:43:05 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 15:43:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14739e799f47da9c256b708f19578335422750fa82325e096a0fdbd0063dcd8`  
		Last Modified: Fri, 15 May 2020 14:35:18 GMT  
		Size: 12.6 MB (12647664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6602cc810aeb39612ffd93aaf08e6a834bd6a23306b89e007274aa317a9388e7`  
		Last Modified: Fri, 15 May 2020 14:35:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590038160b7b9aa93fbc6ca56843fce86d0f211c74e6f1ace6517f9743938740`  
		Last Modified: Fri, 15 May 2020 14:35:26 GMT  
		Size: 14.1 MB (14142560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f027994bbcc3b11ce489c8b38b2e60498e299fa93b3e7be031676c5cb44e5f37`  
		Last Modified: Fri, 15 May 2020 14:35:14 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aec20265c263a1cad53ad047b72af420de2ec322def253cc491fae7b2d9e6c4`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36479c1104bd5c974f4cf08ae38eb1c21dd1bc34c302c6134a0a5741b51d4efc`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5822ef93d09deb9b8d52cfb9e2ccda9b23b28b42c4c22de223caf7866f0b6081`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1ae57a5c23c1e2e03c3ff891870e6c4bcc5c08d9f12dc4f8d9632fe23a2cbd`  
		Last Modified: Fri, 15 May 2020 15:44:16 GMT  
		Size: 66.4 MB (66394484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a6b6b20b38b12032d751706bf19192545484b51348ea74aaff21a34cecd016`  
		Last Modified: Fri, 15 May 2020 15:43:56 GMT  
		Size: 2.8 MB (2767085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5300867f21fc2a48e18e2ca2d1cd7cf8c9e58670d402c7dca32d274035621e7`  
		Last Modified: Fri, 15 May 2020 15:44:22 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85f24a2d3c21d4a59299f89483535ba8cde0a2a00863559627e656945cb6144`  
		Last Modified: Fri, 15 May 2020 15:44:22 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495ece39a90aeb76c551073eb6bc952a847cb5194d17827b46d0f137204e9061`  
		Last Modified: Fri, 15 May 2020 15:44:40 GMT  
		Size: 35.8 MB (35761567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.31.7` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:1bff05c73642df000737e01db2fb4e09810834d0a4f84560a06da2a5bf70eb2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.0 MB (269988737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53d1b5abae3037bac89d9935218a2749efe7220bd3c01f115a902959b2606bfa`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 10:39:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Mon, 18 May 2020 10:39:45 GMT
ENV PHP_VERSION=7.2.31
# Mon, 18 May 2020 10:39:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Mon, 18 May 2020 10:39:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Mon, 18 May 2020 10:42:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 10:42:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 10:47:07 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:17 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 10:47:26 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 10:47:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 10:47:34 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 10:47:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:39 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 10:47:41 GMT
EXPOSE 80
# Mon, 18 May 2020 10:47:43 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:51:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:53:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:56:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:56:27 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:56:31 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Mon, 18 May 2020 19:56:33 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Mon, 18 May 2020 19:56:39 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Mon, 18 May 2020 19:56:42 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Mon, 18 May 2020 19:57:43 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422d598ad54ce6e95730222751503d9b698243cf90a702ad65e2d4631964790b`  
		Last Modified: Mon, 18 May 2020 12:30:00 GMT  
		Size: 12.6 MB (12648662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1981bd0a5f519849b6b58bcf91970f04a47d652e69fe60ac7ab816477283bb`  
		Last Modified: Mon, 18 May 2020 12:29:50 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a723077ecd7e1721f12f36dabd59b626018e3ed70e28d2933f8033c0885179`  
		Last Modified: Mon, 18 May 2020 12:30:08 GMT  
		Size: 14.9 MB (14857939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931596f7dd07359c094e8c5ce6911e9b4f4dd67bb1a11dec735da42f2507236d`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 2.2 KB (2235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cc1daefd84c15ae993c001ad437714bec6b0c7193b7974dd4bbc496d4d3741`  
		Last Modified: Mon, 18 May 2020 12:29:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666d43f8152a6bbf980f795024b39f5011f8a9f8c55f5d4053c973e9c4a1b43`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b330e8c37cbe3045afe862d0defb2365a798a12fceb4484dc2d0683819efa295`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922138725c394061a32405f8fb772954e20eb97e25a5d36c3f6655fc435f6b8`  
		Last Modified: Mon, 18 May 2020 20:02:56 GMT  
		Size: 71.3 MB (71260606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5203e563f1cf9a02c440e94ed4f6afb43648404a70e0916a8db25357f6809f1b`  
		Last Modified: Mon, 18 May 2020 20:01:30 GMT  
		Size: 2.9 MB (2855225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90beeed004f02c7c0a8ff240d4d4327a23ceb8a4171df2bcbfd5727e0dede5a3`  
		Last Modified: Mon, 18 May 2020 20:03:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705f0367663dcd4a8656e85075b3278da811124d25393476ef6b77d59112b04`  
		Last Modified: Mon, 18 May 2020 20:03:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f49dc71c3af4a18627392c2d8c683f005b09a5803bb6522cc4e1fed74f5d0e`  
		Last Modified: Mon, 18 May 2020 20:04:35 GMT  
		Size: 35.8 MB (35762126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:1.33`

```console
$ docker pull mediawiki@sha256:10054842db0f529ec6eb2bb4aad454048ad9b3ee3b3b851c806f11973502728e
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
$ docker pull mediawiki@sha256:a36de3946e6a63a79f2f227385247be84f2bc2ecec9557ed2071f37ae76b54b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254524143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d0fa04e7669cd74c7411a9c921f1fd10fa10bcaef4754242e0722d0df4eaa51`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 14:23:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 14:23:53 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 14:24:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 14:24:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 14:28:04 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 14:28:06 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 14:28:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 14:28:06 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 14:28:06 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:06 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 14:28:07 GMT
EXPOSE 80
# Fri, 15 May 2020 14:28:07 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:10:39 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:09 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 16:12:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:12:10 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 16:12:20 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e342cb20e11a1dd9d7c623fa9432bd079fde2b090476b3134baf0c21d40612a`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 12.6 MB (12648389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c591e1fe994da44df77bd8b6ad18ed428e3d1e7f76c83349d61cf8fa06beab4d`  
		Last Modified: Fri, 15 May 2020 15:11:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e231d94c7c66658f89cc128cad35ec1e8e08f2bba42fd7ca4c2d1933d66910ac`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 13.8 MB (13820369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16787fbb561735285d261bea91186df225573e4b193a7592d4ec49acc32d084`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf849c308b829343ad910dacfe26fea7cf2dfa9dbdc0b3f3a08e1c98222a0162`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d8b80f0c7f4669d6b6e1ed2ecff96de24ee0f969520b367f94df418d5156e0`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca082ed920d4a38e00a209eb7e17c1a8ae106cfe67ecf14accca6b19cb4f447`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea1efaf50e775702242a3eff9784b093e3600ed495d0d6a17a3a58801ff95a1`  
		Last Modified: Fri, 15 May 2020 16:13:49 GMT  
		Size: 64.4 MB (64438938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c31e8e8dd500a452bf4fb65bef4b53cb90b55104201023790cd8eb3b11fd1c9`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 2.8 MB (2780306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192dddd32079e34822616719acd1fefbc9e131f8768410a96134e6990992c6ab`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cedc0546fa17b6cc3a6567871c6258482079f0650a8a365e9c6772f419260c`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003e0cd48706b86851b9ac0f0596091925f18ec14074f01e8d3af460185888f8`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f65bf195377180a6b771652637ee9aa80466f99940086e63ac1e653e9542c8`  
		Last Modified: Fri, 15 May 2020 16:13:57 GMT  
		Size: 38.4 MB (38402810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:2270a1d8b14b964ee92adebd289d3dc4a107c8c39e44341bf78053f31d269ceb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229079502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5132c469c486d6a880123ccc7a40cb0ae6cf08ecdc48b3e8254849feb9d9782`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:55:21 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 May 2020 23:55:22 GMT
ENV PHP_VERSION=7.2.31
# Thu, 14 May 2020 23:55:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Thu, 14 May 2020 23:55:25 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Thu, 14 May 2020 23:55:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:55:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:59:14 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:59:19 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:59:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:59:20 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:59:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:22 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:59:23 GMT
EXPOSE 80
# Thu, 14 May 2020 23:59:23 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:50:28 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:52:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:52:25 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 01:52:30 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:52:34 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:52:35 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 01:52:36 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 01:52:36 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 01:52:37 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 01:52:57 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6825e5831098a7455da6208d36a8631cf5e2823f499953e959a93d2825d216`  
		Last Modified: Fri, 15 May 2020 00:36:52 GMT  
		Size: 12.6 MB (12646387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c90c04c008327b286591e8e09268bce6fb4e7f4f23f3ecd5e756a8b4e5542`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a57b44810b99bff28e6eae7a26a7e63ee4096f279fbe1bfcf664e6273e41714`  
		Last Modified: Fri, 15 May 2020 00:36:53 GMT  
		Size: 12.9 MB (12893543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7a380e949112ca73a08930f495f01082945469b745a50ff5117e6694418b9`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019bfed0e017e52b99ae6700fd766ea74dcd69819f030e640cc2038a720a060e`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec0f544a95469ff33ebce02ed759bdab577bee1ecc6b52e27535b50190afe9d`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059248e2c7e804da9d7b61c6e9d1ca5845709a53347be8b1cd7323c6a38fcc26`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9be3987479af508dffc0cc23bcbacd781b00f13a165a4c554683d6ffde9d4b`  
		Last Modified: Fri, 15 May 2020 01:55:01 GMT  
		Size: 60.8 MB (60766733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57931c4fa281330d8a2a1e6f7ec30e9d57ca8dd99fda7147cdc0822b0be9d29e`  
		Last Modified: Fri, 15 May 2020 01:54:41 GMT  
		Size: 2.7 MB (2699845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9d9d0c3e509622625df75c6956819df8d94dc4efe60bc12221399a4aaa2a8f`  
		Last Modified: Fri, 15 May 2020 01:54:39 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420af56ef82b61aaf3bfe800975a82585a2d4f95a3139c580182df458585d30c`  
		Last Modified: Fri, 15 May 2020 01:54:39 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b10a569dd7c667c16369563975aeab457b7660090b955c29323ccddb104e6f`  
		Last Modified: Fri, 15 May 2020 01:54:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ef5c668ab603bacf087dd6f5ed5658d660840ce2d851d754dff659a363a557`  
		Last Modified: Fri, 15 May 2020 01:55:02 GMT  
		Size: 38.4 MB (38403453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:e8a9a86c49a8ad2e6aadec2935928841a3cef59325877b8e522dd382486f181c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222612271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cd306da7ed80ba57048f02a0b87e09dd48a3181fd63cb1dc81d59486d7a3bf`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:35:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 05:35:19 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 05:35:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 05:35:21 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 05:35:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:35:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:38:37 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:38:40 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:38:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:38:42 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:38:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:43 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:38:43 GMT
EXPOSE 80
# Fri, 15 May 2020 05:38:44 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:37:32 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:04 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 07:39:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:39:08 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:39:09 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 07:39:10 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 07:39:10 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 07:39:11 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 07:39:29 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398113638833857603dca55979da57419d2a5572563cafe1334991af81967142`  
		Last Modified: Fri, 15 May 2020 06:10:24 GMT  
		Size: 12.6 MB (12646418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7959af5842bab4cdea3f1bb587ccf5276a5a9ec306f7549e37c48681732acc`  
		Last Modified: Fri, 15 May 2020 06:10:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ff876ade20645d6ddc3d2b59a603be87a04f0b62827c4665c3f132b44bb823`  
		Last Modified: Fri, 15 May 2020 06:10:25 GMT  
		Size: 12.2 MB (12163941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89eb8d735c9a88db8e9415f7968d824dea1e8ce48775e1f518eac6711f83aa5`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6835a065ff97b202cd23f0f4b753c4d136a169058eacad5989eff11767d592a`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385d20ac491870d83092377014337cc2858d8a8ad5fa34cc5ceb8127c81268d0`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8d5374463d9560454a440a6420fb6b8dfdac2ffe2094ce4390ada18219a7d`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36abbaec8998eb3a82a64613df5bc8258ec9a97630ef2e66abf147adbe44f836`  
		Last Modified: Fri, 15 May 2020 07:41:32 GMT  
		Size: 57.1 MB (57061094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44693c5b4c0ba701dc090f4d812ec58b9769563cd6a75d28d816fe64d1597d1c`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 2.6 MB (2641042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a3c86c58739652e9de2c8ecbf1e6e35f2c35ed2e6bf156d9d7a62f9cdbf5e5`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8f091a3b5fca4a79e6ffdcbaa8f9e3446d93e47fbaaeac6f7be06496aac304`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db86b61467cc5ae06108add0b6e9faa34057e54e5b75174719030e638d7515f0`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d27738bd4597b81957110b74009136505b651c924174ee601609ecd31a702a5`  
		Last Modified: Fri, 15 May 2020 07:41:34 GMT  
		Size: 38.4 MB (38403499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:509a4979bbebf3c5ae72c6ef4728e37694b3f86062c8ad3716e7a9304cc9af72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244335715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3746c3e8043df9aa0e0343feebeddeb7408372b75d6918e69703cf63d169d1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:43:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 15:43:10 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 15:43:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 15:43:12 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 15:43:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:43:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:46:26 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:46:30 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:46:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:46:32 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:46:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:34 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:46:35 GMT
EXPOSE 80
# Fri, 15 May 2020 15:46:36 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:50:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:52:22 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 19:52:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:52:31 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:52:33 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 19:52:34 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 19:52:35 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 19:52:37 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 19:52:53 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87c94fdf28f180d95beba9bf62a84566232ed0ccc85839454cfe7f70498d39`  
		Last Modified: Fri, 15 May 2020 16:20:17 GMT  
		Size: 12.6 MB (12647169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd1d4d985393bba996ffbfdeeb1fc32bcb60b185e25e89516dc194d45c9bfee`  
		Last Modified: Fri, 15 May 2020 16:20:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfd1ad71cc2afd1e01539eec4fa66cb9041b028439a810dc8ef3462d6bfd9e3`  
		Last Modified: Fri, 15 May 2020 16:20:09 GMT  
		Size: 13.5 MB (13517080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1a76aeff57626d8acad75f39da3a39cc866b022ed90a6c743ba8e03ebf5bf`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91781f686504a79cb5c3a9ac44c847e82581db2bac375061f90aa7f401a1d38a`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a4c663a05696bf7ccb08382bef8932d7007cc3efae03cd914f100d1d33a074`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a5c61103dcbd74aed611a358358a9362c4e6da5b98ee8319bbb5b12552c697`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea3f778184af99b72385b780d7c9b4fbb5c9a001a764eada8da384a5bfbb5df`  
		Last Modified: Fri, 15 May 2020 19:54:38 GMT  
		Size: 62.2 MB (62238977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1daf0fab3fde127e7446d705cb687ab4511d7dc90edd8be244ccd98520a784f`  
		Last Modified: Fri, 15 May 2020 19:54:22 GMT  
		Size: 2.8 MB (2750463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c60cb45c44a2faf1f864c69adc336270f443061019e4b3b267389f138020ff`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5455d0d0523c81d6f2c76e08cdb1e8e9f6830e37a40368eed77b3428100685f`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0720228b8c502db5f6f28ea9f85591e21d230bf46730e26e35779d494049c9a`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9852953c9e00820f8805e237d72cafb452a1504c545de30aa187853ea39becc3`  
		Last Modified: Fri, 15 May 2020 19:54:38 GMT  
		Size: 38.4 MB (38403380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33` - linux; 386

```console
$ docker pull mediawiki@sha256:f8a9293db17f62717827b38c8d48516b8d5c9fd335467a044b41d40e8b673a1c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262427724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e1889e89992fab31e7c0ff4c5108e3e91869d568faf645b59a8726f78c8267`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:29:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 13:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:30:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:35:35 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:35:37 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:35:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:35:37 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:35:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:38 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:35:38 GMT
EXPOSE 80
# Fri, 15 May 2020 13:35:38 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:41:07 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:42:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:42:40 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 15:42:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:42:42 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 15:42:55 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14739e799f47da9c256b708f19578335422750fa82325e096a0fdbd0063dcd8`  
		Last Modified: Fri, 15 May 2020 14:35:18 GMT  
		Size: 12.6 MB (12647664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6602cc810aeb39612ffd93aaf08e6a834bd6a23306b89e007274aa317a9388e7`  
		Last Modified: Fri, 15 May 2020 14:35:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590038160b7b9aa93fbc6ca56843fce86d0f211c74e6f1ace6517f9743938740`  
		Last Modified: Fri, 15 May 2020 14:35:26 GMT  
		Size: 14.1 MB (14142560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f027994bbcc3b11ce489c8b38b2e60498e299fa93b3e7be031676c5cb44e5f37`  
		Last Modified: Fri, 15 May 2020 14:35:14 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aec20265c263a1cad53ad047b72af420de2ec322def253cc491fae7b2d9e6c4`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36479c1104bd5c974f4cf08ae38eb1c21dd1bc34c302c6134a0a5741b51d4efc`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5822ef93d09deb9b8d52cfb9e2ccda9b23b28b42c4c22de223caf7866f0b6081`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1ae57a5c23c1e2e03c3ff891870e6c4bcc5c08d9f12dc4f8d9632fe23a2cbd`  
		Last Modified: Fri, 15 May 2020 15:44:16 GMT  
		Size: 66.4 MB (66394484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a6b6b20b38b12032d751706bf19192545484b51348ea74aaff21a34cecd016`  
		Last Modified: Fri, 15 May 2020 15:43:56 GMT  
		Size: 2.8 MB (2767085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310cc8fe6502e5085d087942e895e66941521dc9e24d4e98b674e45005113fae`  
		Last Modified: Fri, 15 May 2020 15:43:55 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a854515df625c06ba3321bce8ff4c910fac6c639d736cf7cdd66e1a88adab36`  
		Last Modified: Fri, 15 May 2020 15:43:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac1ba4a1ebfce49416ed9341a80f27861585759fcda5895932f9fe3dccc54e7`  
		Last Modified: Fri, 15 May 2020 15:43:55 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e40562f13215b7bbce03df57f3d700cb4618dcf01361e2a5f170055101cb5a0`  
		Last Modified: Fri, 15 May 2020 15:44:13 GMT  
		Size: 38.4 MB (38403029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:b37cdbf4c4a9f1d71077a9045d6338164b96677e00d2d6a1846c7616723eaba3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272630469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fdb9d5a9d4eb3d5fdb5bc0f328473ae021ac26abe6bb132051380bdfeee1fad`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 10:39:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Mon, 18 May 2020 10:39:45 GMT
ENV PHP_VERSION=7.2.31
# Mon, 18 May 2020 10:39:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Mon, 18 May 2020 10:39:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Mon, 18 May 2020 10:42:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 10:42:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 10:47:07 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:17 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 10:47:26 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 10:47:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 10:47:34 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 10:47:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:39 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 10:47:41 GMT
EXPOSE 80
# Mon, 18 May 2020 10:47:43 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:51:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:53:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:53:58 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Mon, 18 May 2020 19:54:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:54:20 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:54:24 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Mon, 18 May 2020 19:54:26 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Mon, 18 May 2020 19:54:33 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Mon, 18 May 2020 19:54:42 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Mon, 18 May 2020 19:55:27 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422d598ad54ce6e95730222751503d9b698243cf90a702ad65e2d4631964790b`  
		Last Modified: Mon, 18 May 2020 12:30:00 GMT  
		Size: 12.6 MB (12648662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1981bd0a5f519849b6b58bcf91970f04a47d652e69fe60ac7ab816477283bb`  
		Last Modified: Mon, 18 May 2020 12:29:50 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a723077ecd7e1721f12f36dabd59b626018e3ed70e28d2933f8033c0885179`  
		Last Modified: Mon, 18 May 2020 12:30:08 GMT  
		Size: 14.9 MB (14857939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931596f7dd07359c094e8c5ce6911e9b4f4dd67bb1a11dec735da42f2507236d`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 2.2 KB (2235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cc1daefd84c15ae993c001ad437714bec6b0c7193b7974dd4bbc496d4d3741`  
		Last Modified: Mon, 18 May 2020 12:29:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666d43f8152a6bbf980f795024b39f5011f8a9f8c55f5d4053c973e9c4a1b43`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b330e8c37cbe3045afe862d0defb2365a798a12fceb4484dc2d0683819efa295`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922138725c394061a32405f8fb772954e20eb97e25a5d36c3f6655fc435f6b8`  
		Last Modified: Mon, 18 May 2020 20:02:56 GMT  
		Size: 71.3 MB (71260606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5203e563f1cf9a02c440e94ed4f6afb43648404a70e0916a8db25357f6809f1b`  
		Last Modified: Mon, 18 May 2020 20:01:30 GMT  
		Size: 2.9 MB (2855225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efd3e6ea5dbeec916c6410d03d6f17b4eac74582b7b7ca78ea4eae5b24430e`  
		Last Modified: Mon, 18 May 2020 20:01:25 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7ec02c6577c567385cc72505ac006b3f6c5c2abd54ac5c95a3df382eecf888`  
		Last Modified: Mon, 18 May 2020 20:01:26 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dde02b1527ca67ce7a4d212825417c27bb340054f4c54951bca032fbc767fd9`  
		Last Modified: Mon, 18 May 2020 20:01:26 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2de52b8e356a6abd3d1871df0c97dfdce7d4f199862bc7286b03d5c54eb5bd`  
		Last Modified: Mon, 18 May 2020 20:03:13 GMT  
		Size: 38.4 MB (38403277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:1.33.3`

```console
$ docker pull mediawiki@sha256:10054842db0f529ec6eb2bb4aad454048ad9b3ee3b3b851c806f11973502728e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:1.33.3` - linux; amd64

```console
$ docker pull mediawiki@sha256:a36de3946e6a63a79f2f227385247be84f2bc2ecec9557ed2071f37ae76b54b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254524143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d0fa04e7669cd74c7411a9c921f1fd10fa10bcaef4754242e0722d0df4eaa51`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 14:23:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 14:23:53 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 14:24:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 14:24:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 14:28:04 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 14:28:06 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 14:28:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 14:28:06 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 14:28:06 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:06 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 14:28:07 GMT
EXPOSE 80
# Fri, 15 May 2020 14:28:07 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:10:39 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:09 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 16:12:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:12:10 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 16:12:20 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e342cb20e11a1dd9d7c623fa9432bd079fde2b090476b3134baf0c21d40612a`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 12.6 MB (12648389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c591e1fe994da44df77bd8b6ad18ed428e3d1e7f76c83349d61cf8fa06beab4d`  
		Last Modified: Fri, 15 May 2020 15:11:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e231d94c7c66658f89cc128cad35ec1e8e08f2bba42fd7ca4c2d1933d66910ac`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 13.8 MB (13820369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16787fbb561735285d261bea91186df225573e4b193a7592d4ec49acc32d084`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf849c308b829343ad910dacfe26fea7cf2dfa9dbdc0b3f3a08e1c98222a0162`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d8b80f0c7f4669d6b6e1ed2ecff96de24ee0f969520b367f94df418d5156e0`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca082ed920d4a38e00a209eb7e17c1a8ae106cfe67ecf14accca6b19cb4f447`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea1efaf50e775702242a3eff9784b093e3600ed495d0d6a17a3a58801ff95a1`  
		Last Modified: Fri, 15 May 2020 16:13:49 GMT  
		Size: 64.4 MB (64438938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c31e8e8dd500a452bf4fb65bef4b53cb90b55104201023790cd8eb3b11fd1c9`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 2.8 MB (2780306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192dddd32079e34822616719acd1fefbc9e131f8768410a96134e6990992c6ab`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cedc0546fa17b6cc3a6567871c6258482079f0650a8a365e9c6772f419260c`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003e0cd48706b86851b9ac0f0596091925f18ec14074f01e8d3af460185888f8`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f65bf195377180a6b771652637ee9aa80466f99940086e63ac1e653e9542c8`  
		Last Modified: Fri, 15 May 2020 16:13:57 GMT  
		Size: 38.4 MB (38402810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33.3` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:2270a1d8b14b964ee92adebd289d3dc4a107c8c39e44341bf78053f31d269ceb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229079502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5132c469c486d6a880123ccc7a40cb0ae6cf08ecdc48b3e8254849feb9d9782`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:55:21 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 May 2020 23:55:22 GMT
ENV PHP_VERSION=7.2.31
# Thu, 14 May 2020 23:55:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Thu, 14 May 2020 23:55:25 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Thu, 14 May 2020 23:55:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:55:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:59:14 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:59:19 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:59:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:59:20 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:59:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:22 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:59:23 GMT
EXPOSE 80
# Thu, 14 May 2020 23:59:23 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:50:28 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:52:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:52:25 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 01:52:30 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:52:34 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:52:35 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 01:52:36 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 01:52:36 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 01:52:37 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 01:52:57 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6825e5831098a7455da6208d36a8631cf5e2823f499953e959a93d2825d216`  
		Last Modified: Fri, 15 May 2020 00:36:52 GMT  
		Size: 12.6 MB (12646387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c90c04c008327b286591e8e09268bce6fb4e7f4f23f3ecd5e756a8b4e5542`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a57b44810b99bff28e6eae7a26a7e63ee4096f279fbe1bfcf664e6273e41714`  
		Last Modified: Fri, 15 May 2020 00:36:53 GMT  
		Size: 12.9 MB (12893543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7a380e949112ca73a08930f495f01082945469b745a50ff5117e6694418b9`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019bfed0e017e52b99ae6700fd766ea74dcd69819f030e640cc2038a720a060e`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec0f544a95469ff33ebce02ed759bdab577bee1ecc6b52e27535b50190afe9d`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059248e2c7e804da9d7b61c6e9d1ca5845709a53347be8b1cd7323c6a38fcc26`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9be3987479af508dffc0cc23bcbacd781b00f13a165a4c554683d6ffde9d4b`  
		Last Modified: Fri, 15 May 2020 01:55:01 GMT  
		Size: 60.8 MB (60766733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57931c4fa281330d8a2a1e6f7ec30e9d57ca8dd99fda7147cdc0822b0be9d29e`  
		Last Modified: Fri, 15 May 2020 01:54:41 GMT  
		Size: 2.7 MB (2699845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9d9d0c3e509622625df75c6956819df8d94dc4efe60bc12221399a4aaa2a8f`  
		Last Modified: Fri, 15 May 2020 01:54:39 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420af56ef82b61aaf3bfe800975a82585a2d4f95a3139c580182df458585d30c`  
		Last Modified: Fri, 15 May 2020 01:54:39 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b10a569dd7c667c16369563975aeab457b7660090b955c29323ccddb104e6f`  
		Last Modified: Fri, 15 May 2020 01:54:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ef5c668ab603bacf087dd6f5ed5658d660840ce2d851d754dff659a363a557`  
		Last Modified: Fri, 15 May 2020 01:55:02 GMT  
		Size: 38.4 MB (38403453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33.3` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:e8a9a86c49a8ad2e6aadec2935928841a3cef59325877b8e522dd382486f181c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222612271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cd306da7ed80ba57048f02a0b87e09dd48a3181fd63cb1dc81d59486d7a3bf`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:35:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 05:35:19 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 05:35:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 05:35:21 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 05:35:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:35:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:38:37 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:38:40 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:38:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:38:42 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:38:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:43 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:38:43 GMT
EXPOSE 80
# Fri, 15 May 2020 05:38:44 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:37:32 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:04 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 07:39:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:39:08 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:39:09 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 07:39:10 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 07:39:10 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 07:39:11 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 07:39:29 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398113638833857603dca55979da57419d2a5572563cafe1334991af81967142`  
		Last Modified: Fri, 15 May 2020 06:10:24 GMT  
		Size: 12.6 MB (12646418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7959af5842bab4cdea3f1bb587ccf5276a5a9ec306f7549e37c48681732acc`  
		Last Modified: Fri, 15 May 2020 06:10:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ff876ade20645d6ddc3d2b59a603be87a04f0b62827c4665c3f132b44bb823`  
		Last Modified: Fri, 15 May 2020 06:10:25 GMT  
		Size: 12.2 MB (12163941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89eb8d735c9a88db8e9415f7968d824dea1e8ce48775e1f518eac6711f83aa5`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6835a065ff97b202cd23f0f4b753c4d136a169058eacad5989eff11767d592a`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385d20ac491870d83092377014337cc2858d8a8ad5fa34cc5ceb8127c81268d0`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8d5374463d9560454a440a6420fb6b8dfdac2ffe2094ce4390ada18219a7d`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36abbaec8998eb3a82a64613df5bc8258ec9a97630ef2e66abf147adbe44f836`  
		Last Modified: Fri, 15 May 2020 07:41:32 GMT  
		Size: 57.1 MB (57061094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44693c5b4c0ba701dc090f4d812ec58b9769563cd6a75d28d816fe64d1597d1c`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 2.6 MB (2641042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a3c86c58739652e9de2c8ecbf1e6e35f2c35ed2e6bf156d9d7a62f9cdbf5e5`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8f091a3b5fca4a79e6ffdcbaa8f9e3446d93e47fbaaeac6f7be06496aac304`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db86b61467cc5ae06108add0b6e9faa34057e54e5b75174719030e638d7515f0`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d27738bd4597b81957110b74009136505b651c924174ee601609ecd31a702a5`  
		Last Modified: Fri, 15 May 2020 07:41:34 GMT  
		Size: 38.4 MB (38403499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33.3` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:509a4979bbebf3c5ae72c6ef4728e37694b3f86062c8ad3716e7a9304cc9af72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244335715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3746c3e8043df9aa0e0343feebeddeb7408372b75d6918e69703cf63d169d1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:43:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 15:43:10 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 15:43:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 15:43:12 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 15:43:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:43:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:46:26 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:46:30 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:46:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:46:32 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:46:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:34 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:46:35 GMT
EXPOSE 80
# Fri, 15 May 2020 15:46:36 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:50:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:52:22 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 19:52:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:52:31 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:52:33 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 19:52:34 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 19:52:35 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 19:52:37 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 19:52:53 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87c94fdf28f180d95beba9bf62a84566232ed0ccc85839454cfe7f70498d39`  
		Last Modified: Fri, 15 May 2020 16:20:17 GMT  
		Size: 12.6 MB (12647169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd1d4d985393bba996ffbfdeeb1fc32bcb60b185e25e89516dc194d45c9bfee`  
		Last Modified: Fri, 15 May 2020 16:20:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfd1ad71cc2afd1e01539eec4fa66cb9041b028439a810dc8ef3462d6bfd9e3`  
		Last Modified: Fri, 15 May 2020 16:20:09 GMT  
		Size: 13.5 MB (13517080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1a76aeff57626d8acad75f39da3a39cc866b022ed90a6c743ba8e03ebf5bf`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91781f686504a79cb5c3a9ac44c847e82581db2bac375061f90aa7f401a1d38a`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a4c663a05696bf7ccb08382bef8932d7007cc3efae03cd914f100d1d33a074`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a5c61103dcbd74aed611a358358a9362c4e6da5b98ee8319bbb5b12552c697`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea3f778184af99b72385b780d7c9b4fbb5c9a001a764eada8da384a5bfbb5df`  
		Last Modified: Fri, 15 May 2020 19:54:38 GMT  
		Size: 62.2 MB (62238977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1daf0fab3fde127e7446d705cb687ab4511d7dc90edd8be244ccd98520a784f`  
		Last Modified: Fri, 15 May 2020 19:54:22 GMT  
		Size: 2.8 MB (2750463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c60cb45c44a2faf1f864c69adc336270f443061019e4b3b267389f138020ff`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5455d0d0523c81d6f2c76e08cdb1e8e9f6830e37a40368eed77b3428100685f`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0720228b8c502db5f6f28ea9f85591e21d230bf46730e26e35779d494049c9a`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9852953c9e00820f8805e237d72cafb452a1504c545de30aa187853ea39becc3`  
		Last Modified: Fri, 15 May 2020 19:54:38 GMT  
		Size: 38.4 MB (38403380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33.3` - linux; 386

```console
$ docker pull mediawiki@sha256:f8a9293db17f62717827b38c8d48516b8d5c9fd335467a044b41d40e8b673a1c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262427724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e1889e89992fab31e7c0ff4c5108e3e91869d568faf645b59a8726f78c8267`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:29:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 13:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:30:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:35:35 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:35:37 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:35:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:35:37 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:35:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:38 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:35:38 GMT
EXPOSE 80
# Fri, 15 May 2020 13:35:38 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:41:07 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:42:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:42:40 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 15:42:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:42:42 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 15:42:55 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14739e799f47da9c256b708f19578335422750fa82325e096a0fdbd0063dcd8`  
		Last Modified: Fri, 15 May 2020 14:35:18 GMT  
		Size: 12.6 MB (12647664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6602cc810aeb39612ffd93aaf08e6a834bd6a23306b89e007274aa317a9388e7`  
		Last Modified: Fri, 15 May 2020 14:35:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590038160b7b9aa93fbc6ca56843fce86d0f211c74e6f1ace6517f9743938740`  
		Last Modified: Fri, 15 May 2020 14:35:26 GMT  
		Size: 14.1 MB (14142560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f027994bbcc3b11ce489c8b38b2e60498e299fa93b3e7be031676c5cb44e5f37`  
		Last Modified: Fri, 15 May 2020 14:35:14 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aec20265c263a1cad53ad047b72af420de2ec322def253cc491fae7b2d9e6c4`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36479c1104bd5c974f4cf08ae38eb1c21dd1bc34c302c6134a0a5741b51d4efc`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5822ef93d09deb9b8d52cfb9e2ccda9b23b28b42c4c22de223caf7866f0b6081`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1ae57a5c23c1e2e03c3ff891870e6c4bcc5c08d9f12dc4f8d9632fe23a2cbd`  
		Last Modified: Fri, 15 May 2020 15:44:16 GMT  
		Size: 66.4 MB (66394484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a6b6b20b38b12032d751706bf19192545484b51348ea74aaff21a34cecd016`  
		Last Modified: Fri, 15 May 2020 15:43:56 GMT  
		Size: 2.8 MB (2767085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310cc8fe6502e5085d087942e895e66941521dc9e24d4e98b674e45005113fae`  
		Last Modified: Fri, 15 May 2020 15:43:55 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a854515df625c06ba3321bce8ff4c910fac6c639d736cf7cdd66e1a88adab36`  
		Last Modified: Fri, 15 May 2020 15:43:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac1ba4a1ebfce49416ed9341a80f27861585759fcda5895932f9fe3dccc54e7`  
		Last Modified: Fri, 15 May 2020 15:43:55 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e40562f13215b7bbce03df57f3d700cb4618dcf01361e2a5f170055101cb5a0`  
		Last Modified: Fri, 15 May 2020 15:44:13 GMT  
		Size: 38.4 MB (38403029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.33.3` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:b37cdbf4c4a9f1d71077a9045d6338164b96677e00d2d6a1846c7616723eaba3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272630469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fdb9d5a9d4eb3d5fdb5bc0f328473ae021ac26abe6bb132051380bdfeee1fad`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 10:39:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Mon, 18 May 2020 10:39:45 GMT
ENV PHP_VERSION=7.2.31
# Mon, 18 May 2020 10:39:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Mon, 18 May 2020 10:39:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Mon, 18 May 2020 10:42:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 10:42:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 10:47:07 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:17 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 10:47:26 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 10:47:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 10:47:34 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 10:47:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:39 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 10:47:41 GMT
EXPOSE 80
# Mon, 18 May 2020 10:47:43 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:51:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:53:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:53:58 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Mon, 18 May 2020 19:54:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:54:20 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:54:24 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Mon, 18 May 2020 19:54:26 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Mon, 18 May 2020 19:54:33 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Mon, 18 May 2020 19:54:42 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Mon, 18 May 2020 19:55:27 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422d598ad54ce6e95730222751503d9b698243cf90a702ad65e2d4631964790b`  
		Last Modified: Mon, 18 May 2020 12:30:00 GMT  
		Size: 12.6 MB (12648662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1981bd0a5f519849b6b58bcf91970f04a47d652e69fe60ac7ab816477283bb`  
		Last Modified: Mon, 18 May 2020 12:29:50 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a723077ecd7e1721f12f36dabd59b626018e3ed70e28d2933f8033c0885179`  
		Last Modified: Mon, 18 May 2020 12:30:08 GMT  
		Size: 14.9 MB (14857939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931596f7dd07359c094e8c5ce6911e9b4f4dd67bb1a11dec735da42f2507236d`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 2.2 KB (2235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cc1daefd84c15ae993c001ad437714bec6b0c7193b7974dd4bbc496d4d3741`  
		Last Modified: Mon, 18 May 2020 12:29:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666d43f8152a6bbf980f795024b39f5011f8a9f8c55f5d4053c973e9c4a1b43`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b330e8c37cbe3045afe862d0defb2365a798a12fceb4484dc2d0683819efa295`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922138725c394061a32405f8fb772954e20eb97e25a5d36c3f6655fc435f6b8`  
		Last Modified: Mon, 18 May 2020 20:02:56 GMT  
		Size: 71.3 MB (71260606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5203e563f1cf9a02c440e94ed4f6afb43648404a70e0916a8db25357f6809f1b`  
		Last Modified: Mon, 18 May 2020 20:01:30 GMT  
		Size: 2.9 MB (2855225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efd3e6ea5dbeec916c6410d03d6f17b4eac74582b7b7ca78ea4eae5b24430e`  
		Last Modified: Mon, 18 May 2020 20:01:25 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7ec02c6577c567385cc72505ac006b3f6c5c2abd54ac5c95a3df382eecf888`  
		Last Modified: Mon, 18 May 2020 20:01:26 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dde02b1527ca67ce7a4d212825417c27bb340054f4c54951bca032fbc767fd9`  
		Last Modified: Mon, 18 May 2020 20:01:26 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2de52b8e356a6abd3d1871df0c97dfdce7d4f199862bc7286b03d5c54eb5bd`  
		Last Modified: Mon, 18 May 2020 20:03:13 GMT  
		Size: 38.4 MB (38403277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:1.34`

```console
$ docker pull mediawiki@sha256:bb832ca583c8a9f8dec7c81f3e6f16c7f475b6b893cef161640d53272eaacc7a
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
$ docker pull mediawiki@sha256:29b19fb44ba857f5a784c06d16db4dc7b7e97728f7722986881a545712a570ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.2 MB (257167590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec57d9a3fb725cc77dec57b49e2a0e48308d0373f7f9d7d7a2f195cfdea5fb91`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:21:15 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 13:21:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:21:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:27:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:11 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:27:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:27:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:27:13 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:27:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:14 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:27:15 GMT
EXPOSE 80
# Fri, 15 May 2020 13:27:15 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:08:06 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:09:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:09:39 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 16:09:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:09:40 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 16:09:50 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79fb2b388016d9ef524926aa6e5510ffe2d6643a57cd4e09b991ca90ee2072e`  
		Last Modified: Fri, 15 May 2020 15:09:00 GMT  
		Size: 12.5 MB (12454915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa6f0dd42392167b786a269124c84e7cb00bc7dfcde4ea31a4d63ed938eae5`  
		Last Modified: Fri, 15 May 2020 15:08:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9a337c36d9faf17171bac8095de0116c196c8d43d3c8ffd191a6cd3c76d8e`  
		Last Modified: Fri, 15 May 2020 15:09:17 GMT  
		Size: 14.1 MB (14059019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ec85e069109a12ff3539fd6a0da18305c4de7e87a517f19fd22f69d52c4d05`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f88b4f6085316d9f15f1eb8f44f029df3b9ef1c212ce061b6fb27c69596cd`  
		Last Modified: Fri, 15 May 2020 15:08:57 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845e768a44c508b027ed195329349d126b34299f7984158fdf20556acc37e788`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232824f4bf64490716a966bedba7eac6feea4d604f178d602fc97d4c4c87204a`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d2a14eceb1759254f8986a3f37d6c3fc2115c1ed0fc6fecae0094b56cb8735`  
		Last Modified: Fri, 15 May 2020 16:13:26 GMT  
		Size: 64.4 MB (64439822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236d7407028fa4e508d439aa0e8ae86a566b895726fe95d72360232602a69105`  
		Last Modified: Fri, 15 May 2020 16:13:13 GMT  
		Size: 2.8 MB (2848763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8633a5b9d982bead149206f6edf6ba53bfac4d103fa2d781dc47582680041f65`  
		Last Modified: Fri, 15 May 2020 16:13:10 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4820551e47bb3ee07365f44ac5b0bc1d5c1f20575a6de30f402c91d7115d7f6c`  
		Last Modified: Fri, 15 May 2020 16:13:09 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a8e3703db6228225b71d7787cb821efad10f58a429d5b6c61857b99535d68f`  
		Last Modified: Fri, 15 May 2020 16:13:10 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4d3ec4c337c08e2f04d313efcb0bf68751d9d07db4cc27c18494a79cc207c`  
		Last Modified: Fri, 15 May 2020 16:13:24 GMT  
		Size: 40.9 MB (40931742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:6ef90891668c07f83007fad2d70e1f6cd6c43bfcb17ad7cc98bbd6c4734bf063
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231663676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80523e7fc3b2f6883baafa07eaabfde0098fb7f6e209b23db2320aba7d1d32c9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:16:47 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 14 May 2020 23:16:48 GMT
ENV PHP_VERSION=7.3.18
# Thu, 14 May 2020 23:16:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Thu, 14 May 2020 23:16:50 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Thu, 14 May 2020 23:17:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:17:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:20:24 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:20:29 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:20:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:20:31 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:20:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:33 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:20:34 GMT
EXPOSE 80
# Thu, 14 May 2020 23:20:35 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:46:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:48:18 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 01:48:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:48:23 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:48:24 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 01:48:25 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 01:48:27 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 01:48:28 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 01:48:47 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651d4b2e219c22e4556ae6b91b43c8fa3015b952189897ed5f4050faff7adc57`  
		Last Modified: Fri, 15 May 2020 00:34:25 GMT  
		Size: 12.5 MB (12453066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77956b846553f8a18b4aad33de1e52e4cd7a6d43477e54561c8d6656f36ba194`  
		Last Modified: Fri, 15 May 2020 00:34:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9465c0242e4217e7a1c41b0782d633a3ce75e5013e456e288a972cce1f0ac14`  
		Last Modified: Fri, 15 May 2020 00:34:23 GMT  
		Size: 13.1 MB (13073912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea20311112e0d260a80646a73d2d4caa8f67976bc5560d9f2f08d9916d48278`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38d64713f6a75a47fafa5e05c780455f367744a0dc6a0afbd47dadc7302ff53`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef83e0d9c5f54cf179d1c2408b0003012b1b4158c15b1cc30531d9753ae7abe1`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c868686b2b57194f4b983dc554dd48f424894a9f6fc09d6247c5f4440d0e68bb`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a5cf53aa89098463346fff882e09c58d7fd9141761ebed3effb61812dd6eac`  
		Last Modified: Fri, 15 May 2020 01:54:31 GMT  
		Size: 60.8 MB (60766605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae80ee1b272d3a549d3dd81531120d8527cd4dbde708005ffc001cf5de2ae97e`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 2.8 MB (2767806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807c15fe77b8c2b2ec3bb36d38407d30a94142edfafce9d40832a80d7af9a46`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aa15a93e8e5b94b1efc9881a1c56d7c8fb3a1b5c40c2897fc86cfafa2b483`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4c546f84eb62fb9c3a674ac306012ac81735450e45f5d49c6a4e361925f96d`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea2a9eb4e1831052ec170cf68df7ec7183158c2fe0aa441d9e15878b56f03fb`  
		Last Modified: Fri, 15 May 2020 01:54:30 GMT  
		Size: 40.9 MB (40932734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:cb6ef0227eacbaf8adebfaf0476cad0286cc023280381ce2ca0fb5ffb819ed24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225218401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f7db6f03bb23cbbe7debb0714273ece2d6b5881708726101cdb566b0834770`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:01:31 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 05:01:32 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 05:01:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 05:01:34 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 05:01:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:01:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:04:44 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:47 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:04:49 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:04:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:04:51 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:04:51 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:52 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:04:53 GMT
EXPOSE 80
# Fri, 15 May 2020 05:04:54 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:34:13 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:35:51 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 07:35:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:35:55 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:35:56 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 07:35:57 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 07:35:57 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 07:35:58 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 07:36:20 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2938e621459f55a8bead228570f7ad0f7f06671d3261b2d6d78eca4caaefc20e`  
		Last Modified: Fri, 15 May 2020 06:08:00 GMT  
		Size: 12.5 MB (12453083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec53a887462bb7b82d74f19073590522ce9ba29e9ea928e31d218e6261016e0`  
		Last Modified: Fri, 15 May 2020 06:07:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0f40794844f49b5960f331bd0929aa1e88233edeabd5a44e9aca1e4e8a724d`  
		Last Modified: Fri, 15 May 2020 06:07:59 GMT  
		Size: 12.4 MB (12370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac5f0d41f04b86d527452536d2d9bc4009483bc2338c77d984c4ea52c0c710d`  
		Last Modified: Fri, 15 May 2020 06:07:55 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f668c907a8577f1ef10583437ae78b4bd2113faf23421990f408299a814de30`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b645fbaa2410002cae358e403d3a1b43df9830df618afa35731f27a3850000`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fd081f06ffde760d6f3b50d5225b212466a3b52e47cb3876798a4ef8fd1f75`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8081be2e26e7116795496458ee38a8cded038b68aaf1f6800099fe5c8be51b9`  
		Last Modified: Fri, 15 May 2020 07:40:51 GMT  
		Size: 57.1 MB (57061226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1094fa30f94d21e1ebc451bb84f1cf4206d8d30be046eaa6dfbd7635a5e15044`  
		Last Modified: Fri, 15 May 2020 07:40:33 GMT  
		Size: 2.7 MB (2704244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e697dcb512362cb5881d15c4c66a197c366bbb47b359c87f2841b333100da952`  
		Last Modified: Fri, 15 May 2020 07:40:32 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238c0ef2f57091402a22b91e128a8585792c132816512ffb0c5e515324a56bc5`  
		Last Modified: Fri, 15 May 2020 07:40:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072cc991f71c06383542e9830cc1cb4671b648d50b22afb1b30d1a2007d41fa`  
		Last Modified: Fri, 15 May 2020 07:40:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a15059b37524232bf4608f46cf2e3c6d148da21d5a48b6c24ca4aed522e8`  
		Last Modified: Fri, 15 May 2020 07:40:58 GMT  
		Size: 40.9 MB (40932759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:b1ad8500fb35495bf117bc219bed8f1be657b08385c56f9b8e08ac3c34feac95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.0 MB (246967619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f968f66621280d113ebe8ac024f2438ec655038b74a5fdcb7bdcdcb0fbda45`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:07:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 15:07:09 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 15:07:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 15:07:10 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 15:07:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:07:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:10:38 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:41 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:10:42 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:10:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:10:44 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:10:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:46 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:10:46 GMT
EXPOSE 80
# Fri, 15 May 2020 15:10:47 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:46:49 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:48:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:48:15 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 19:48:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:48:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:48:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 19:48:19 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 19:48:20 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 19:48:21 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 19:48:36 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae3de17dd48c732d21fd24f161790248745a1f9f5343ca11b2b43c46e105ea5`  
		Last Modified: Fri, 15 May 2020 16:17:15 GMT  
		Size: 12.5 MB (12453774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb6370bcc1b22f91bc8e213c5b1a4b772d0344be0e7bb9221e63b67db1a142b`  
		Last Modified: Fri, 15 May 2020 16:17:12 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9312f5ef6faa9b465032a4a48145dbd87fe48546ab4b8888738098c00e9f1ad3`  
		Last Modified: Fri, 15 May 2020 16:17:15 GMT  
		Size: 13.7 MB (13744535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c631ec2f0346fc26c53da3692591b7b0debae99b1a15c5534b41b5ba3b239`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b694d004d03fc5a193f48261b7427b006bf62d5e961a72e73f41ee22d13486d`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6c5ca8de4c593238fbedb6cd4958d9de263b56c9c74734d0155ff1096acaf5`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0641e65be1657f4646febd47c17faf35740796ac356e2e26a487b5387ea8a937`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d46d3d03a9f3c6f1f266236a9de585cfff43f73b8d8a1e8d35dd31f3d7d681`  
		Last Modified: Fri, 15 May 2020 19:54:12 GMT  
		Size: 62.2 MB (62238680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a789a163be1e82fb5c0bea8cbebc15041095c08e469b493e190d1e08549d9f3`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 2.8 MB (2819336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98349c303c7d0b2146568c695df1c147d413be75c4f768c0e85a4fdfe1222e`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d503ef15664e43f308e3bd8a34106f553eb9eba97021263c5ad3cd0372732e3b`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a819fc78ba92cfdb40deb661f60ec2a14ccc1cb8100de733b0fc5e4f6d0c5dd`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf8389f93f7e9c79bcb56ef17776a68d219e0c43085b8de81217e59f8cfe24`  
		Last Modified: Fri, 15 May 2020 19:54:12 GMT  
		Size: 40.9 MB (40932669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34` - linux; 386

```console
$ docker pull mediawiki@sha256:332189a321378b5bfa8dec506debb9858bb1ce25fece88eef6e8d4b2dfc93045
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.1 MB (265080182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf89f7d308e111eba6cd152f622205cd4efa33523feb1af181b1c97fd1e5f5c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 12:27:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 12:27:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 12:27:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 12:31:13 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:14 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 12:31:15 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 12:31:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 12:31:15 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 12:31:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:16 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 12:31:16 GMT
EXPOSE 80
# Fri, 15 May 2020 12:31:16 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:38:31 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:39:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:40:00 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 15:40:01 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:40:02 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 15:40:03 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 15:40:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1f71bc06b5ba65a360df23e6baed84cf6a160b954839ade5fb135a184dd24f`  
		Last Modified: Fri, 15 May 2020 14:33:13 GMT  
		Size: 12.5 MB (12454242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ba2fc11a09f1683bd8774c9257aebf492a8a5012970c1f9a1bd0ca35edc3b0`  
		Last Modified: Fri, 15 May 2020 14:33:09 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74a16114860a4d9f5b31e4c56097ff316e09ee0a1c2e90786f3897bd9f8fdd8`  
		Last Modified: Fri, 15 May 2020 14:33:13 GMT  
		Size: 14.4 MB (14375467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247829d9036e677667bd1c3161c7315e639cc0d45116994d134b130d591ec272`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f71c9bd38dca215fe8eaa7397a213a4be8ab9875edbf590ffeacb3e2c4cfa27`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c911d28b575600b8e73c4aa3e85eaaa209727dd18042dc8ddbd2b4fca3b33dc`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82ab66a540f597ce5ca06a395af6ec5fdcc863f663dc058db62daf9c78f090`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109a070655fcc0c1debc1ee41d7ad694a65ee44f682c056b1c54980ffb66973`  
		Last Modified: Fri, 15 May 2020 15:43:50 GMT  
		Size: 66.4 MB (66394508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27b117c4639d08d7aeb286c29b2848c3b983598e0ae07395ab4c80c2c785ed4`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 2.9 MB (2851267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3829f79f51e528e8c68c793caad7bea03e0df15d73e9db6ca0ba3ccf1e9a0f8e`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c514ae942b80c6b7c6c079584aba65bac31d2b773e7507b7d9c829f226b86e91`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d2cb07003bcf2a9df5a93a6034719260d5961e7393349f53e3cf66b21aa523`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b394e7970eb830e1c09319e5841d27d587ca68c518780d6e6dc1ccdb27fd0fd`  
		Last Modified: Fri, 15 May 2020 15:43:48 GMT  
		Size: 40.9 MB (40931786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:aa2aed9f98726d2510e1ebeb5d5c0e130d64989af29b27815f57a29d6321b5fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.3 MB (275283823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9774b50c3e0a56b3bff561f2cf04379af84da0cf2f6a67fcfd53d924da5f0222`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 09:03:54 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Mon, 18 May 2020 09:03:57 GMT
ENV PHP_VERSION=7.3.18
# Mon, 18 May 2020 09:04:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Mon, 18 May 2020 09:04:02 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Mon, 18 May 2020 09:04:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 09:04:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 09:09:08 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:18 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 09:09:24 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 09:09:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 09:09:32 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 09:09:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:41 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 09:09:45 GMT
EXPOSE 80
# Mon, 18 May 2020 09:09:48 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:35:00 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:36:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:37:05 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Mon, 18 May 2020 19:37:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:37:35 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:37:40 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Mon, 18 May 2020 19:37:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Mon, 18 May 2020 19:37:51 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Mon, 18 May 2020 19:37:57 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Mon, 18 May 2020 19:38:38 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5778da4b9e5d7a88f35ba1be2447f4f549ba69a64e3d51f25a3d12ffcd3cb2`  
		Last Modified: Mon, 18 May 2020 12:18:41 GMT  
		Size: 12.5 MB (12455153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71128df22a3960c05cabb8404ffb23bc6a97a69eceecf88249d546ec4b569`  
		Last Modified: Mon, 18 May 2020 12:18:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe189a8a7aa4a630396336b029b1c309e64143334b9269b1fde2ea84d02a64a7`  
		Last Modified: Mon, 18 May 2020 12:18:44 GMT  
		Size: 15.1 MB (15099913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f65c89f9f877a51558fb3fce1bb2c07546baec1d107e4bba266b0f0ce71a566`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 2.2 KB (2234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504d05192abd7dd43e3bf43ec49a93d38dd7cf9766ac7b79de11cfea30ee9d96`  
		Last Modified: Mon, 18 May 2020 12:18:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104c16784d2476249f104fed21df2bb71e7381dc70e23ff42ad529bf5194b39b`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93db3a5ecb93bdf1621a60e23c4fccf40972b0a0a9cf3289348c920fe37ae677`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7c05be6c020e5a185c9e6238c470df50b8aecf5b693efef9f93894f7c51d72`  
		Last Modified: Mon, 18 May 2020 20:01:06 GMT  
		Size: 71.3 MB (71259919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d066ae6d7c04158054703b1090b60c538d06c67c5e507f6251edd00f34b40e4`  
		Last Modified: Mon, 18 May 2020 19:58:43 GMT  
		Size: 2.9 MB (2931556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ee04cfb1211afda04063f7fb27a91b6a9464b71d507a0fe4c60be6efd3b81`  
		Last Modified: Mon, 18 May 2020 19:58:41 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38433421ca9b924ec74833c35c458d15dfd4840146a3d9e8774991067a149ec`  
		Last Modified: Mon, 18 May 2020 19:58:40 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdbfaa842585c91095d27c11c54f50df89493a214aae3e47f4fdcb7ceb46601`  
		Last Modified: Mon, 18 May 2020 19:58:41 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bcb826d084e75a26f21ccce8d07eba5a298e01e61c1c573bfd10737d07a193b`  
		Last Modified: Mon, 18 May 2020 20:00:48 GMT  
		Size: 40.9 MB (40932529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:1.34.1`

```console
$ docker pull mediawiki@sha256:bb832ca583c8a9f8dec7c81f3e6f16c7f475b6b893cef161640d53272eaacc7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:1.34.1` - linux; amd64

```console
$ docker pull mediawiki@sha256:29b19fb44ba857f5a784c06d16db4dc7b7e97728f7722986881a545712a570ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.2 MB (257167590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec57d9a3fb725cc77dec57b49e2a0e48308d0373f7f9d7d7a2f195cfdea5fb91`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:21:15 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 13:21:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:21:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:27:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:11 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:27:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:27:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:27:13 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:27:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:14 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:27:15 GMT
EXPOSE 80
# Fri, 15 May 2020 13:27:15 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:08:06 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:09:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:09:39 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 16:09:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:09:40 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 16:09:50 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79fb2b388016d9ef524926aa6e5510ffe2d6643a57cd4e09b991ca90ee2072e`  
		Last Modified: Fri, 15 May 2020 15:09:00 GMT  
		Size: 12.5 MB (12454915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa6f0dd42392167b786a269124c84e7cb00bc7dfcde4ea31a4d63ed938eae5`  
		Last Modified: Fri, 15 May 2020 15:08:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9a337c36d9faf17171bac8095de0116c196c8d43d3c8ffd191a6cd3c76d8e`  
		Last Modified: Fri, 15 May 2020 15:09:17 GMT  
		Size: 14.1 MB (14059019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ec85e069109a12ff3539fd6a0da18305c4de7e87a517f19fd22f69d52c4d05`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f88b4f6085316d9f15f1eb8f44f029df3b9ef1c212ce061b6fb27c69596cd`  
		Last Modified: Fri, 15 May 2020 15:08:57 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845e768a44c508b027ed195329349d126b34299f7984158fdf20556acc37e788`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232824f4bf64490716a966bedba7eac6feea4d604f178d602fc97d4c4c87204a`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d2a14eceb1759254f8986a3f37d6c3fc2115c1ed0fc6fecae0094b56cb8735`  
		Last Modified: Fri, 15 May 2020 16:13:26 GMT  
		Size: 64.4 MB (64439822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236d7407028fa4e508d439aa0e8ae86a566b895726fe95d72360232602a69105`  
		Last Modified: Fri, 15 May 2020 16:13:13 GMT  
		Size: 2.8 MB (2848763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8633a5b9d982bead149206f6edf6ba53bfac4d103fa2d781dc47582680041f65`  
		Last Modified: Fri, 15 May 2020 16:13:10 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4820551e47bb3ee07365f44ac5b0bc1d5c1f20575a6de30f402c91d7115d7f6c`  
		Last Modified: Fri, 15 May 2020 16:13:09 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a8e3703db6228225b71d7787cb821efad10f58a429d5b6c61857b99535d68f`  
		Last Modified: Fri, 15 May 2020 16:13:10 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4d3ec4c337c08e2f04d313efcb0bf68751d9d07db4cc27c18494a79cc207c`  
		Last Modified: Fri, 15 May 2020 16:13:24 GMT  
		Size: 40.9 MB (40931742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34.1` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:6ef90891668c07f83007fad2d70e1f6cd6c43bfcb17ad7cc98bbd6c4734bf063
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231663676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80523e7fc3b2f6883baafa07eaabfde0098fb7f6e209b23db2320aba7d1d32c9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:16:47 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 14 May 2020 23:16:48 GMT
ENV PHP_VERSION=7.3.18
# Thu, 14 May 2020 23:16:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Thu, 14 May 2020 23:16:50 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Thu, 14 May 2020 23:17:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:17:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:20:24 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:20:29 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:20:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:20:31 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:20:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:33 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:20:34 GMT
EXPOSE 80
# Thu, 14 May 2020 23:20:35 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:46:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:48:18 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 01:48:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:48:23 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:48:24 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 01:48:25 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 01:48:27 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 01:48:28 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 01:48:47 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651d4b2e219c22e4556ae6b91b43c8fa3015b952189897ed5f4050faff7adc57`  
		Last Modified: Fri, 15 May 2020 00:34:25 GMT  
		Size: 12.5 MB (12453066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77956b846553f8a18b4aad33de1e52e4cd7a6d43477e54561c8d6656f36ba194`  
		Last Modified: Fri, 15 May 2020 00:34:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9465c0242e4217e7a1c41b0782d633a3ce75e5013e456e288a972cce1f0ac14`  
		Last Modified: Fri, 15 May 2020 00:34:23 GMT  
		Size: 13.1 MB (13073912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea20311112e0d260a80646a73d2d4caa8f67976bc5560d9f2f08d9916d48278`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38d64713f6a75a47fafa5e05c780455f367744a0dc6a0afbd47dadc7302ff53`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef83e0d9c5f54cf179d1c2408b0003012b1b4158c15b1cc30531d9753ae7abe1`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c868686b2b57194f4b983dc554dd48f424894a9f6fc09d6247c5f4440d0e68bb`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a5cf53aa89098463346fff882e09c58d7fd9141761ebed3effb61812dd6eac`  
		Last Modified: Fri, 15 May 2020 01:54:31 GMT  
		Size: 60.8 MB (60766605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae80ee1b272d3a549d3dd81531120d8527cd4dbde708005ffc001cf5de2ae97e`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 2.8 MB (2767806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807c15fe77b8c2b2ec3bb36d38407d30a94142edfafce9d40832a80d7af9a46`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aa15a93e8e5b94b1efc9881a1c56d7c8fb3a1b5c40c2897fc86cfafa2b483`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4c546f84eb62fb9c3a674ac306012ac81735450e45f5d49c6a4e361925f96d`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea2a9eb4e1831052ec170cf68df7ec7183158c2fe0aa441d9e15878b56f03fb`  
		Last Modified: Fri, 15 May 2020 01:54:30 GMT  
		Size: 40.9 MB (40932734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34.1` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:cb6ef0227eacbaf8adebfaf0476cad0286cc023280381ce2ca0fb5ffb819ed24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225218401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f7db6f03bb23cbbe7debb0714273ece2d6b5881708726101cdb566b0834770`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:01:31 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 05:01:32 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 05:01:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 05:01:34 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 05:01:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:01:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:04:44 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:47 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:04:49 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:04:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:04:51 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:04:51 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:52 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:04:53 GMT
EXPOSE 80
# Fri, 15 May 2020 05:04:54 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:34:13 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:35:51 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 07:35:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:35:55 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:35:56 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 07:35:57 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 07:35:57 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 07:35:58 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 07:36:20 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2938e621459f55a8bead228570f7ad0f7f06671d3261b2d6d78eca4caaefc20e`  
		Last Modified: Fri, 15 May 2020 06:08:00 GMT  
		Size: 12.5 MB (12453083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec53a887462bb7b82d74f19073590522ce9ba29e9ea928e31d218e6261016e0`  
		Last Modified: Fri, 15 May 2020 06:07:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0f40794844f49b5960f331bd0929aa1e88233edeabd5a44e9aca1e4e8a724d`  
		Last Modified: Fri, 15 May 2020 06:07:59 GMT  
		Size: 12.4 MB (12370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac5f0d41f04b86d527452536d2d9bc4009483bc2338c77d984c4ea52c0c710d`  
		Last Modified: Fri, 15 May 2020 06:07:55 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f668c907a8577f1ef10583437ae78b4bd2113faf23421990f408299a814de30`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b645fbaa2410002cae358e403d3a1b43df9830df618afa35731f27a3850000`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fd081f06ffde760d6f3b50d5225b212466a3b52e47cb3876798a4ef8fd1f75`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8081be2e26e7116795496458ee38a8cded038b68aaf1f6800099fe5c8be51b9`  
		Last Modified: Fri, 15 May 2020 07:40:51 GMT  
		Size: 57.1 MB (57061226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1094fa30f94d21e1ebc451bb84f1cf4206d8d30be046eaa6dfbd7635a5e15044`  
		Last Modified: Fri, 15 May 2020 07:40:33 GMT  
		Size: 2.7 MB (2704244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e697dcb512362cb5881d15c4c66a197c366bbb47b359c87f2841b333100da952`  
		Last Modified: Fri, 15 May 2020 07:40:32 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238c0ef2f57091402a22b91e128a8585792c132816512ffb0c5e515324a56bc5`  
		Last Modified: Fri, 15 May 2020 07:40:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072cc991f71c06383542e9830cc1cb4671b648d50b22afb1b30d1a2007d41fa`  
		Last Modified: Fri, 15 May 2020 07:40:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a15059b37524232bf4608f46cf2e3c6d148da21d5a48b6c24ca4aed522e8`  
		Last Modified: Fri, 15 May 2020 07:40:58 GMT  
		Size: 40.9 MB (40932759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34.1` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:b1ad8500fb35495bf117bc219bed8f1be657b08385c56f9b8e08ac3c34feac95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.0 MB (246967619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f968f66621280d113ebe8ac024f2438ec655038b74a5fdcb7bdcdcb0fbda45`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:07:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 15:07:09 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 15:07:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 15:07:10 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 15:07:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:07:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:10:38 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:41 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:10:42 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:10:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:10:44 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:10:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:46 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:10:46 GMT
EXPOSE 80
# Fri, 15 May 2020 15:10:47 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:46:49 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:48:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:48:15 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 19:48:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:48:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:48:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 19:48:19 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 19:48:20 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 19:48:21 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 19:48:36 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae3de17dd48c732d21fd24f161790248745a1f9f5343ca11b2b43c46e105ea5`  
		Last Modified: Fri, 15 May 2020 16:17:15 GMT  
		Size: 12.5 MB (12453774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb6370bcc1b22f91bc8e213c5b1a4b772d0344be0e7bb9221e63b67db1a142b`  
		Last Modified: Fri, 15 May 2020 16:17:12 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9312f5ef6faa9b465032a4a48145dbd87fe48546ab4b8888738098c00e9f1ad3`  
		Last Modified: Fri, 15 May 2020 16:17:15 GMT  
		Size: 13.7 MB (13744535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c631ec2f0346fc26c53da3692591b7b0debae99b1a15c5534b41b5ba3b239`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b694d004d03fc5a193f48261b7427b006bf62d5e961a72e73f41ee22d13486d`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6c5ca8de4c593238fbedb6cd4958d9de263b56c9c74734d0155ff1096acaf5`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0641e65be1657f4646febd47c17faf35740796ac356e2e26a487b5387ea8a937`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d46d3d03a9f3c6f1f266236a9de585cfff43f73b8d8a1e8d35dd31f3d7d681`  
		Last Modified: Fri, 15 May 2020 19:54:12 GMT  
		Size: 62.2 MB (62238680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a789a163be1e82fb5c0bea8cbebc15041095c08e469b493e190d1e08549d9f3`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 2.8 MB (2819336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98349c303c7d0b2146568c695df1c147d413be75c4f768c0e85a4fdfe1222e`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d503ef15664e43f308e3bd8a34106f553eb9eba97021263c5ad3cd0372732e3b`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a819fc78ba92cfdb40deb661f60ec2a14ccc1cb8100de733b0fc5e4f6d0c5dd`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf8389f93f7e9c79bcb56ef17776a68d219e0c43085b8de81217e59f8cfe24`  
		Last Modified: Fri, 15 May 2020 19:54:12 GMT  
		Size: 40.9 MB (40932669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34.1` - linux; 386

```console
$ docker pull mediawiki@sha256:332189a321378b5bfa8dec506debb9858bb1ce25fece88eef6e8d4b2dfc93045
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.1 MB (265080182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf89f7d308e111eba6cd152f622205cd4efa33523feb1af181b1c97fd1e5f5c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 12:27:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 12:27:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 12:27:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 12:31:13 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:14 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 12:31:15 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 12:31:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 12:31:15 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 12:31:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:16 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 12:31:16 GMT
EXPOSE 80
# Fri, 15 May 2020 12:31:16 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:38:31 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:39:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:40:00 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 15:40:01 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:40:02 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 15:40:03 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 15:40:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1f71bc06b5ba65a360df23e6baed84cf6a160b954839ade5fb135a184dd24f`  
		Last Modified: Fri, 15 May 2020 14:33:13 GMT  
		Size: 12.5 MB (12454242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ba2fc11a09f1683bd8774c9257aebf492a8a5012970c1f9a1bd0ca35edc3b0`  
		Last Modified: Fri, 15 May 2020 14:33:09 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74a16114860a4d9f5b31e4c56097ff316e09ee0a1c2e90786f3897bd9f8fdd8`  
		Last Modified: Fri, 15 May 2020 14:33:13 GMT  
		Size: 14.4 MB (14375467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247829d9036e677667bd1c3161c7315e639cc0d45116994d134b130d591ec272`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f71c9bd38dca215fe8eaa7397a213a4be8ab9875edbf590ffeacb3e2c4cfa27`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c911d28b575600b8e73c4aa3e85eaaa209727dd18042dc8ddbd2b4fca3b33dc`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82ab66a540f597ce5ca06a395af6ec5fdcc863f663dc058db62daf9c78f090`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109a070655fcc0c1debc1ee41d7ad694a65ee44f682c056b1c54980ffb66973`  
		Last Modified: Fri, 15 May 2020 15:43:50 GMT  
		Size: 66.4 MB (66394508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27b117c4639d08d7aeb286c29b2848c3b983598e0ae07395ab4c80c2c785ed4`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 2.9 MB (2851267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3829f79f51e528e8c68c793caad7bea03e0df15d73e9db6ca0ba3ccf1e9a0f8e`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c514ae942b80c6b7c6c079584aba65bac31d2b773e7507b7d9c829f226b86e91`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d2cb07003bcf2a9df5a93a6034719260d5961e7393349f53e3cf66b21aa523`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b394e7970eb830e1c09319e5841d27d587ca68c518780d6e6dc1ccdb27fd0fd`  
		Last Modified: Fri, 15 May 2020 15:43:48 GMT  
		Size: 40.9 MB (40931786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:1.34.1` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:aa2aed9f98726d2510e1ebeb5d5c0e130d64989af29b27815f57a29d6321b5fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.3 MB (275283823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9774b50c3e0a56b3bff561f2cf04379af84da0cf2f6a67fcfd53d924da5f0222`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 09:03:54 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Mon, 18 May 2020 09:03:57 GMT
ENV PHP_VERSION=7.3.18
# Mon, 18 May 2020 09:04:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Mon, 18 May 2020 09:04:02 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Mon, 18 May 2020 09:04:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 09:04:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 09:09:08 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:18 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 09:09:24 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 09:09:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 09:09:32 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 09:09:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:41 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 09:09:45 GMT
EXPOSE 80
# Mon, 18 May 2020 09:09:48 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:35:00 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:36:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:37:05 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Mon, 18 May 2020 19:37:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:37:35 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:37:40 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Mon, 18 May 2020 19:37:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Mon, 18 May 2020 19:37:51 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Mon, 18 May 2020 19:37:57 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Mon, 18 May 2020 19:38:38 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5778da4b9e5d7a88f35ba1be2447f4f549ba69a64e3d51f25a3d12ffcd3cb2`  
		Last Modified: Mon, 18 May 2020 12:18:41 GMT  
		Size: 12.5 MB (12455153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71128df22a3960c05cabb8404ffb23bc6a97a69eceecf88249d546ec4b569`  
		Last Modified: Mon, 18 May 2020 12:18:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe189a8a7aa4a630396336b029b1c309e64143334b9269b1fde2ea84d02a64a7`  
		Last Modified: Mon, 18 May 2020 12:18:44 GMT  
		Size: 15.1 MB (15099913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f65c89f9f877a51558fb3fce1bb2c07546baec1d107e4bba266b0f0ce71a566`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 2.2 KB (2234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504d05192abd7dd43e3bf43ec49a93d38dd7cf9766ac7b79de11cfea30ee9d96`  
		Last Modified: Mon, 18 May 2020 12:18:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104c16784d2476249f104fed21df2bb71e7381dc70e23ff42ad529bf5194b39b`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93db3a5ecb93bdf1621a60e23c4fccf40972b0a0a9cf3289348c920fe37ae677`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7c05be6c020e5a185c9e6238c470df50b8aecf5b693efef9f93894f7c51d72`  
		Last Modified: Mon, 18 May 2020 20:01:06 GMT  
		Size: 71.3 MB (71259919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d066ae6d7c04158054703b1090b60c538d06c67c5e507f6251edd00f34b40e4`  
		Last Modified: Mon, 18 May 2020 19:58:43 GMT  
		Size: 2.9 MB (2931556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ee04cfb1211afda04063f7fb27a91b6a9464b71d507a0fe4c60be6efd3b81`  
		Last Modified: Mon, 18 May 2020 19:58:41 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38433421ca9b924ec74833c35c458d15dfd4840146a3d9e8774991067a149ec`  
		Last Modified: Mon, 18 May 2020 19:58:40 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdbfaa842585c91095d27c11c54f50df89493a214aae3e47f4fdcb7ceb46601`  
		Last Modified: Mon, 18 May 2020 19:58:41 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bcb826d084e75a26f21ccce8d07eba5a298e01e61c1c573bfd10737d07a193b`  
		Last Modified: Mon, 18 May 2020 20:00:48 GMT  
		Size: 40.9 MB (40932529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:latest`

```console
$ docker pull mediawiki@sha256:bb832ca583c8a9f8dec7c81f3e6f16c7f475b6b893cef161640d53272eaacc7a
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
$ docker pull mediawiki@sha256:29b19fb44ba857f5a784c06d16db4dc7b7e97728f7722986881a545712a570ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.2 MB (257167590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec57d9a3fb725cc77dec57b49e2a0e48308d0373f7f9d7d7a2f195cfdea5fb91`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:21:15 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 13:21:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:21:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:27:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:11 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:27:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:27:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:27:13 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:27:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:14 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:27:15 GMT
EXPOSE 80
# Fri, 15 May 2020 13:27:15 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:08:06 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:09:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:09:39 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 16:09:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:09:40 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 16:09:50 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79fb2b388016d9ef524926aa6e5510ffe2d6643a57cd4e09b991ca90ee2072e`  
		Last Modified: Fri, 15 May 2020 15:09:00 GMT  
		Size: 12.5 MB (12454915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa6f0dd42392167b786a269124c84e7cb00bc7dfcde4ea31a4d63ed938eae5`  
		Last Modified: Fri, 15 May 2020 15:08:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9a337c36d9faf17171bac8095de0116c196c8d43d3c8ffd191a6cd3c76d8e`  
		Last Modified: Fri, 15 May 2020 15:09:17 GMT  
		Size: 14.1 MB (14059019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ec85e069109a12ff3539fd6a0da18305c4de7e87a517f19fd22f69d52c4d05`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f88b4f6085316d9f15f1eb8f44f029df3b9ef1c212ce061b6fb27c69596cd`  
		Last Modified: Fri, 15 May 2020 15:08:57 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845e768a44c508b027ed195329349d126b34299f7984158fdf20556acc37e788`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232824f4bf64490716a966bedba7eac6feea4d604f178d602fc97d4c4c87204a`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d2a14eceb1759254f8986a3f37d6c3fc2115c1ed0fc6fecae0094b56cb8735`  
		Last Modified: Fri, 15 May 2020 16:13:26 GMT  
		Size: 64.4 MB (64439822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236d7407028fa4e508d439aa0e8ae86a566b895726fe95d72360232602a69105`  
		Last Modified: Fri, 15 May 2020 16:13:13 GMT  
		Size: 2.8 MB (2848763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8633a5b9d982bead149206f6edf6ba53bfac4d103fa2d781dc47582680041f65`  
		Last Modified: Fri, 15 May 2020 16:13:10 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4820551e47bb3ee07365f44ac5b0bc1d5c1f20575a6de30f402c91d7115d7f6c`  
		Last Modified: Fri, 15 May 2020 16:13:09 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a8e3703db6228225b71d7787cb821efad10f58a429d5b6c61857b99535d68f`  
		Last Modified: Fri, 15 May 2020 16:13:10 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4d3ec4c337c08e2f04d313efcb0bf68751d9d07db4cc27c18494a79cc207c`  
		Last Modified: Fri, 15 May 2020 16:13:24 GMT  
		Size: 40.9 MB (40931742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:latest` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:6ef90891668c07f83007fad2d70e1f6cd6c43bfcb17ad7cc98bbd6c4734bf063
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231663676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80523e7fc3b2f6883baafa07eaabfde0098fb7f6e209b23db2320aba7d1d32c9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:16:47 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 14 May 2020 23:16:48 GMT
ENV PHP_VERSION=7.3.18
# Thu, 14 May 2020 23:16:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Thu, 14 May 2020 23:16:50 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Thu, 14 May 2020 23:17:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:17:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:20:24 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:20:29 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:20:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:20:31 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:20:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:33 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:20:34 GMT
EXPOSE 80
# Thu, 14 May 2020 23:20:35 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:46:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:48:18 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 01:48:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:48:23 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:48:24 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 01:48:25 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 01:48:27 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 01:48:28 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 01:48:47 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651d4b2e219c22e4556ae6b91b43c8fa3015b952189897ed5f4050faff7adc57`  
		Last Modified: Fri, 15 May 2020 00:34:25 GMT  
		Size: 12.5 MB (12453066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77956b846553f8a18b4aad33de1e52e4cd7a6d43477e54561c8d6656f36ba194`  
		Last Modified: Fri, 15 May 2020 00:34:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9465c0242e4217e7a1c41b0782d633a3ce75e5013e456e288a972cce1f0ac14`  
		Last Modified: Fri, 15 May 2020 00:34:23 GMT  
		Size: 13.1 MB (13073912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea20311112e0d260a80646a73d2d4caa8f67976bc5560d9f2f08d9916d48278`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38d64713f6a75a47fafa5e05c780455f367744a0dc6a0afbd47dadc7302ff53`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef83e0d9c5f54cf179d1c2408b0003012b1b4158c15b1cc30531d9753ae7abe1`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c868686b2b57194f4b983dc554dd48f424894a9f6fc09d6247c5f4440d0e68bb`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a5cf53aa89098463346fff882e09c58d7fd9141761ebed3effb61812dd6eac`  
		Last Modified: Fri, 15 May 2020 01:54:31 GMT  
		Size: 60.8 MB (60766605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae80ee1b272d3a549d3dd81531120d8527cd4dbde708005ffc001cf5de2ae97e`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 2.8 MB (2767806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807c15fe77b8c2b2ec3bb36d38407d30a94142edfafce9d40832a80d7af9a46`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aa15a93e8e5b94b1efc9881a1c56d7c8fb3a1b5c40c2897fc86cfafa2b483`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4c546f84eb62fb9c3a674ac306012ac81735450e45f5d49c6a4e361925f96d`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea2a9eb4e1831052ec170cf68df7ec7183158c2fe0aa441d9e15878b56f03fb`  
		Last Modified: Fri, 15 May 2020 01:54:30 GMT  
		Size: 40.9 MB (40932734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:latest` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:cb6ef0227eacbaf8adebfaf0476cad0286cc023280381ce2ca0fb5ffb819ed24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225218401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f7db6f03bb23cbbe7debb0714273ece2d6b5881708726101cdb566b0834770`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:01:31 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 05:01:32 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 05:01:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 05:01:34 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 05:01:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:01:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:04:44 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:47 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:04:49 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:04:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:04:51 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:04:51 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:52 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:04:53 GMT
EXPOSE 80
# Fri, 15 May 2020 05:04:54 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:34:13 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:35:51 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 07:35:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:35:55 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:35:56 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 07:35:57 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 07:35:57 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 07:35:58 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 07:36:20 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2938e621459f55a8bead228570f7ad0f7f06671d3261b2d6d78eca4caaefc20e`  
		Last Modified: Fri, 15 May 2020 06:08:00 GMT  
		Size: 12.5 MB (12453083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec53a887462bb7b82d74f19073590522ce9ba29e9ea928e31d218e6261016e0`  
		Last Modified: Fri, 15 May 2020 06:07:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0f40794844f49b5960f331bd0929aa1e88233edeabd5a44e9aca1e4e8a724d`  
		Last Modified: Fri, 15 May 2020 06:07:59 GMT  
		Size: 12.4 MB (12370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac5f0d41f04b86d527452536d2d9bc4009483bc2338c77d984c4ea52c0c710d`  
		Last Modified: Fri, 15 May 2020 06:07:55 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f668c907a8577f1ef10583437ae78b4bd2113faf23421990f408299a814de30`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b645fbaa2410002cae358e403d3a1b43df9830df618afa35731f27a3850000`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fd081f06ffde760d6f3b50d5225b212466a3b52e47cb3876798a4ef8fd1f75`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8081be2e26e7116795496458ee38a8cded038b68aaf1f6800099fe5c8be51b9`  
		Last Modified: Fri, 15 May 2020 07:40:51 GMT  
		Size: 57.1 MB (57061226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1094fa30f94d21e1ebc451bb84f1cf4206d8d30be046eaa6dfbd7635a5e15044`  
		Last Modified: Fri, 15 May 2020 07:40:33 GMT  
		Size: 2.7 MB (2704244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e697dcb512362cb5881d15c4c66a197c366bbb47b359c87f2841b333100da952`  
		Last Modified: Fri, 15 May 2020 07:40:32 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238c0ef2f57091402a22b91e128a8585792c132816512ffb0c5e515324a56bc5`  
		Last Modified: Fri, 15 May 2020 07:40:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072cc991f71c06383542e9830cc1cb4671b648d50b22afb1b30d1a2007d41fa`  
		Last Modified: Fri, 15 May 2020 07:40:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a15059b37524232bf4608f46cf2e3c6d148da21d5a48b6c24ca4aed522e8`  
		Last Modified: Fri, 15 May 2020 07:40:58 GMT  
		Size: 40.9 MB (40932759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:latest` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:b1ad8500fb35495bf117bc219bed8f1be657b08385c56f9b8e08ac3c34feac95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.0 MB (246967619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f968f66621280d113ebe8ac024f2438ec655038b74a5fdcb7bdcdcb0fbda45`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:07:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 15:07:09 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 15:07:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 15:07:10 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 15:07:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:07:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:10:38 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:41 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:10:42 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:10:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:10:44 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:10:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:46 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:10:46 GMT
EXPOSE 80
# Fri, 15 May 2020 15:10:47 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:46:49 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:48:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:48:15 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 19:48:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:48:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:48:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 19:48:19 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 19:48:20 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 19:48:21 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 19:48:36 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae3de17dd48c732d21fd24f161790248745a1f9f5343ca11b2b43c46e105ea5`  
		Last Modified: Fri, 15 May 2020 16:17:15 GMT  
		Size: 12.5 MB (12453774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb6370bcc1b22f91bc8e213c5b1a4b772d0344be0e7bb9221e63b67db1a142b`  
		Last Modified: Fri, 15 May 2020 16:17:12 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9312f5ef6faa9b465032a4a48145dbd87fe48546ab4b8888738098c00e9f1ad3`  
		Last Modified: Fri, 15 May 2020 16:17:15 GMT  
		Size: 13.7 MB (13744535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c631ec2f0346fc26c53da3692591b7b0debae99b1a15c5534b41b5ba3b239`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b694d004d03fc5a193f48261b7427b006bf62d5e961a72e73f41ee22d13486d`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6c5ca8de4c593238fbedb6cd4958d9de263b56c9c74734d0155ff1096acaf5`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0641e65be1657f4646febd47c17faf35740796ac356e2e26a487b5387ea8a937`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d46d3d03a9f3c6f1f266236a9de585cfff43f73b8d8a1e8d35dd31f3d7d681`  
		Last Modified: Fri, 15 May 2020 19:54:12 GMT  
		Size: 62.2 MB (62238680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a789a163be1e82fb5c0bea8cbebc15041095c08e469b493e190d1e08549d9f3`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 2.8 MB (2819336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98349c303c7d0b2146568c695df1c147d413be75c4f768c0e85a4fdfe1222e`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d503ef15664e43f308e3bd8a34106f553eb9eba97021263c5ad3cd0372732e3b`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a819fc78ba92cfdb40deb661f60ec2a14ccc1cb8100de733b0fc5e4f6d0c5dd`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf8389f93f7e9c79bcb56ef17776a68d219e0c43085b8de81217e59f8cfe24`  
		Last Modified: Fri, 15 May 2020 19:54:12 GMT  
		Size: 40.9 MB (40932669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:latest` - linux; 386

```console
$ docker pull mediawiki@sha256:332189a321378b5bfa8dec506debb9858bb1ce25fece88eef6e8d4b2dfc93045
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.1 MB (265080182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf89f7d308e111eba6cd152f622205cd4efa33523feb1af181b1c97fd1e5f5c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 12:27:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 12:27:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 12:27:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 12:31:13 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:14 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 12:31:15 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 12:31:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 12:31:15 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 12:31:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:16 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 12:31:16 GMT
EXPOSE 80
# Fri, 15 May 2020 12:31:16 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:38:31 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:39:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:40:00 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 15:40:01 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:40:02 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 15:40:03 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 15:40:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1f71bc06b5ba65a360df23e6baed84cf6a160b954839ade5fb135a184dd24f`  
		Last Modified: Fri, 15 May 2020 14:33:13 GMT  
		Size: 12.5 MB (12454242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ba2fc11a09f1683bd8774c9257aebf492a8a5012970c1f9a1bd0ca35edc3b0`  
		Last Modified: Fri, 15 May 2020 14:33:09 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74a16114860a4d9f5b31e4c56097ff316e09ee0a1c2e90786f3897bd9f8fdd8`  
		Last Modified: Fri, 15 May 2020 14:33:13 GMT  
		Size: 14.4 MB (14375467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247829d9036e677667bd1c3161c7315e639cc0d45116994d134b130d591ec272`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f71c9bd38dca215fe8eaa7397a213a4be8ab9875edbf590ffeacb3e2c4cfa27`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c911d28b575600b8e73c4aa3e85eaaa209727dd18042dc8ddbd2b4fca3b33dc`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82ab66a540f597ce5ca06a395af6ec5fdcc863f663dc058db62daf9c78f090`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109a070655fcc0c1debc1ee41d7ad694a65ee44f682c056b1c54980ffb66973`  
		Last Modified: Fri, 15 May 2020 15:43:50 GMT  
		Size: 66.4 MB (66394508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27b117c4639d08d7aeb286c29b2848c3b983598e0ae07395ab4c80c2c785ed4`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 2.9 MB (2851267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3829f79f51e528e8c68c793caad7bea03e0df15d73e9db6ca0ba3ccf1e9a0f8e`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c514ae942b80c6b7c6c079584aba65bac31d2b773e7507b7d9c829f226b86e91`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d2cb07003bcf2a9df5a93a6034719260d5961e7393349f53e3cf66b21aa523`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b394e7970eb830e1c09319e5841d27d587ca68c518780d6e6dc1ccdb27fd0fd`  
		Last Modified: Fri, 15 May 2020 15:43:48 GMT  
		Size: 40.9 MB (40931786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:latest` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:aa2aed9f98726d2510e1ebeb5d5c0e130d64989af29b27815f57a29d6321b5fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.3 MB (275283823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9774b50c3e0a56b3bff561f2cf04379af84da0cf2f6a67fcfd53d924da5f0222`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 09:03:54 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Mon, 18 May 2020 09:03:57 GMT
ENV PHP_VERSION=7.3.18
# Mon, 18 May 2020 09:04:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Mon, 18 May 2020 09:04:02 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Mon, 18 May 2020 09:04:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 09:04:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 09:09:08 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:18 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 09:09:24 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 09:09:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 09:09:32 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 09:09:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:41 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 09:09:45 GMT
EXPOSE 80
# Mon, 18 May 2020 09:09:48 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:35:00 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:36:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:37:05 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Mon, 18 May 2020 19:37:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:37:35 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:37:40 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Mon, 18 May 2020 19:37:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Mon, 18 May 2020 19:37:51 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Mon, 18 May 2020 19:37:57 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Mon, 18 May 2020 19:38:38 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5778da4b9e5d7a88f35ba1be2447f4f549ba69a64e3d51f25a3d12ffcd3cb2`  
		Last Modified: Mon, 18 May 2020 12:18:41 GMT  
		Size: 12.5 MB (12455153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71128df22a3960c05cabb8404ffb23bc6a97a69eceecf88249d546ec4b569`  
		Last Modified: Mon, 18 May 2020 12:18:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe189a8a7aa4a630396336b029b1c309e64143334b9269b1fde2ea84d02a64a7`  
		Last Modified: Mon, 18 May 2020 12:18:44 GMT  
		Size: 15.1 MB (15099913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f65c89f9f877a51558fb3fce1bb2c07546baec1d107e4bba266b0f0ce71a566`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 2.2 KB (2234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504d05192abd7dd43e3bf43ec49a93d38dd7cf9766ac7b79de11cfea30ee9d96`  
		Last Modified: Mon, 18 May 2020 12:18:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104c16784d2476249f104fed21df2bb71e7381dc70e23ff42ad529bf5194b39b`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93db3a5ecb93bdf1621a60e23c4fccf40972b0a0a9cf3289348c920fe37ae677`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7c05be6c020e5a185c9e6238c470df50b8aecf5b693efef9f93894f7c51d72`  
		Last Modified: Mon, 18 May 2020 20:01:06 GMT  
		Size: 71.3 MB (71259919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d066ae6d7c04158054703b1090b60c538d06c67c5e507f6251edd00f34b40e4`  
		Last Modified: Mon, 18 May 2020 19:58:43 GMT  
		Size: 2.9 MB (2931556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ee04cfb1211afda04063f7fb27a91b6a9464b71d507a0fe4c60be6efd3b81`  
		Last Modified: Mon, 18 May 2020 19:58:41 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38433421ca9b924ec74833c35c458d15dfd4840146a3d9e8774991067a149ec`  
		Last Modified: Mon, 18 May 2020 19:58:40 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdbfaa842585c91095d27c11c54f50df89493a214aae3e47f4fdcb7ceb46601`  
		Last Modified: Mon, 18 May 2020 19:58:41 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bcb826d084e75a26f21ccce8d07eba5a298e01e61c1c573bfd10737d07a193b`  
		Last Modified: Mon, 18 May 2020 20:00:48 GMT  
		Size: 40.9 MB (40932529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:legacy`

```console
$ docker pull mediawiki@sha256:10054842db0f529ec6eb2bb4aad454048ad9b3ee3b3b851c806f11973502728e
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
$ docker pull mediawiki@sha256:a36de3946e6a63a79f2f227385247be84f2bc2ecec9557ed2071f37ae76b54b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254524143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d0fa04e7669cd74c7411a9c921f1fd10fa10bcaef4754242e0722d0df4eaa51`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 14:23:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 14:23:53 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 14:24:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 14:24:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 14:28:04 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 14:28:06 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 14:28:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 14:28:06 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 14:28:06 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:06 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 14:28:07 GMT
EXPOSE 80
# Fri, 15 May 2020 14:28:07 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:10:39 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:09 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 16:12:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:12:10 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 16:12:11 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 16:12:20 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e342cb20e11a1dd9d7c623fa9432bd079fde2b090476b3134baf0c21d40612a`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 12.6 MB (12648389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c591e1fe994da44df77bd8b6ad18ed428e3d1e7f76c83349d61cf8fa06beab4d`  
		Last Modified: Fri, 15 May 2020 15:11:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e231d94c7c66658f89cc128cad35ec1e8e08f2bba42fd7ca4c2d1933d66910ac`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 13.8 MB (13820369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16787fbb561735285d261bea91186df225573e4b193a7592d4ec49acc32d084`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf849c308b829343ad910dacfe26fea7cf2dfa9dbdc0b3f3a08e1c98222a0162`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d8b80f0c7f4669d6b6e1ed2ecff96de24ee0f969520b367f94df418d5156e0`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca082ed920d4a38e00a209eb7e17c1a8ae106cfe67ecf14accca6b19cb4f447`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea1efaf50e775702242a3eff9784b093e3600ed495d0d6a17a3a58801ff95a1`  
		Last Modified: Fri, 15 May 2020 16:13:49 GMT  
		Size: 64.4 MB (64438938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c31e8e8dd500a452bf4fb65bef4b53cb90b55104201023790cd8eb3b11fd1c9`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 2.8 MB (2780306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192dddd32079e34822616719acd1fefbc9e131f8768410a96134e6990992c6ab`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cedc0546fa17b6cc3a6567871c6258482079f0650a8a365e9c6772f419260c`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003e0cd48706b86851b9ac0f0596091925f18ec14074f01e8d3af460185888f8`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f65bf195377180a6b771652637ee9aa80466f99940086e63ac1e653e9542c8`  
		Last Modified: Fri, 15 May 2020 16:13:57 GMT  
		Size: 38.4 MB (38402810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:2270a1d8b14b964ee92adebd289d3dc4a107c8c39e44341bf78053f31d269ceb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.1 MB (229079502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5132c469c486d6a880123ccc7a40cb0ae6cf08ecdc48b3e8254849feb9d9782`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:55:21 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 May 2020 23:55:22 GMT
ENV PHP_VERSION=7.2.31
# Thu, 14 May 2020 23:55:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Thu, 14 May 2020 23:55:25 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Thu, 14 May 2020 23:55:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:55:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:59:14 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:59:19 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:59:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:59:20 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:59:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:22 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:59:23 GMT
EXPOSE 80
# Thu, 14 May 2020 23:59:23 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:50:28 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:52:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:52:25 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 01:52:30 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:52:34 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:52:35 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 01:52:36 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 01:52:36 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 01:52:37 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 01:52:57 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6825e5831098a7455da6208d36a8631cf5e2823f499953e959a93d2825d216`  
		Last Modified: Fri, 15 May 2020 00:36:52 GMT  
		Size: 12.6 MB (12646387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c90c04c008327b286591e8e09268bce6fb4e7f4f23f3ecd5e756a8b4e5542`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a57b44810b99bff28e6eae7a26a7e63ee4096f279fbe1bfcf664e6273e41714`  
		Last Modified: Fri, 15 May 2020 00:36:53 GMT  
		Size: 12.9 MB (12893543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7a380e949112ca73a08930f495f01082945469b745a50ff5117e6694418b9`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019bfed0e017e52b99ae6700fd766ea74dcd69819f030e640cc2038a720a060e`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec0f544a95469ff33ebce02ed759bdab577bee1ecc6b52e27535b50190afe9d`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059248e2c7e804da9d7b61c6e9d1ca5845709a53347be8b1cd7323c6a38fcc26`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9be3987479af508dffc0cc23bcbacd781b00f13a165a4c554683d6ffde9d4b`  
		Last Modified: Fri, 15 May 2020 01:55:01 GMT  
		Size: 60.8 MB (60766733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57931c4fa281330d8a2a1e6f7ec30e9d57ca8dd99fda7147cdc0822b0be9d29e`  
		Last Modified: Fri, 15 May 2020 01:54:41 GMT  
		Size: 2.7 MB (2699845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9d9d0c3e509622625df75c6956819df8d94dc4efe60bc12221399a4aaa2a8f`  
		Last Modified: Fri, 15 May 2020 01:54:39 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420af56ef82b61aaf3bfe800975a82585a2d4f95a3139c580182df458585d30c`  
		Last Modified: Fri, 15 May 2020 01:54:39 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b10a569dd7c667c16369563975aeab457b7660090b955c29323ccddb104e6f`  
		Last Modified: Fri, 15 May 2020 01:54:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ef5c668ab603bacf087dd6f5ed5658d660840ce2d851d754dff659a363a557`  
		Last Modified: Fri, 15 May 2020 01:55:02 GMT  
		Size: 38.4 MB (38403453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:e8a9a86c49a8ad2e6aadec2935928841a3cef59325877b8e522dd382486f181c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222612271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cd306da7ed80ba57048f02a0b87e09dd48a3181fd63cb1dc81d59486d7a3bf`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:35:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 05:35:19 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 05:35:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 05:35:21 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 05:35:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:35:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:38:37 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:38:40 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:38:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:38:42 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:38:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:43 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:38:43 GMT
EXPOSE 80
# Fri, 15 May 2020 05:38:44 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:37:32 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:04 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 07:39:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:39:08 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:39:09 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 07:39:10 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 07:39:10 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 07:39:11 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 07:39:29 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398113638833857603dca55979da57419d2a5572563cafe1334991af81967142`  
		Last Modified: Fri, 15 May 2020 06:10:24 GMT  
		Size: 12.6 MB (12646418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7959af5842bab4cdea3f1bb587ccf5276a5a9ec306f7549e37c48681732acc`  
		Last Modified: Fri, 15 May 2020 06:10:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ff876ade20645d6ddc3d2b59a603be87a04f0b62827c4665c3f132b44bb823`  
		Last Modified: Fri, 15 May 2020 06:10:25 GMT  
		Size: 12.2 MB (12163941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89eb8d735c9a88db8e9415f7968d824dea1e8ce48775e1f518eac6711f83aa5`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6835a065ff97b202cd23f0f4b753c4d136a169058eacad5989eff11767d592a`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385d20ac491870d83092377014337cc2858d8a8ad5fa34cc5ceb8127c81268d0`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8d5374463d9560454a440a6420fb6b8dfdac2ffe2094ce4390ada18219a7d`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36abbaec8998eb3a82a64613df5bc8258ec9a97630ef2e66abf147adbe44f836`  
		Last Modified: Fri, 15 May 2020 07:41:32 GMT  
		Size: 57.1 MB (57061094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44693c5b4c0ba701dc090f4d812ec58b9769563cd6a75d28d816fe64d1597d1c`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 2.6 MB (2641042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a3c86c58739652e9de2c8ecbf1e6e35f2c35ed2e6bf156d9d7a62f9cdbf5e5`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8f091a3b5fca4a79e6ffdcbaa8f9e3446d93e47fbaaeac6f7be06496aac304`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db86b61467cc5ae06108add0b6e9faa34057e54e5b75174719030e638d7515f0`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d27738bd4597b81957110b74009136505b651c924174ee601609ecd31a702a5`  
		Last Modified: Fri, 15 May 2020 07:41:34 GMT  
		Size: 38.4 MB (38403499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:509a4979bbebf3c5ae72c6ef4728e37694b3f86062c8ad3716e7a9304cc9af72
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244335715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be3746c3e8043df9aa0e0343feebeddeb7408372b75d6918e69703cf63d169d1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:43:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 15:43:10 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 15:43:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 15:43:12 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 15:43:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:43:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:46:26 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:46:30 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:46:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:46:32 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:46:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:34 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:46:35 GMT
EXPOSE 80
# Fri, 15 May 2020 15:46:36 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:50:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:52:22 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 19:52:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:52:31 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:52:33 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 19:52:34 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 19:52:35 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 19:52:37 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 19:52:53 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87c94fdf28f180d95beba9bf62a84566232ed0ccc85839454cfe7f70498d39`  
		Last Modified: Fri, 15 May 2020 16:20:17 GMT  
		Size: 12.6 MB (12647169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd1d4d985393bba996ffbfdeeb1fc32bcb60b185e25e89516dc194d45c9bfee`  
		Last Modified: Fri, 15 May 2020 16:20:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfd1ad71cc2afd1e01539eec4fa66cb9041b028439a810dc8ef3462d6bfd9e3`  
		Last Modified: Fri, 15 May 2020 16:20:09 GMT  
		Size: 13.5 MB (13517080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1a76aeff57626d8acad75f39da3a39cc866b022ed90a6c743ba8e03ebf5bf`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91781f686504a79cb5c3a9ac44c847e82581db2bac375061f90aa7f401a1d38a`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a4c663a05696bf7ccb08382bef8932d7007cc3efae03cd914f100d1d33a074`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a5c61103dcbd74aed611a358358a9362c4e6da5b98ee8319bbb5b12552c697`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea3f778184af99b72385b780d7c9b4fbb5c9a001a764eada8da384a5bfbb5df`  
		Last Modified: Fri, 15 May 2020 19:54:38 GMT  
		Size: 62.2 MB (62238977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1daf0fab3fde127e7446d705cb687ab4511d7dc90edd8be244ccd98520a784f`  
		Last Modified: Fri, 15 May 2020 19:54:22 GMT  
		Size: 2.8 MB (2750463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c60cb45c44a2faf1f864c69adc336270f443061019e4b3b267389f138020ff`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 591.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5455d0d0523c81d6f2c76e08cdb1e8e9f6830e37a40368eed77b3428100685f`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0720228b8c502db5f6f28ea9f85591e21d230bf46730e26e35779d494049c9a`  
		Last Modified: Fri, 15 May 2020 19:54:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9852953c9e00820f8805e237d72cafb452a1504c545de30aa187853ea39becc3`  
		Last Modified: Fri, 15 May 2020 19:54:38 GMT  
		Size: 38.4 MB (38403380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; 386

```console
$ docker pull mediawiki@sha256:f8a9293db17f62717827b38c8d48516b8d5c9fd335467a044b41d40e8b673a1c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.4 MB (262427724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4e1889e89992fab31e7c0ff4c5108e3e91869d568faf645b59a8726f78c8267`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:29:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 13:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:30:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:35:35 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:35:37 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:35:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:35:37 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:35:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:38 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:35:38 GMT
EXPOSE 80
# Fri, 15 May 2020 13:35:38 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:41:07 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:42:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:42:40 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 15:42:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:42:42 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Fri, 15 May 2020 15:42:42 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Fri, 15 May 2020 15:42:55 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14739e799f47da9c256b708f19578335422750fa82325e096a0fdbd0063dcd8`  
		Last Modified: Fri, 15 May 2020 14:35:18 GMT  
		Size: 12.6 MB (12647664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6602cc810aeb39612ffd93aaf08e6a834bd6a23306b89e007274aa317a9388e7`  
		Last Modified: Fri, 15 May 2020 14:35:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590038160b7b9aa93fbc6ca56843fce86d0f211c74e6f1ace6517f9743938740`  
		Last Modified: Fri, 15 May 2020 14:35:26 GMT  
		Size: 14.1 MB (14142560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f027994bbcc3b11ce489c8b38b2e60498e299fa93b3e7be031676c5cb44e5f37`  
		Last Modified: Fri, 15 May 2020 14:35:14 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aec20265c263a1cad53ad047b72af420de2ec322def253cc491fae7b2d9e6c4`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36479c1104bd5c974f4cf08ae38eb1c21dd1bc34c302c6134a0a5741b51d4efc`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5822ef93d09deb9b8d52cfb9e2ccda9b23b28b42c4c22de223caf7866f0b6081`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1ae57a5c23c1e2e03c3ff891870e6c4bcc5c08d9f12dc4f8d9632fe23a2cbd`  
		Last Modified: Fri, 15 May 2020 15:44:16 GMT  
		Size: 66.4 MB (66394484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a6b6b20b38b12032d751706bf19192545484b51348ea74aaff21a34cecd016`  
		Last Modified: Fri, 15 May 2020 15:43:56 GMT  
		Size: 2.8 MB (2767085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310cc8fe6502e5085d087942e895e66941521dc9e24d4e98b674e45005113fae`  
		Last Modified: Fri, 15 May 2020 15:43:55 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a854515df625c06ba3321bce8ff4c910fac6c639d736cf7cdd66e1a88adab36`  
		Last Modified: Fri, 15 May 2020 15:43:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac1ba4a1ebfce49416ed9341a80f27861585759fcda5895932f9fe3dccc54e7`  
		Last Modified: Fri, 15 May 2020 15:43:55 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e40562f13215b7bbce03df57f3d700cb4618dcf01361e2a5f170055101cb5a0`  
		Last Modified: Fri, 15 May 2020 15:44:13 GMT  
		Size: 38.4 MB (38403029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacy` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:b37cdbf4c4a9f1d71077a9045d6338164b96677e00d2d6a1846c7616723eaba3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **272.6 MB (272630469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fdb9d5a9d4eb3d5fdb5bc0f328473ae021ac26abe6bb132051380bdfeee1fad`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 10:39:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Mon, 18 May 2020 10:39:45 GMT
ENV PHP_VERSION=7.2.31
# Mon, 18 May 2020 10:39:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Mon, 18 May 2020 10:39:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Mon, 18 May 2020 10:42:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 10:42:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 10:47:07 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:17 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 10:47:26 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 10:47:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 10:47:34 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 10:47:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:39 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 10:47:41 GMT
EXPOSE 80
# Mon, 18 May 2020 10:47:43 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:51:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:53:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:53:58 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Mon, 18 May 2020 19:54:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:54:20 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:54:24 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.33
# Mon, 18 May 2020 19:54:26 GMT
ENV MEDIAWIKI_BRANCH=REL1_33
# Mon, 18 May 2020 19:54:33 GMT
ENV MEDIAWIKI_VERSION=1.33.3
# Mon, 18 May 2020 19:54:42 GMT
ENV MEDIAWIKI_SHA512=edca9810ad105a1018808bfc253c567c9d3841d606ce9e224f3b49e9f5e9f0ca7bf6599fb8dfa83473f1aca8102480bd38e65eede9f1a45144737d998881123e
# Mon, 18 May 2020 19:55:27 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422d598ad54ce6e95730222751503d9b698243cf90a702ad65e2d4631964790b`  
		Last Modified: Mon, 18 May 2020 12:30:00 GMT  
		Size: 12.6 MB (12648662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1981bd0a5f519849b6b58bcf91970f04a47d652e69fe60ac7ab816477283bb`  
		Last Modified: Mon, 18 May 2020 12:29:50 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a723077ecd7e1721f12f36dabd59b626018e3ed70e28d2933f8033c0885179`  
		Last Modified: Mon, 18 May 2020 12:30:08 GMT  
		Size: 14.9 MB (14857939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931596f7dd07359c094e8c5ce6911e9b4f4dd67bb1a11dec735da42f2507236d`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 2.2 KB (2235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cc1daefd84c15ae993c001ad437714bec6b0c7193b7974dd4bbc496d4d3741`  
		Last Modified: Mon, 18 May 2020 12:29:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666d43f8152a6bbf980f795024b39f5011f8a9f8c55f5d4053c973e9c4a1b43`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b330e8c37cbe3045afe862d0defb2365a798a12fceb4484dc2d0683819efa295`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922138725c394061a32405f8fb772954e20eb97e25a5d36c3f6655fc435f6b8`  
		Last Modified: Mon, 18 May 2020 20:02:56 GMT  
		Size: 71.3 MB (71260606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5203e563f1cf9a02c440e94ed4f6afb43648404a70e0916a8db25357f6809f1b`  
		Last Modified: Mon, 18 May 2020 20:01:30 GMT  
		Size: 2.9 MB (2855225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efd3e6ea5dbeec916c6410d03d6f17b4eac74582b7b7ca78ea4eae5b24430e`  
		Last Modified: Mon, 18 May 2020 20:01:25 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7ec02c6577c567385cc72505ac006b3f6c5c2abd54ac5c95a3df382eecf888`  
		Last Modified: Mon, 18 May 2020 20:01:26 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dde02b1527ca67ce7a4d212825417c27bb340054f4c54951bca032fbc767fd9`  
		Last Modified: Mon, 18 May 2020 20:01:26 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2de52b8e356a6abd3d1871df0c97dfdce7d4f199862bc7286b03d5c54eb5bd`  
		Last Modified: Mon, 18 May 2020 20:03:13 GMT  
		Size: 38.4 MB (38403277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:legacylts`

```console
$ docker pull mediawiki@sha256:5176842e2050332682288e83db7c341a83bfe4570f3fcd1ad898904a19c922e8
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
$ docker pull mediawiki@sha256:f675c8e6ca0a2dba64611b2a916e768145eba50a2689ef9c965a9dbb45b73556
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251882389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb9f6a83f744e7bf771f96d0dcd49a573b37cd4a7680aa88123402323e52c84b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 14:23:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 14:23:53 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 14:24:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 14:24:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 14:28:04 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 14:28:06 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 14:28:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 14:28:06 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 14:28:06 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:06 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 14:28:07 GMT
EXPOSE 80
# Fri, 15 May 2020 14:28:07 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:10:39 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:12:41 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 16:12:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e342cb20e11a1dd9d7c623fa9432bd079fde2b090476b3134baf0c21d40612a`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 12.6 MB (12648389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c591e1fe994da44df77bd8b6ad18ed428e3d1e7f76c83349d61cf8fa06beab4d`  
		Last Modified: Fri, 15 May 2020 15:11:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e231d94c7c66658f89cc128cad35ec1e8e08f2bba42fd7ca4c2d1933d66910ac`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 13.8 MB (13820369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16787fbb561735285d261bea91186df225573e4b193a7592d4ec49acc32d084`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf849c308b829343ad910dacfe26fea7cf2dfa9dbdc0b3f3a08e1c98222a0162`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d8b80f0c7f4669d6b6e1ed2ecff96de24ee0f969520b367f94df418d5156e0`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca082ed920d4a38e00a209eb7e17c1a8ae106cfe67ecf14accca6b19cb4f447`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea1efaf50e775702242a3eff9784b093e3600ed495d0d6a17a3a58801ff95a1`  
		Last Modified: Fri, 15 May 2020 16:13:49 GMT  
		Size: 64.4 MB (64438938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c31e8e8dd500a452bf4fb65bef4b53cb90b55104201023790cd8eb3b11fd1c9`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 2.8 MB (2780306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33dc37249be4cc31520a2516d4f67ade63354dc7ff49ad6b0e8673902bd54c3`  
		Last Modified: Fri, 15 May 2020 16:14:03 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f85ce9298260b76daa7b6ddcbe7e22e66d75a11e19000d172ee8fdf5ecd3a0c`  
		Last Modified: Fri, 15 May 2020 16:14:03 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b607dca168b949fbdad65fc55f6d5c9147a80b459ef8b31078ef8ad5658d6a`  
		Last Modified: Fri, 15 May 2020 16:14:14 GMT  
		Size: 35.8 MB (35761633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacylts` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:181b23f356406ec27652ae93cdf04257f37209d4d3b8c53d4118accfc612ec29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226437533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cbd3309a5ba147b5c72762e94f49d101f5ee0c15ec30d55001f6ecfaea0f0b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:55:21 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 May 2020 23:55:22 GMT
ENV PHP_VERSION=7.2.31
# Thu, 14 May 2020 23:55:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Thu, 14 May 2020 23:55:25 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Thu, 14 May 2020 23:55:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:55:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:59:14 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:59:19 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:59:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:59:20 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:59:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:22 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:59:23 GMT
EXPOSE 80
# Thu, 14 May 2020 23:59:23 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:50:28 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:52:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:53:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:53:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:53:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 01:53:20 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 01:53:21 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 01:53:21 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 01:53:42 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6825e5831098a7455da6208d36a8631cf5e2823f499953e959a93d2825d216`  
		Last Modified: Fri, 15 May 2020 00:36:52 GMT  
		Size: 12.6 MB (12646387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c90c04c008327b286591e8e09268bce6fb4e7f4f23f3ecd5e756a8b4e5542`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a57b44810b99bff28e6eae7a26a7e63ee4096f279fbe1bfcf664e6273e41714`  
		Last Modified: Fri, 15 May 2020 00:36:53 GMT  
		Size: 12.9 MB (12893543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7a380e949112ca73a08930f495f01082945469b745a50ff5117e6694418b9`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019bfed0e017e52b99ae6700fd766ea74dcd69819f030e640cc2038a720a060e`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec0f544a95469ff33ebce02ed759bdab577bee1ecc6b52e27535b50190afe9d`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059248e2c7e804da9d7b61c6e9d1ca5845709a53347be8b1cd7323c6a38fcc26`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9be3987479af508dffc0cc23bcbacd781b00f13a165a4c554683d6ffde9d4b`  
		Last Modified: Fri, 15 May 2020 01:55:01 GMT  
		Size: 60.8 MB (60766733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57931c4fa281330d8a2a1e6f7ec30e9d57ca8dd99fda7147cdc0822b0be9d29e`  
		Last Modified: Fri, 15 May 2020 01:54:41 GMT  
		Size: 2.7 MB (2699845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d629bc11e6a1afbc207740507c6b99bc2ad69d629a6d4d3440e21e27e628b6`  
		Last Modified: Fri, 15 May 2020 01:55:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8221e24aea8426213ec533916ababeecfaeb20ca923a35facbf59429b2cb2716`  
		Last Modified: Fri, 15 May 2020 01:55:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a1ef64a11d60ac8a94e89b261e655dba843b0a07ab48eae4e2ac406b1be330`  
		Last Modified: Fri, 15 May 2020 01:55:27 GMT  
		Size: 35.8 MB (35762057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacylts` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:bb45aad9d109c0cff5afb8609036166897fffbeaadcc796e3781ee83ece22187
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.0 MB (219970207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75d2cc7515ec9a1b95fd63c3e6b3010cbf907687f0250ec968f04fd67a427e61`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:35:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 05:35:19 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 05:35:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 05:35:21 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 05:35:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:35:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:38:37 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:38:40 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:38:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:38:42 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:38:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:43 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:38:43 GMT
EXPOSE 80
# Fri, 15 May 2020 05:38:44 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:37:32 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:39:55 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:39:56 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 07:39:57 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 07:39:57 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 07:39:58 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 07:40:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398113638833857603dca55979da57419d2a5572563cafe1334991af81967142`  
		Last Modified: Fri, 15 May 2020 06:10:24 GMT  
		Size: 12.6 MB (12646418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7959af5842bab4cdea3f1bb587ccf5276a5a9ec306f7549e37c48681732acc`  
		Last Modified: Fri, 15 May 2020 06:10:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ff876ade20645d6ddc3d2b59a603be87a04f0b62827c4665c3f132b44bb823`  
		Last Modified: Fri, 15 May 2020 06:10:25 GMT  
		Size: 12.2 MB (12163941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89eb8d735c9a88db8e9415f7968d824dea1e8ce48775e1f518eac6711f83aa5`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6835a065ff97b202cd23f0f4b753c4d136a169058eacad5989eff11767d592a`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385d20ac491870d83092377014337cc2858d8a8ad5fa34cc5ceb8127c81268d0`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8d5374463d9560454a440a6420fb6b8dfdac2ffe2094ce4390ada18219a7d`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36abbaec8998eb3a82a64613df5bc8258ec9a97630ef2e66abf147adbe44f836`  
		Last Modified: Fri, 15 May 2020 07:41:32 GMT  
		Size: 57.1 MB (57061094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44693c5b4c0ba701dc090f4d812ec58b9769563cd6a75d28d816fe64d1597d1c`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 2.6 MB (2641042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0bbdc1a3038c8e8bb6c476e51757e9e6127183edb412c913d112965f251144`  
		Last Modified: Fri, 15 May 2020 07:41:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5da091af18cb7439249bb6314c3caf4f208a378f3506025bd0aa5bb2fe7524`  
		Last Modified: Fri, 15 May 2020 07:41:42 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7dcf2d8bad80dde7b446926234306961b3c6ffd1ed2cc6ec1fc8944c964c`  
		Last Modified: Fri, 15 May 2020 07:42:01 GMT  
		Size: 35.8 MB (35762010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacylts` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:787472e32803f153474046c3d6e8567242c5e4958aaa6be6fff30f3d3ee19eec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241693952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecc258368bab8df819d24c9023f2720c8393c3e4e16473cc708f030a2179dee`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:43:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 15:43:10 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 15:43:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 15:43:12 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 15:43:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:43:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:46:26 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:46:30 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:46:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:46:32 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:46:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:34 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:46:35 GMT
EXPOSE 80
# Fri, 15 May 2020 15:46:36 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:50:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:53:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:53:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:53:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 19:53:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 19:53:14 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 19:53:16 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 19:53:30 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87c94fdf28f180d95beba9bf62a84566232ed0ccc85839454cfe7f70498d39`  
		Last Modified: Fri, 15 May 2020 16:20:17 GMT  
		Size: 12.6 MB (12647169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd1d4d985393bba996ffbfdeeb1fc32bcb60b185e25e89516dc194d45c9bfee`  
		Last Modified: Fri, 15 May 2020 16:20:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfd1ad71cc2afd1e01539eec4fa66cb9041b028439a810dc8ef3462d6bfd9e3`  
		Last Modified: Fri, 15 May 2020 16:20:09 GMT  
		Size: 13.5 MB (13517080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1a76aeff57626d8acad75f39da3a39cc866b022ed90a6c743ba8e03ebf5bf`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91781f686504a79cb5c3a9ac44c847e82581db2bac375061f90aa7f401a1d38a`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a4c663a05696bf7ccb08382bef8932d7007cc3efae03cd914f100d1d33a074`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a5c61103dcbd74aed611a358358a9362c4e6da5b98ee8319bbb5b12552c697`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea3f778184af99b72385b780d7c9b4fbb5c9a001a764eada8da384a5bfbb5df`  
		Last Modified: Fri, 15 May 2020 19:54:38 GMT  
		Size: 62.2 MB (62238977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1daf0fab3fde127e7446d705cb687ab4511d7dc90edd8be244ccd98520a784f`  
		Last Modified: Fri, 15 May 2020 19:54:22 GMT  
		Size: 2.8 MB (2750463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d0ac654d18ee14a8dbed833a764067c883bf569686ffbb5891fca9eda6ae0b`  
		Last Modified: Fri, 15 May 2020 19:54:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa07d03ce00c5da6acb550c3867ca2ff5d5393ade79556196636b2e30478644`  
		Last Modified: Fri, 15 May 2020 19:54:45 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66840e504bf2520d1897c55db6fdc79c9149f3c1519209f0b703b3522211c877`  
		Last Modified: Fri, 15 May 2020 19:55:01 GMT  
		Size: 35.8 MB (35762208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacylts` - linux; 386

```console
$ docker pull mediawiki@sha256:1e6922f6fde549dddba1148486f1297f31b67bba9f38527dd5ed2e652b0fd540
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.8 MB (259785687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38de43bfa9877383e56d982f373037f3daa9c872b5946fab8954d1f316cd370d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:29:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 13:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:30:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:35:35 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:35:37 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:35:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:35:37 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:35:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:38 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:35:38 GMT
EXPOSE 80
# Fri, 15 May 2020 13:35:38 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:41:07 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:42:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:43:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:43:04 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:43:04 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 15:43:04 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 15:43:05 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 15:43:05 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 15:43:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14739e799f47da9c256b708f19578335422750fa82325e096a0fdbd0063dcd8`  
		Last Modified: Fri, 15 May 2020 14:35:18 GMT  
		Size: 12.6 MB (12647664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6602cc810aeb39612ffd93aaf08e6a834bd6a23306b89e007274aa317a9388e7`  
		Last Modified: Fri, 15 May 2020 14:35:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590038160b7b9aa93fbc6ca56843fce86d0f211c74e6f1ace6517f9743938740`  
		Last Modified: Fri, 15 May 2020 14:35:26 GMT  
		Size: 14.1 MB (14142560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f027994bbcc3b11ce489c8b38b2e60498e299fa93b3e7be031676c5cb44e5f37`  
		Last Modified: Fri, 15 May 2020 14:35:14 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aec20265c263a1cad53ad047b72af420de2ec322def253cc491fae7b2d9e6c4`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36479c1104bd5c974f4cf08ae38eb1c21dd1bc34c302c6134a0a5741b51d4efc`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5822ef93d09deb9b8d52cfb9e2ccda9b23b28b42c4c22de223caf7866f0b6081`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1ae57a5c23c1e2e03c3ff891870e6c4bcc5c08d9f12dc4f8d9632fe23a2cbd`  
		Last Modified: Fri, 15 May 2020 15:44:16 GMT  
		Size: 66.4 MB (66394484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a6b6b20b38b12032d751706bf19192545484b51348ea74aaff21a34cecd016`  
		Last Modified: Fri, 15 May 2020 15:43:56 GMT  
		Size: 2.8 MB (2767085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5300867f21fc2a48e18e2ca2d1cd7cf8c9e58670d402c7dca32d274035621e7`  
		Last Modified: Fri, 15 May 2020 15:44:22 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85f24a2d3c21d4a59299f89483535ba8cde0a2a00863559627e656945cb6144`  
		Last Modified: Fri, 15 May 2020 15:44:22 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495ece39a90aeb76c551073eb6bc952a847cb5194d17827b46d0f137204e9061`  
		Last Modified: Fri, 15 May 2020 15:44:40 GMT  
		Size: 35.8 MB (35761567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:legacylts` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:1bff05c73642df000737e01db2fb4e09810834d0a4f84560a06da2a5bf70eb2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.0 MB (269988737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53d1b5abae3037bac89d9935218a2749efe7220bd3c01f115a902959b2606bfa`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 10:39:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Mon, 18 May 2020 10:39:45 GMT
ENV PHP_VERSION=7.2.31
# Mon, 18 May 2020 10:39:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Mon, 18 May 2020 10:39:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Mon, 18 May 2020 10:42:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 10:42:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 10:47:07 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:17 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 10:47:26 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 10:47:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 10:47:34 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 10:47:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:39 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 10:47:41 GMT
EXPOSE 80
# Mon, 18 May 2020 10:47:43 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:51:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:53:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:56:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:56:27 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:56:31 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Mon, 18 May 2020 19:56:33 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Mon, 18 May 2020 19:56:39 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Mon, 18 May 2020 19:56:42 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Mon, 18 May 2020 19:57:43 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422d598ad54ce6e95730222751503d9b698243cf90a702ad65e2d4631964790b`  
		Last Modified: Mon, 18 May 2020 12:30:00 GMT  
		Size: 12.6 MB (12648662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1981bd0a5f519849b6b58bcf91970f04a47d652e69fe60ac7ab816477283bb`  
		Last Modified: Mon, 18 May 2020 12:29:50 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a723077ecd7e1721f12f36dabd59b626018e3ed70e28d2933f8033c0885179`  
		Last Modified: Mon, 18 May 2020 12:30:08 GMT  
		Size: 14.9 MB (14857939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931596f7dd07359c094e8c5ce6911e9b4f4dd67bb1a11dec735da42f2507236d`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 2.2 KB (2235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cc1daefd84c15ae993c001ad437714bec6b0c7193b7974dd4bbc496d4d3741`  
		Last Modified: Mon, 18 May 2020 12:29:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666d43f8152a6bbf980f795024b39f5011f8a9f8c55f5d4053c973e9c4a1b43`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b330e8c37cbe3045afe862d0defb2365a798a12fceb4484dc2d0683819efa295`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922138725c394061a32405f8fb772954e20eb97e25a5d36c3f6655fc435f6b8`  
		Last Modified: Mon, 18 May 2020 20:02:56 GMT  
		Size: 71.3 MB (71260606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5203e563f1cf9a02c440e94ed4f6afb43648404a70e0916a8db25357f6809f1b`  
		Last Modified: Mon, 18 May 2020 20:01:30 GMT  
		Size: 2.9 MB (2855225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90beeed004f02c7c0a8ff240d4d4327a23ceb8a4171df2bcbfd5727e0dede5a3`  
		Last Modified: Mon, 18 May 2020 20:03:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705f0367663dcd4a8656e85075b3278da811124d25393476ef6b77d59112b04`  
		Last Modified: Mon, 18 May 2020 20:03:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f49dc71c3af4a18627392c2d8c683f005b09a5803bb6522cc4e1fed74f5d0e`  
		Last Modified: Mon, 18 May 2020 20:04:35 GMT  
		Size: 35.8 MB (35762126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:lts`

```console
$ docker pull mediawiki@sha256:5176842e2050332682288e83db7c341a83bfe4570f3fcd1ad898904a19c922e8
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
$ docker pull mediawiki@sha256:f675c8e6ca0a2dba64611b2a916e768145eba50a2689ef9c965a9dbb45b73556
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251882389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb9f6a83f744e7bf771f96d0dcd49a573b37cd4a7680aa88123402323e52c84b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 14:23:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 14:23:53 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 14:23:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 14:24:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 14:24:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 14:28:04 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 14:28:06 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 14:28:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 14:28:06 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 14:28:06 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 14:28:06 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 14:28:07 GMT
EXPOSE 80
# Fri, 15 May 2020 14:28:07 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:10:39 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:12:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:12:41 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 16:12:41 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 16:12:49 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e342cb20e11a1dd9d7c623fa9432bd079fde2b090476b3134baf0c21d40612a`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 12.6 MB (12648389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c591e1fe994da44df77bd8b6ad18ed428e3d1e7f76c83349d61cf8fa06beab4d`  
		Last Modified: Fri, 15 May 2020 15:11:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e231d94c7c66658f89cc128cad35ec1e8e08f2bba42fd7ca4c2d1933d66910ac`  
		Last Modified: Fri, 15 May 2020 15:11:16 GMT  
		Size: 13.8 MB (13820369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16787fbb561735285d261bea91186df225573e4b193a7592d4ec49acc32d084`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf849c308b829343ad910dacfe26fea7cf2dfa9dbdc0b3f3a08e1c98222a0162`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d8b80f0c7f4669d6b6e1ed2ecff96de24ee0f969520b367f94df418d5156e0`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca082ed920d4a38e00a209eb7e17c1a8ae106cfe67ecf14accca6b19cb4f447`  
		Last Modified: Fri, 15 May 2020 15:11:13 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea1efaf50e775702242a3eff9784b093e3600ed495d0d6a17a3a58801ff95a1`  
		Last Modified: Fri, 15 May 2020 16:13:49 GMT  
		Size: 64.4 MB (64438938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c31e8e8dd500a452bf4fb65bef4b53cb90b55104201023790cd8eb3b11fd1c9`  
		Last Modified: Fri, 15 May 2020 16:13:33 GMT  
		Size: 2.8 MB (2780306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33dc37249be4cc31520a2516d4f67ade63354dc7ff49ad6b0e8673902bd54c3`  
		Last Modified: Fri, 15 May 2020 16:14:03 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f85ce9298260b76daa7b6ddcbe7e22e66d75a11e19000d172ee8fdf5ecd3a0c`  
		Last Modified: Fri, 15 May 2020 16:14:03 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b607dca168b949fbdad65fc55f6d5c9147a80b459ef8b31078ef8ad5658d6a`  
		Last Modified: Fri, 15 May 2020 16:14:14 GMT  
		Size: 35.8 MB (35761633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:181b23f356406ec27652ae93cdf04257f37209d4d3b8c53d4118accfc612ec29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226437533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46cbd3309a5ba147b5c72762e94f49d101f5ee0c15ec30d55001f6ecfaea0f0b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:55:21 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 14 May 2020 23:55:22 GMT
ENV PHP_VERSION=7.2.31
# Thu, 14 May 2020 23:55:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Thu, 14 May 2020 23:55:25 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Thu, 14 May 2020 23:55:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:55:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:59:14 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:59:19 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:59:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:59:20 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:59:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:59:22 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:59:23 GMT
EXPOSE 80
# Thu, 14 May 2020 23:59:23 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:50:28 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:52:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:53:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:53:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:53:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 01:53:20 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 01:53:21 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 01:53:21 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 01:53:42 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6825e5831098a7455da6208d36a8631cf5e2823f499953e959a93d2825d216`  
		Last Modified: Fri, 15 May 2020 00:36:52 GMT  
		Size: 12.6 MB (12646387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c90c04c008327b286591e8e09268bce6fb4e7f4f23f3ecd5e756a8b4e5542`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a57b44810b99bff28e6eae7a26a7e63ee4096f279fbe1bfcf664e6273e41714`  
		Last Modified: Fri, 15 May 2020 00:36:53 GMT  
		Size: 12.9 MB (12893543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e7a380e949112ca73a08930f495f01082945469b745a50ff5117e6694418b9`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019bfed0e017e52b99ae6700fd766ea74dcd69819f030e640cc2038a720a060e`  
		Last Modified: Fri, 15 May 2020 00:36:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec0f544a95469ff33ebce02ed759bdab577bee1ecc6b52e27535b50190afe9d`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059248e2c7e804da9d7b61c6e9d1ca5845709a53347be8b1cd7323c6a38fcc26`  
		Last Modified: Fri, 15 May 2020 00:36:48 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9be3987479af508dffc0cc23bcbacd781b00f13a165a4c554683d6ffde9d4b`  
		Last Modified: Fri, 15 May 2020 01:55:01 GMT  
		Size: 60.8 MB (60766733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57931c4fa281330d8a2a1e6f7ec30e9d57ca8dd99fda7147cdc0822b0be9d29e`  
		Last Modified: Fri, 15 May 2020 01:54:41 GMT  
		Size: 2.7 MB (2699845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d629bc11e6a1afbc207740507c6b99bc2ad69d629a6d4d3440e21e27e628b6`  
		Last Modified: Fri, 15 May 2020 01:55:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8221e24aea8426213ec533916ababeecfaeb20ca923a35facbf59429b2cb2716`  
		Last Modified: Fri, 15 May 2020 01:55:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a1ef64a11d60ac8a94e89b261e655dba843b0a07ab48eae4e2ac406b1be330`  
		Last Modified: Fri, 15 May 2020 01:55:27 GMT  
		Size: 35.8 MB (35762057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:bb45aad9d109c0cff5afb8609036166897fffbeaadcc796e3781ee83ece22187
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.0 MB (219970207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75d2cc7515ec9a1b95fd63c3e6b3010cbf907687f0250ec968f04fd67a427e61`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:35:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 05:35:19 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 05:35:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 05:35:21 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 05:35:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:35:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:38:37 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:38:40 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:38:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:38:42 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:38:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:38:43 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:38:43 GMT
EXPOSE 80
# Fri, 15 May 2020 05:38:44 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:37:32 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:39:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:39:55 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:39:56 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 07:39:57 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 07:39:57 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 07:39:58 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 07:40:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398113638833857603dca55979da57419d2a5572563cafe1334991af81967142`  
		Last Modified: Fri, 15 May 2020 06:10:24 GMT  
		Size: 12.6 MB (12646418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af7959af5842bab4cdea3f1bb587ccf5276a5a9ec306f7549e37c48681732acc`  
		Last Modified: Fri, 15 May 2020 06:10:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ff876ade20645d6ddc3d2b59a603be87a04f0b62827c4665c3f132b44bb823`  
		Last Modified: Fri, 15 May 2020 06:10:25 GMT  
		Size: 12.2 MB (12163941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89eb8d735c9a88db8e9415f7968d824dea1e8ce48775e1f518eac6711f83aa5`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6835a065ff97b202cd23f0f4b753c4d136a169058eacad5989eff11767d592a`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385d20ac491870d83092377014337cc2858d8a8ad5fa34cc5ceb8127c81268d0`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8d5374463d9560454a440a6420fb6b8dfdac2ffe2094ce4390ada18219a7d`  
		Last Modified: Fri, 15 May 2020 06:10:21 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36abbaec8998eb3a82a64613df5bc8258ec9a97630ef2e66abf147adbe44f836`  
		Last Modified: Fri, 15 May 2020 07:41:32 GMT  
		Size: 57.1 MB (57061094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44693c5b4c0ba701dc090f4d812ec58b9769563cd6a75d28d816fe64d1597d1c`  
		Last Modified: Fri, 15 May 2020 07:41:12 GMT  
		Size: 2.6 MB (2641042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0bbdc1a3038c8e8bb6c476e51757e9e6127183edb412c913d112965f251144`  
		Last Modified: Fri, 15 May 2020 07:41:43 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5da091af18cb7439249bb6314c3caf4f208a378f3506025bd0aa5bb2fe7524`  
		Last Modified: Fri, 15 May 2020 07:41:42 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7dcf2d8bad80dde7b446926234306961b3c6ffd1ed2cc6ec1fc8944c964c`  
		Last Modified: Fri, 15 May 2020 07:42:01 GMT  
		Size: 35.8 MB (35762010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:787472e32803f153474046c3d6e8567242c5e4958aaa6be6fff30f3d3ee19eec
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241693952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecc258368bab8df819d24c9023f2720c8393c3e4e16473cc708f030a2179dee`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:43:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 15:43:10 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 15:43:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 15:43:12 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 15:43:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:43:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:46:26 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:46:30 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:46:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:46:32 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:46:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:46:34 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:46:35 GMT
EXPOSE 80
# Fri, 15 May 2020 15:46:36 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:50:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:53:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:53:11 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:53:12 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 19:53:13 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 19:53:14 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 19:53:16 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 19:53:30 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b87c94fdf28f180d95beba9bf62a84566232ed0ccc85839454cfe7f70498d39`  
		Last Modified: Fri, 15 May 2020 16:20:17 GMT  
		Size: 12.6 MB (12647169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd1d4d985393bba996ffbfdeeb1fc32bcb60b185e25e89516dc194d45c9bfee`  
		Last Modified: Fri, 15 May 2020 16:20:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfd1ad71cc2afd1e01539eec4fa66cb9041b028439a810dc8ef3462d6bfd9e3`  
		Last Modified: Fri, 15 May 2020 16:20:09 GMT  
		Size: 13.5 MB (13517080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1a76aeff57626d8acad75f39da3a39cc866b022ed90a6c743ba8e03ebf5bf`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 2.2 KB (2232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91781f686504a79cb5c3a9ac44c847e82581db2bac375061f90aa7f401a1d38a`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a4c663a05696bf7ccb08382bef8932d7007cc3efae03cd914f100d1d33a074`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a5c61103dcbd74aed611a358358a9362c4e6da5b98ee8319bbb5b12552c697`  
		Last Modified: Fri, 15 May 2020 16:20:05 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea3f778184af99b72385b780d7c9b4fbb5c9a001a764eada8da384a5bfbb5df`  
		Last Modified: Fri, 15 May 2020 19:54:38 GMT  
		Size: 62.2 MB (62238977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1daf0fab3fde127e7446d705cb687ab4511d7dc90edd8be244ccd98520a784f`  
		Last Modified: Fri, 15 May 2020 19:54:22 GMT  
		Size: 2.8 MB (2750463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d0ac654d18ee14a8dbed833a764067c883bf569686ffbb5891fca9eda6ae0b`  
		Last Modified: Fri, 15 May 2020 19:54:45 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa07d03ce00c5da6acb550c3867ca2ff5d5393ade79556196636b2e30478644`  
		Last Modified: Fri, 15 May 2020 19:54:45 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66840e504bf2520d1897c55db6fdc79c9149f3c1519209f0b703b3522211c877`  
		Last Modified: Fri, 15 May 2020 19:55:01 GMT  
		Size: 35.8 MB (35762208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; 386

```console
$ docker pull mediawiki@sha256:1e6922f6fde549dddba1148486f1297f31b67bba9f38527dd5ed2e652b0fd540
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.8 MB (259785687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38de43bfa9877383e56d982f373037f3daa9c872b5946fab8954d1f316cd370d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:29:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_VERSION=7.2.31
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Fri, 15 May 2020 13:29:47 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Fri, 15 May 2020 13:30:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:30:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:35:35 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:35:37 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:35:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:35:37 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:35:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:35:38 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:35:38 GMT
EXPOSE 80
# Fri, 15 May 2020 13:35:38 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:41:07 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:42:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:43:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:43:04 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:43:04 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Fri, 15 May 2020 15:43:04 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Fri, 15 May 2020 15:43:05 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Fri, 15 May 2020 15:43:05 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Fri, 15 May 2020 15:43:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14739e799f47da9c256b708f19578335422750fa82325e096a0fdbd0063dcd8`  
		Last Modified: Fri, 15 May 2020 14:35:18 GMT  
		Size: 12.6 MB (12647664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6602cc810aeb39612ffd93aaf08e6a834bd6a23306b89e007274aa317a9388e7`  
		Last Modified: Fri, 15 May 2020 14:35:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590038160b7b9aa93fbc6ca56843fce86d0f211c74e6f1ace6517f9743938740`  
		Last Modified: Fri, 15 May 2020 14:35:26 GMT  
		Size: 14.1 MB (14142560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f027994bbcc3b11ce489c8b38b2e60498e299fa93b3e7be031676c5cb44e5f37`  
		Last Modified: Fri, 15 May 2020 14:35:14 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aec20265c263a1cad53ad047b72af420de2ec322def253cc491fae7b2d9e6c4`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36479c1104bd5c974f4cf08ae38eb1c21dd1bc34c302c6134a0a5741b51d4efc`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5822ef93d09deb9b8d52cfb9e2ccda9b23b28b42c4c22de223caf7866f0b6081`  
		Last Modified: Fri, 15 May 2020 14:35:15 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1ae57a5c23c1e2e03c3ff891870e6c4bcc5c08d9f12dc4f8d9632fe23a2cbd`  
		Last Modified: Fri, 15 May 2020 15:44:16 GMT  
		Size: 66.4 MB (66394484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a6b6b20b38b12032d751706bf19192545484b51348ea74aaff21a34cecd016`  
		Last Modified: Fri, 15 May 2020 15:43:56 GMT  
		Size: 2.8 MB (2767085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5300867f21fc2a48e18e2ca2d1cd7cf8c9e58670d402c7dca32d274035621e7`  
		Last Modified: Fri, 15 May 2020 15:44:22 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85f24a2d3c21d4a59299f89483535ba8cde0a2a00863559627e656945cb6144`  
		Last Modified: Fri, 15 May 2020 15:44:22 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495ece39a90aeb76c551073eb6bc952a847cb5194d17827b46d0f137204e9061`  
		Last Modified: Fri, 15 May 2020 15:44:40 GMT  
		Size: 35.8 MB (35761567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:lts` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:1bff05c73642df000737e01db2fb4e09810834d0a4f84560a06da2a5bf70eb2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **270.0 MB (269988737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53d1b5abae3037bac89d9935218a2749efe7220bd3c01f115a902959b2606bfa`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 10:39:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Mon, 18 May 2020 10:39:45 GMT
ENV PHP_VERSION=7.2.31
# Mon, 18 May 2020 10:39:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.2.31.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.2.31.tar.xz.asc
# Mon, 18 May 2020 10:39:54 GMT
ENV PHP_SHA256=8beaa634bb878a96af9bc8643811ea46973f5f41ad2bfb6ab4cfd290e5a39806 PHP_MD5=
# Mon, 18 May 2020 10:42:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 10:42:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 10:47:07 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:17 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 10:47:26 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 10:47:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 10:47:34 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 10:47:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 10:47:39 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 10:47:41 GMT
EXPOSE 80
# Mon, 18 May 2020 10:47:43 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:51:25 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:53:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.17; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:56:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:56:27 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:56:31 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.31
# Mon, 18 May 2020 19:56:33 GMT
ENV MEDIAWIKI_BRANCH=REL1_31
# Mon, 18 May 2020 19:56:39 GMT
ENV MEDIAWIKI_VERSION=1.31.7
# Mon, 18 May 2020 19:56:42 GMT
ENV MEDIAWIKI_SHA512=7cd106bc775f1c3997786f0bb3e2412e30d0338133d6b9c6fb7af2550c519c57b0c274095747bbb5469a59e6511206953577b7b31bfc659b82f1583620482c1b
# Mon, 18 May 2020 19:57:43 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422d598ad54ce6e95730222751503d9b698243cf90a702ad65e2d4631964790b`  
		Last Modified: Mon, 18 May 2020 12:30:00 GMT  
		Size: 12.6 MB (12648662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1981bd0a5f519849b6b58bcf91970f04a47d652e69fe60ac7ab816477283bb`  
		Last Modified: Mon, 18 May 2020 12:29:50 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a723077ecd7e1721f12f36dabd59b626018e3ed70e28d2933f8033c0885179`  
		Last Modified: Mon, 18 May 2020 12:30:08 GMT  
		Size: 14.9 MB (14857939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931596f7dd07359c094e8c5ce6911e9b4f4dd67bb1a11dec735da42f2507236d`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 2.2 KB (2235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cc1daefd84c15ae993c001ad437714bec6b0c7193b7974dd4bbc496d4d3741`  
		Last Modified: Mon, 18 May 2020 12:29:32 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6666d43f8152a6bbf980f795024b39f5011f8a9f8c55f5d4053c973e9c4a1b43`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b330e8c37cbe3045afe862d0defb2365a798a12fceb4484dc2d0683819efa295`  
		Last Modified: Mon, 18 May 2020 12:29:37 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1922138725c394061a32405f8fb772954e20eb97e25a5d36c3f6655fc435f6b8`  
		Last Modified: Mon, 18 May 2020 20:02:56 GMT  
		Size: 71.3 MB (71260606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5203e563f1cf9a02c440e94ed4f6afb43648404a70e0916a8db25357f6809f1b`  
		Last Modified: Mon, 18 May 2020 20:01:30 GMT  
		Size: 2.9 MB (2855225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90beeed004f02c7c0a8ff240d4d4327a23ceb8a4171df2bcbfd5727e0dede5a3`  
		Last Modified: Mon, 18 May 2020 20:03:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6705f0367663dcd4a8656e85075b3278da811124d25393476ef6b77d59112b04`  
		Last Modified: Mon, 18 May 2020 20:03:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f49dc71c3af4a18627392c2d8c683f005b09a5803bb6522cc4e1fed74f5d0e`  
		Last Modified: Mon, 18 May 2020 20:04:35 GMT  
		Size: 35.8 MB (35762126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `mediawiki:stable`

```console
$ docker pull mediawiki@sha256:bb832ca583c8a9f8dec7c81f3e6f16c7f475b6b893cef161640d53272eaacc7a
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
$ docker pull mediawiki@sha256:29b19fb44ba857f5a784c06d16db4dc7b7e97728f7722986881a545712a570ae
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.2 MB (257167590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec57d9a3fb725cc77dec57b49e2a0e48308d0373f7f9d7d7a2f195cfdea5fb91`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 06:28:44 GMT
ADD file:7780c81c33e6cc5b6261af4a6c611cce0f39dec3131009bb297e65f12020c150 in / 
# Fri, 15 May 2020 06:28:44 GMT
CMD ["bash"]
# Fri, 15 May 2020 12:41:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 12:41:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 12:41:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 12:41:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 12:41:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 12:49:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 12:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 12:49:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 12:49:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 12:49:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 12:49:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 13:21:15 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 13:21:16 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 13:21:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 13:21:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 13:27:10 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:11 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 13:27:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 13:27:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 13:27:13 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 13:27:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 13:27:14 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 13:27:15 GMT
EXPOSE 80
# Fri, 15 May 2020 13:27:15 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 16:08:06 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:09:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 16:09:39 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 16:09:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 16:09:40 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 16:09:41 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 16:09:50 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:afb6ec6fdc1c3ba04f7a56db32c5ff5ff38962dc4cd0ffdef5beaa0ce2eb77e2`  
		Last Modified: Fri, 15 May 2020 06:37:39 GMT  
		Size: 27.1 MB (27098756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d895574014b07620962dc74d8e480e4629fbb3afb45c2bf57249a6ec1a0e64c`  
		Last Modified: Fri, 15 May 2020 15:07:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c309fdad64103ed6195af8392df8834b3ba6c40ff2070a2230d835960c41e10b`  
		Last Modified: Fri, 15 May 2020 15:07:25 GMT  
		Size: 76.7 MB (76652092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c201f6a5d6f95f92d66f943b5413d3637ec1fce1735885558bca16f7302bfaed`  
		Last Modified: Fri, 15 May 2020 15:07:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f853892aac5282dcd651f71ce35d32c4f66c6c1e6864a13b10100dff4c1d5`  
		Last Modified: Fri, 15 May 2020 15:07:44 GMT  
		Size: 18.7 MB (18675995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b2113b4005b0fc3cd483f8ec5e00202376f2b89a050cd742fc37627e40537`  
		Last Modified: Fri, 15 May 2020 15:07:41 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3c0b4710d3bfd982a9a2fc845001e73b11043e83f3618713bbc5ed47218462c`  
		Last Modified: Fri, 15 May 2020 15:07:40 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79fb2b388016d9ef524926aa6e5510ffe2d6643a57cd4e09b991ca90ee2072e`  
		Last Modified: Fri, 15 May 2020 15:09:00 GMT  
		Size: 12.5 MB (12454915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30aa6f0dd42392167b786a269124c84e7cb00bc7dfcde4ea31a4d63ed938eae5`  
		Last Modified: Fri, 15 May 2020 15:08:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af9a337c36d9faf17171bac8095de0116c196c8d43d3c8ffd191a6cd3c76d8e`  
		Last Modified: Fri, 15 May 2020 15:09:17 GMT  
		Size: 14.1 MB (14059019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ec85e069109a12ff3539fd6a0da18305c4de7e87a517f19fd22f69d52c4d05`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606f88b4f6085316d9f15f1eb8f44f029df3b9ef1c212ce061b6fb27c69596cd`  
		Last Modified: Fri, 15 May 2020 15:08:57 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845e768a44c508b027ed195329349d126b34299f7984158fdf20556acc37e788`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232824f4bf64490716a966bedba7eac6feea4d604f178d602fc97d4c4c87204a`  
		Last Modified: Fri, 15 May 2020 15:08:56 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d2a14eceb1759254f8986a3f37d6c3fc2115c1ed0fc6fecae0094b56cb8735`  
		Last Modified: Fri, 15 May 2020 16:13:26 GMT  
		Size: 64.4 MB (64439822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:236d7407028fa4e508d439aa0e8ae86a566b895726fe95d72360232602a69105`  
		Last Modified: Fri, 15 May 2020 16:13:13 GMT  
		Size: 2.8 MB (2848763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8633a5b9d982bead149206f6edf6ba53bfac4d103fa2d781dc47582680041f65`  
		Last Modified: Fri, 15 May 2020 16:13:10 GMT  
		Size: 575.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4820551e47bb3ee07365f44ac5b0bc1d5c1f20575a6de30f402c91d7115d7f6c`  
		Last Modified: Fri, 15 May 2020 16:13:09 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a8e3703db6228225b71d7787cb821efad10f58a429d5b6c61857b99535d68f`  
		Last Modified: Fri, 15 May 2020 16:13:10 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf4d3ec4c337c08e2f04d313efcb0bf68751d9d07db4cc27c18494a79cc207c`  
		Last Modified: Fri, 15 May 2020 16:13:24 GMT  
		Size: 40.9 MB (40931742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable` - linux; arm variant v5

```console
$ docker pull mediawiki@sha256:6ef90891668c07f83007fad2d70e1f6cd6c43bfcb17ad7cc98bbd6c4734bf063
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.7 MB (231663676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80523e7fc3b2f6883baafa07eaabfde0098fb7f6e209b23db2320aba7d1d32c9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 14 May 2020 22:38:03 GMT
ADD file:cbd01ff8d2e40a25bcdb13dc19ffe124c2927b491997dc1c57d4f2c2a308e279 in / 
# Thu, 14 May 2020 22:38:05 GMT
CMD ["bash"]
# Thu, 14 May 2020 22:53:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 14 May 2020 22:53:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 14 May 2020 22:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 22:54:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 May 2020 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 May 2020 22:58:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 14 May 2020 22:58:33 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 14 May 2020 22:58:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 14 May 2020 22:58:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 14 May 2020 22:59:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 14 May 2020 22:59:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 14 May 2020 22:59:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 May 2020 22:59:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 May 2020 23:16:47 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 14 May 2020 23:16:48 GMT
ENV PHP_VERSION=7.3.18
# Thu, 14 May 2020 23:16:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Thu, 14 May 2020 23:16:50 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Thu, 14 May 2020 23:17:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 14 May 2020 23:17:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 23:20:24 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 23:20:29 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 14 May 2020 23:20:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 23:20:31 GMT
STOPSIGNAL SIGWINCH
# Thu, 14 May 2020 23:20:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 14 May 2020 23:20:33 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 23:20:34 GMT
EXPOSE 80
# Thu, 14 May 2020 23:20:35 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 01:46:23 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:48:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 01:48:18 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 01:48:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 01:48:23 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 01:48:24 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 01:48:25 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 01:48:27 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 01:48:28 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 01:48:47 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:24d81022117207b0239d8a8023ca1724b7dde38cb08ce5b9199f59d475d1e600`  
		Last Modified: Thu, 14 May 2020 22:46:51 GMT  
		Size: 24.8 MB (24838470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a42299ddedd5cfd647260b922cf5b0d778940c409129a7054e269c1035bbcbce`  
		Last Modified: Fri, 15 May 2020 00:32:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c018702f98470e8a3438b1cabef55f7cfdb35054aa4f70d669147282f60504d3`  
		Last Modified: Fri, 15 May 2020 00:32:27 GMT  
		Size: 58.8 MB (58799623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605152dc8022c86f5eea93fc446938868856622fc0cdc23b84e7a3a88acaff98`  
		Last Modified: Fri, 15 May 2020 00:32:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:880c410be3fca2cb9173a7372bdb74f92c24cf14880e071cbecd7a621f6d6be3`  
		Last Modified: Fri, 15 May 2020 00:32:57 GMT  
		Size: 18.0 MB (18024813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5117285f0e73747608f4f0e88147a02bb83267a8c3e7ed8caf536d462bc9634`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3290ea8f06dabe7879ffdcb510f0aed946069a1cbe47d29165074733a60c0e5`  
		Last Modified: Fri, 15 May 2020 00:32:49 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651d4b2e219c22e4556ae6b91b43c8fa3015b952189897ed5f4050faff7adc57`  
		Last Modified: Fri, 15 May 2020 00:34:25 GMT  
		Size: 12.5 MB (12453066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77956b846553f8a18b4aad33de1e52e4cd7a6d43477e54561c8d6656f36ba194`  
		Last Modified: Fri, 15 May 2020 00:34:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9465c0242e4217e7a1c41b0782d633a3ce75e5013e456e288a972cce1f0ac14`  
		Last Modified: Fri, 15 May 2020 00:34:23 GMT  
		Size: 13.1 MB (13073912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea20311112e0d260a80646a73d2d4caa8f67976bc5560d9f2f08d9916d48278`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 2.2 KB (2228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e38d64713f6a75a47fafa5e05c780455f367744a0dc6a0afbd47dadc7302ff53`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef83e0d9c5f54cf179d1c2408b0003012b1b4158c15b1cc30531d9753ae7abe1`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c868686b2b57194f4b983dc554dd48f424894a9f6fc09d6247c5f4440d0e68bb`  
		Last Modified: Fri, 15 May 2020 00:34:18 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a5cf53aa89098463346fff882e09c58d7fd9141761ebed3effb61812dd6eac`  
		Last Modified: Fri, 15 May 2020 01:54:31 GMT  
		Size: 60.8 MB (60766605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae80ee1b272d3a549d3dd81531120d8527cd4dbde708005ffc001cf5de2ae97e`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 2.8 MB (2767806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8807c15fe77b8c2b2ec3bb36d38407d30a94142edfafce9d40832a80d7af9a46`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 589.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:165aa15a93e8e5b94b1efc9881a1c56d7c8fb3a1b5c40c2897fc86cfafa2b483`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4c546f84eb62fb9c3a674ac306012ac81735450e45f5d49c6a4e361925f96d`  
		Last Modified: Fri, 15 May 2020 01:54:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea2a9eb4e1831052ec170cf68df7ec7183158c2fe0aa441d9e15878b56f03fb`  
		Last Modified: Fri, 15 May 2020 01:54:30 GMT  
		Size: 40.9 MB (40932734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:cb6ef0227eacbaf8adebfaf0476cad0286cc023280381ce2ca0fb5ffb819ed24
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.2 MB (225218401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f7db6f03bb23cbbe7debb0714273ece2d6b5881708726101cdb566b0834770`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 01:00:06 GMT
ADD file:e3f9a454eccb40b4d7bf1dcc17ec29589a007ac67545d1cb5b6fa213c872c8f2 in / 
# Fri, 15 May 2020 01:00:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:42:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 04:42:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 04:42:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:42:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 04:42:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 04:46:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 04:46:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 04:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 04:46:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 04:46:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 04:46:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 04:46:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 04:46:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 05:01:31 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 05:01:32 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 05:01:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 05:01:34 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 05:01:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 05:01:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 05:04:44 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:47 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 05:04:49 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 05:04:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 05:04:51 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 05:04:51 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 05:04:52 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 05:04:53 GMT
EXPOSE 80
# Fri, 15 May 2020 05:04:54 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 07:34:13 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 07:35:51 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 07:35:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 07:35:55 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 07:35:56 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 07:35:57 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 07:35:57 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 07:35:58 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 07:36:20 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:e41e28500352be59188c3d871a4b5a3f594350b860a9a36ed5808a35920bdae4`  
		Last Modified: Fri, 15 May 2020 01:11:21 GMT  
		Size: 22.7 MB (22705925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9280666064bffcca221d0080298d7943accb5508c37cb14ad2d1727db9ffea8`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8763bc41333e3706105b5f3a46f380db66d2e4e94e99b24e8f686d75405b9cc6`  
		Last Modified: Fri, 15 May 2020 06:05:46 GMT  
		Size: 59.5 MB (59501734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b477d76b007babd3a7aa5458e4e9eb6f16fa46331b293025b6c801bce5a4dd2`  
		Last Modified: Fri, 15 May 2020 06:05:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2730bbece625baddb8e54c6917bcd55aa8926e38537eebefe173bddd456293c`  
		Last Modified: Fri, 15 May 2020 06:06:19 GMT  
		Size: 17.5 MB (17481982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dfbc2496f1c671afd07962dbd920e8f54d00eca301035f6c8fc470b771082e`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caf8b716a60c09a45fe9376381ec37239bd96abe3f46868265a4ca11911c394`  
		Last Modified: Fri, 15 May 2020 06:06:13 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2938e621459f55a8bead228570f7ad0f7f06671d3261b2d6d78eca4caaefc20e`  
		Last Modified: Fri, 15 May 2020 06:08:00 GMT  
		Size: 12.5 MB (12453083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec53a887462bb7b82d74f19073590522ce9ba29e9ea928e31d218e6261016e0`  
		Last Modified: Fri, 15 May 2020 06:07:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0f40794844f49b5960f331bd0929aa1e88233edeabd5a44e9aca1e4e8a724d`  
		Last Modified: Fri, 15 May 2020 06:07:59 GMT  
		Size: 12.4 MB (12370806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac5f0d41f04b86d527452536d2d9bc4009483bc2338c77d984c4ea52c0c710d`  
		Last Modified: Fri, 15 May 2020 06:07:55 GMT  
		Size: 2.2 KB (2227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f668c907a8577f1ef10583437ae78b4bd2113faf23421990f408299a814de30`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b645fbaa2410002cae358e403d3a1b43df9830df618afa35731f27a3850000`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fd081f06ffde760d6f3b50d5225b212466a3b52e47cb3876798a4ef8fd1f75`  
		Last Modified: Fri, 15 May 2020 06:07:54 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8081be2e26e7116795496458ee38a8cded038b68aaf1f6800099fe5c8be51b9`  
		Last Modified: Fri, 15 May 2020 07:40:51 GMT  
		Size: 57.1 MB (57061226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1094fa30f94d21e1ebc451bb84f1cf4206d8d30be046eaa6dfbd7635a5e15044`  
		Last Modified: Fri, 15 May 2020 07:40:33 GMT  
		Size: 2.7 MB (2704244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e697dcb512362cb5881d15c4c66a197c366bbb47b359c87f2841b333100da952`  
		Last Modified: Fri, 15 May 2020 07:40:32 GMT  
		Size: 590.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238c0ef2f57091402a22b91e128a8585792c132816512ffb0c5e515324a56bc5`  
		Last Modified: Fri, 15 May 2020 07:40:32 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a072cc991f71c06383542e9830cc1cb4671b648d50b22afb1b30d1a2007d41fa`  
		Last Modified: Fri, 15 May 2020 07:40:31 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e53a15059b37524232bf4608f46cf2e3c6d148da21d5a48b6c24ca4aed522e8`  
		Last Modified: Fri, 15 May 2020 07:40:58 GMT  
		Size: 40.9 MB (40932759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:b1ad8500fb35495bf117bc219bed8f1be657b08385c56f9b8e08ac3c34feac95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.0 MB (246967619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09f968f66621280d113ebe8ac024f2438ec655038b74a5fdcb7bdcdcb0fbda45`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 12:44:06 GMT
ADD file:b305c1792102142f183d3084026f0fc6be3ddf8d1959b32f0a5d22d35eebcd15 in / 
# Fri, 15 May 2020 12:44:07 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:43:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 14:43:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 14:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:43:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 14:43:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 14:48:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 14:48:24 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 14:48:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 14:48:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 14:48:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 14:48:49 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 14:48:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 14:48:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 15:07:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 15:07:09 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 15:07:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 15:07:10 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 15:07:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 15:07:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 15:10:38 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:41 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 15:10:42 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 15:10:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 15:10:44 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 15:10:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 15:10:46 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 15:10:46 GMT
EXPOSE 80
# Fri, 15 May 2020 15:10:47 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 19:46:49 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:48:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 19:48:15 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 19:48:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 19:48:18 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 19:48:19 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 19:48:19 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 19:48:20 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 19:48:21 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 19:48:36 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:8a7e1e68c24e5cac20ef26d29505c58456b561c431f0c683b66d1a0943f40dd4`  
		Last Modified: Fri, 15 May 2020 12:53:36 GMT  
		Size: 25.9 MB (25857195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42061ac2c49d09e73194c334968747b3b19a921d4e9334d5820775aab2296364`  
		Last Modified: Fri, 15 May 2020 16:14:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc62fa730b42fee32600d030e8a9ed9c17a6485bcf657bc0d677c3c8b4f1b97f`  
		Last Modified: Fri, 15 May 2020 16:14:52 GMT  
		Size: 70.3 MB (70335430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409a141b13978205b5c0b271cd4de0eb119f9da7b2b9a45d298a449fa6a60126`  
		Last Modified: Fri, 15 May 2020 16:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd5b848325aee6d8c850b775d1e5d458cc078526c0037001de044b901979554`  
		Last Modified: Fri, 15 May 2020 16:15:37 GMT  
		Size: 18.6 MB (18579370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04f5399bda859f607e9c2bcd88e5fb85f411ef85eb7037065cec7a111d8a2b2`  
		Last Modified: Fri, 15 May 2020 16:15:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de3de018ff536eb6704e2e73fd598164f712a238926b28b0e63ab8377c8dd7`  
		Last Modified: Fri, 15 May 2020 16:15:31 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae3de17dd48c732d21fd24f161790248745a1f9f5343ca11b2b43c46e105ea5`  
		Last Modified: Fri, 15 May 2020 16:17:15 GMT  
		Size: 12.5 MB (12453774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb6370bcc1b22f91bc8e213c5b1a4b772d0344be0e7bb9221e63b67db1a142b`  
		Last Modified: Fri, 15 May 2020 16:17:12 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9312f5ef6faa9b465032a4a48145dbd87fe48546ab4b8888738098c00e9f1ad3`  
		Last Modified: Fri, 15 May 2020 16:17:15 GMT  
		Size: 13.7 MB (13744535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46c631ec2f0346fc26c53da3692591b7b0debae99b1a15c5534b41b5ba3b239`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b694d004d03fc5a193f48261b7427b006bf62d5e961a72e73f41ee22d13486d`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6c5ca8de4c593238fbedb6cd4958d9de263b56c9c74734d0155ff1096acaf5`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 210.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0641e65be1657f4646febd47c17faf35740796ac356e2e26a487b5387ea8a937`  
		Last Modified: Fri, 15 May 2020 16:17:11 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5d46d3d03a9f3c6f1f266236a9de585cfff43f73b8d8a1e8d35dd31f3d7d681`  
		Last Modified: Fri, 15 May 2020 19:54:12 GMT  
		Size: 62.2 MB (62238680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a789a163be1e82fb5c0bea8cbebc15041095c08e469b493e190d1e08549d9f3`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 2.8 MB (2819336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e98349c303c7d0b2146568c695df1c147d413be75c4f768c0e85a4fdfe1222e`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d503ef15664e43f308e3bd8a34106f553eb9eba97021263c5ad3cd0372732e3b`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a819fc78ba92cfdb40deb661f60ec2a14ccc1cb8100de733b0fc5e4f6d0c5dd`  
		Last Modified: Fri, 15 May 2020 19:53:55 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bf8389f93f7e9c79bcb56ef17776a68d219e0c43085b8de81217e59f8cfe24`  
		Last Modified: Fri, 15 May 2020 19:54:12 GMT  
		Size: 40.9 MB (40932669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable` - linux; 386

```console
$ docker pull mediawiki@sha256:332189a321378b5bfa8dec506debb9858bb1ce25fece88eef6e8d4b2dfc93045
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.1 MB (265080182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdf89f7d308e111eba6cd152f622205cd4efa33523feb1af181b1c97fd1e5f5c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 15 May 2020 07:07:55 GMT
ADD file:0c3b44c83914e95e4604999a86af05023cdd2b2f795e71d737e428fae4a7e0ac in / 
# Fri, 15 May 2020 07:07:56 GMT
CMD ["bash"]
# Fri, 15 May 2020 11:51:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 15 May 2020 11:51:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 15 May 2020 11:52:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 11:52:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 May 2020 11:52:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 15 May 2020 11:59:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 15 May 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 15 May 2020 11:59:43 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 15 May 2020 11:59:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 15 May 2020 11:59:45 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 May 2020 11:59:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 May 2020 12:27:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_VERSION=7.3.18
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Fri, 15 May 2020 12:27:11 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Fri, 15 May 2020 12:27:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 15 May 2020 12:27:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 12:31:13 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:14 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 12:31:15 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 15 May 2020 12:31:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 12:31:15 GMT
STOPSIGNAL SIGWINCH
# Fri, 15 May 2020 12:31:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 15 May 2020 12:31:16 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 12:31:16 GMT
EXPOSE 80
# Fri, 15 May 2020 12:31:16 GMT
CMD ["apache2-foreground"]
# Fri, 15 May 2020 15:38:31 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:39:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 15:40:00 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Fri, 15 May 2020 15:40:01 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 15 May 2020 15:40:02 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Fri, 15 May 2020 15:40:02 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Fri, 15 May 2020 15:40:03 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Fri, 15 May 2020 15:40:15 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:a5695130085a13212b02bf2645a52af5b41dd13e6dc9b29e2d7f357e1525aa48`  
		Last Modified: Fri, 15 May 2020 07:18:14 GMT  
		Size: 27.8 MB (27754922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89d28cd610c05ce76582dbe2667f63e5d6aed254763805cf6938e0a88c28e2`  
		Last Modified: Fri, 15 May 2020 14:30:09 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b8e0eef637c7ebea12f7ec2ea59d6f27711c62690cc7bfca8fbadc5234199b`  
		Last Modified: Fri, 15 May 2020 14:30:49 GMT  
		Size: 81.2 MB (81198662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6611120af4ba82b997d65abf03da25fae06fd0897bc7618d4769640aa2a126df`  
		Last Modified: Fri, 15 May 2020 14:30:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1bf16ca0c76e7067ff0ea6ba2d4f542654b7f161bf45ad6dbab323453ba39d`  
		Last Modified: Fri, 15 May 2020 14:31:22 GMT  
		Size: 19.1 MB (19112829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b0d96f987afef1c5cb6e7ee1bd11903a797a9e8061592b6ca1780cf655a8de`  
		Last Modified: Fri, 15 May 2020 14:31:10 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c952831376c8e30ddfce88236562fb74896243ba6210bfafd16cc6ccb30d98`  
		Last Modified: Fri, 15 May 2020 14:31:11 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1f71bc06b5ba65a360df23e6baed84cf6a160b954839ade5fb135a184dd24f`  
		Last Modified: Fri, 15 May 2020 14:33:13 GMT  
		Size: 12.5 MB (12454242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ba2fc11a09f1683bd8774c9257aebf492a8a5012970c1f9a1bd0ca35edc3b0`  
		Last Modified: Fri, 15 May 2020 14:33:09 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74a16114860a4d9f5b31e4c56097ff316e09ee0a1c2e90786f3897bd9f8fdd8`  
		Last Modified: Fri, 15 May 2020 14:33:13 GMT  
		Size: 14.4 MB (14375467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247829d9036e677667bd1c3161c7315e639cc0d45116994d134b130d591ec272`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f71c9bd38dca215fe8eaa7397a213a4be8ab9875edbf590ffeacb3e2c4cfa27`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c911d28b575600b8e73c4aa3e85eaaa209727dd18042dc8ddbd2b4fca3b33dc`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed82ab66a540f597ce5ca06a395af6ec5fdcc863f663dc058db62daf9c78f090`  
		Last Modified: Fri, 15 May 2020 14:33:08 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4109a070655fcc0c1debc1ee41d7ad694a65ee44f682c056b1c54980ffb66973`  
		Last Modified: Fri, 15 May 2020 15:43:50 GMT  
		Size: 66.4 MB (66394508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27b117c4639d08d7aeb286c29b2848c3b983598e0ae07395ab4c80c2c785ed4`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 2.9 MB (2851267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3829f79f51e528e8c68c793caad7bea03e0df15d73e9db6ca0ba3ccf1e9a0f8e`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c514ae942b80c6b7c6c079584aba65bac31d2b773e7507b7d9c829f226b86e91`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d2cb07003bcf2a9df5a93a6034719260d5961e7393349f53e3cf66b21aa523`  
		Last Modified: Fri, 15 May 2020 15:43:27 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b394e7970eb830e1c09319e5841d27d587ca68c518780d6e6dc1ccdb27fd0fd`  
		Last Modified: Fri, 15 May 2020 15:43:48 GMT  
		Size: 40.9 MB (40931786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:aa2aed9f98726d2510e1ebeb5d5c0e130d64989af29b27815f57a29d6321b5fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.3 MB (275283823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9774b50c3e0a56b3bff561f2cf04379af84da0cf2f6a67fcfd53d924da5f0222`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 16 May 2020 17:14:59 GMT
ADD file:b2656a1711bd47585595ae2927cfd4ec00eb903d193583d945b6d60f0a2691bb in / 
# Sat, 16 May 2020 17:15:04 GMT
CMD ["bash"]
# Sat, 16 May 2020 18:53:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 16 May 2020 18:53:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Mon, 18 May 2020 07:41:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 07:41:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 May 2020 07:41:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 May 2020 07:51:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Mon, 18 May 2020 07:51:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Mon, 18 May 2020 07:54:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Mon, 18 May 2020 07:54:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Mon, 18 May 2020 07:54:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Mon, 18 May 2020 07:54:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Mon, 18 May 2020 07:54:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Mon, 18 May 2020 07:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:54:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 May 2020 07:55:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 May 2020 09:03:54 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Mon, 18 May 2020 09:03:57 GMT
ENV PHP_VERSION=7.3.18
# Mon, 18 May 2020 09:04:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.18.tar.xz.asc
# Mon, 18 May 2020 09:04:02 GMT
ENV PHP_SHA256=7b3e2479a8d6fd7666dcdef8aec50d49c4599cc6ee86e48d41724cfd99cc9e58 PHP_MD5=
# Mon, 18 May 2020 09:04:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 18 May 2020 09:04:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Mon, 18 May 2020 09:09:08 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:18 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 May 2020 09:09:24 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Mon, 18 May 2020 09:09:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 May 2020 09:09:32 GMT
STOPSIGNAL SIGWINCH
# Mon, 18 May 2020 09:09:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 18 May 2020 09:09:41 GMT
WORKDIR /var/www/html
# Mon, 18 May 2020 09:09:45 GMT
EXPOSE 80
# Mon, 18 May 2020 09:09:48 GMT
CMD ["apache2-foreground"]
# Mon, 18 May 2020 19:35:00 GMT
RUN set -eux; 		apt-get update; 	apt-get install -y --no-install-recommends 		git 		librsvg2-bin 		imagemagick 		python3 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:36:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libicu-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install apcu-5.1.18; 	docker-php-ext-enable 		apcu 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Mon, 18 May 2020 19:37:05 GMT
RUN set -eux; 	a2enmod rewrite; 	{ 		echo '<Directory /var/www/html>'; 		echo '  RewriteEngine On'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-f'; 		echo '  RewriteCond %{REQUEST_FILENAME} !-d'; 		echo '  RewriteRule ^ %{DOCUMENT_ROOT}/index.php [L]'; 		echo '</Directory>'; 	} > "$APACHE_CONFDIR/conf-available/short-url.conf"; 	a2enconf short-url
# Mon, 18 May 2020 19:37:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 18 May 2020 19:37:35 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Mon, 18 May 2020 19:37:40 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.34
# Mon, 18 May 2020 19:37:43 GMT
ENV MEDIAWIKI_BRANCH=REL1_34
# Mon, 18 May 2020 19:37:51 GMT
ENV MEDIAWIKI_VERSION=1.34.1
# Mon, 18 May 2020 19:37:57 GMT
ENV MEDIAWIKI_SHA512=3a03ac696e2d5300faba0819ba0d876a21798c8dcdc64cc2792c6db0aa81d4feaced8dc133b6ca3e476c770bf51516b0a624cb336784ae3d2b51c8c0aa5987a0
# Mon, 18 May 2020 19:38:38 GMT
RUN set -eux; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	echo "${MEDIAWIKI_SHA512} *mediawiki.tar.gz" | sha512sum -c -; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	rm mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images
```

-	Layers:
	-	`sha256:034d508ed7647e7139951a435acc95e0124f50c984670d0e53b4f5ba25cf6ed1`  
		Last Modified: Sat, 16 May 2020 18:31:49 GMT  
		Size: 30.5 MB (30524456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a07ac0f385b5553b02726ba8115299da7558e011e6e9721cb9d0603a4813fcf`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be8555f343dcf20b8c2e70f8252e8f2a13a3ae778af6bf4beef48543623ae15`  
		Last Modified: Mon, 18 May 2020 12:11:07 GMT  
		Size: 82.3 MB (82260584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b8ff09f6d8c9fc7ddb3e73ee445eaebca761911a3a9b4dc2720115593a8bdd`  
		Last Modified: Mon, 18 May 2020 12:09:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cb70d525c126bfedd25f50052313a5e902b05de96b38282b8de81d390ae6b6`  
		Last Modified: Mon, 18 May 2020 12:12:20 GMT  
		Size: 19.8 MB (19813054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a601400cd3f9457b1f6e7ad6acc7fb1833370c8879525fe5588e2e226c467fc`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5627d3d5a6729f6e3bd9bf3ba7c6a89b4bff9d2e6b5edf9ba9abaf133f579d`  
		Last Modified: Mon, 18 May 2020 12:11:59 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5778da4b9e5d7a88f35ba1be2447f4f549ba69a64e3d51f25a3d12ffcd3cb2`  
		Last Modified: Mon, 18 May 2020 12:18:41 GMT  
		Size: 12.5 MB (12455153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c71128df22a3960c05cabb8404ffb23bc6a97a69eceecf88249d546ec4b569`  
		Last Modified: Mon, 18 May 2020 12:18:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe189a8a7aa4a630396336b029b1c309e64143334b9269b1fde2ea84d02a64a7`  
		Last Modified: Mon, 18 May 2020 12:18:44 GMT  
		Size: 15.1 MB (15099913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f65c89f9f877a51558fb3fce1bb2c07546baec1d107e4bba266b0f0ce71a566`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 2.2 KB (2234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:504d05192abd7dd43e3bf43ec49a93d38dd7cf9766ac7b79de11cfea30ee9d96`  
		Last Modified: Mon, 18 May 2020 12:18:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104c16784d2476249f104fed21df2bb71e7381dc70e23ff42ad529bf5194b39b`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93db3a5ecb93bdf1621a60e23c4fccf40972b0a0a9cf3289348c920fe37ae677`  
		Last Modified: Mon, 18 May 2020 12:18:34 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7c05be6c020e5a185c9e6238c470df50b8aecf5b693efef9f93894f7c51d72`  
		Last Modified: Mon, 18 May 2020 20:01:06 GMT  
		Size: 71.3 MB (71259919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d066ae6d7c04158054703b1090b60c538d06c67c5e507f6251edd00f34b40e4`  
		Last Modified: Mon, 18 May 2020 19:58:43 GMT  
		Size: 2.9 MB (2931556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593ee04cfb1211afda04063f7fb27a91b6a9464b71d507a0fe4c60be6efd3b81`  
		Last Modified: Mon, 18 May 2020 19:58:41 GMT  
		Size: 581.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38433421ca9b924ec74833c35c458d15dfd4840146a3d9e8774991067a149ec`  
		Last Modified: Mon, 18 May 2020 19:58:40 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdbfaa842585c91095d27c11c54f50df89493a214aae3e47f4fdcb7ceb46601`  
		Last Modified: Mon, 18 May 2020 19:58:41 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bcb826d084e75a26f21ccce8d07eba5a298e01e61c1c573bfd10737d07a193b`  
		Last Modified: Mon, 18 May 2020 20:00:48 GMT  
		Size: 40.9 MB (40932529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
