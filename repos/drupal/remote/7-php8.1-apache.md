## `drupal:7-php8.1-apache`

```console
$ docker pull drupal@sha256:37320dc01b66388377fa37f9d41f1a84ec42c45019fae9d059840bae23aa1831
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

### `drupal:7-php8.1-apache` - linux; amd64

```console
$ docker pull drupal@sha256:73daa10550d5939a9d48347743896e361655ba5a36e007900d4d4507ae948b05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.7 MB (182669654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91e9eedc1532225f3862a8b310b41c3766ba8aa9f324ab98e4617a495105cd29`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:44 GMT
ADD file:209589a8bdb5a3788ee42ecdbccbbb561835dab96b0d8286bb5a2229d2f41be7 in / 
# Thu, 27 Jul 2023 23:24:45 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 10:58:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 10:58:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 10:58:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 10:58:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 10:58:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 11:02:25 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 11:02:25 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 11:02:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 11:02:33 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 11:02:34 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 11:02:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 11:02:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 11:02:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 12:25:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 04 Aug 2023 22:15:32 GMT
ENV PHP_VERSION=8.1.22
# Fri, 04 Aug 2023 22:15:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Fri, 04 Aug 2023 22:15:32 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Fri, 04 Aug 2023 22:15:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Aug 2023 22:15:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:19:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Aug 2023 22:19:06 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:19:07 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Aug 2023 22:19:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Aug 2023 22:19:07 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Aug 2023 22:19:07 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:19:07 GMT
WORKDIR /var/www/html
# Fri, 04 Aug 2023 22:19:07 GMT
EXPOSE 80
# Fri, 04 Aug 2023 22:19:07 GMT
CMD ["apache2-foreground"]
# Fri, 04 Aug 2023 23:45:05 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 04 Aug 2023 23:45:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 04 Aug 2023 23:55:51 GMT
ENV DRUPAL_VERSION=7.98
# Fri, 04 Aug 2023 23:55:51 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Fri, 04 Aug 2023 23:55:52 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:648e0aadf75ac2ef63c5390adc6dc14fde37a5ad88c2870ea604df0a9c0eb4e5`  
		Last Modified: Thu, 27 Jul 2023 23:29:26 GMT  
		Size: 29.1 MB (29124532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318af44fe1855432fb2ca0b6e30af6ccf6237eef18b244e8629567adaef85f6f`  
		Last Modified: Fri, 28 Jul 2023 13:44:54 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9eb75e2f2e68f3c9cdebb7f3abd41a83909ad1e3fe3001c563020f460daa0d`  
		Last Modified: Fri, 28 Jul 2023 13:45:09 GMT  
		Size: 104.3 MB (104340589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6a1589be26232fc35f64f3e7f899c1fc17342b33a8f6f10dad5ebd0bb77969`  
		Last Modified: Fri, 28 Jul 2023 13:44:54 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b9d509db518c3d801c2cbf38d0d84d9a0a95be954203a554275480fa5281fd`  
		Last Modified: Fri, 28 Jul 2023 13:45:36 GMT  
		Size: 20.3 MB (20303148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b069ee18a831a32f9f51d36b8bbdf205c6bdbe09efdd19e694869df96a6a09`  
		Last Modified: Fri, 28 Jul 2023 13:45:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc306e44a7c856f4289a217b8a9dd9255969befe37f8520dc73d8690713edacf`  
		Last Modified: Fri, 28 Jul 2023 13:45:33 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a886a16c1e6a8fbe0ec3d11c7dace76434894aea072364afd2ef466fd46bffa9`  
		Last Modified: Fri, 04 Aug 2023 23:23:02 GMT  
		Size: 12.1 MB (12141436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d100e7e4373eb5ab7968bbadf6b99ea18bfe8558f399a0da1f65100ebdc09e93`  
		Last Modified: Fri, 04 Aug 2023 23:22:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5fbf5d89a24faf8ee193cc20080fd86047fe6d4ead84168da06a77104c388d`  
		Last Modified: Fri, 04 Aug 2023 23:23:01 GMT  
		Size: 11.1 MB (11145456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f724ff2adb4f70ee96669c282c2aa4040302395f0bb617a4845de8be2dbb99`  
		Last Modified: Fri, 04 Aug 2023 23:22:59 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2eb93e1f1dd5a9da3e6a7612743f97914f9e856ef13db41f6c593ff65f28ba`  
		Last Modified: Fri, 04 Aug 2023 23:22:59 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c8eb1378c37eb8a95dd84beb22244985f3d7693f553fa1dd0b388c0c2a8a85`  
		Last Modified: Fri, 04 Aug 2023 23:22:59 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14e2c3f05010625c613cb56684b141a280fdc9202d0b0d01ee44d79c69bea70`  
		Last Modified: Fri, 04 Aug 2023 23:59:32 GMT  
		Size: 2.2 MB (2197812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26c85477e4939b85e26cae245029bd0851890587f98a2f70c9171a71415132b`  
		Last Modified: Fri, 04 Aug 2023 23:59:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338709604a9fdb0623b715d21e965c642f7bc3196f56d09eef06d4d940276cf1`  
		Last Modified: Sat, 05 Aug 2023 00:08:05 GMT  
		Size: 3.4 MB (3410785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache` - linux; arm variant v5

```console
$ docker pull drupal@sha256:37bec56935043b93aba00671c6c55a7843b18ee59d8cc26965e957475824d78d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155945981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed0bc8d58d8e3f29d6610a6946cd4e9db5cbf86cacaba5378e40537196b789ab`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:29 GMT
ADD file:53cf36eb7b72a7e970f4b18af1589402b2900f12e30820cdeccc8bb0c166df80 in / 
# Thu, 27 Jul 2023 23:48:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 08:31:18 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 08:31:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 08:31:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 08:31:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 08:31:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 08:34:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 08:34:41 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 08:34:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 08:34:55 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 08:34:56 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 08:34:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 08:34:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 08:34:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 09:50:22 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 04 Aug 2023 22:25:50 GMT
ENV PHP_VERSION=8.1.22
# Fri, 04 Aug 2023 22:25:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Fri, 04 Aug 2023 22:25:51 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Fri, 04 Aug 2023 22:26:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Aug 2023 22:26:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:30:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Aug 2023 22:30:22 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:30:23 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Aug 2023 22:30:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Aug 2023 22:30:23 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Aug 2023 22:30:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:30:23 GMT
WORKDIR /var/www/html
# Fri, 04 Aug 2023 22:30:23 GMT
EXPOSE 80
# Fri, 04 Aug 2023 22:30:24 GMT
CMD ["apache2-foreground"]
# Sat, 05 Aug 2023 00:08:23 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 05 Aug 2023 00:08:23 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 05 Aug 2023 00:08:23 GMT
ENV DRUPAL_VERSION=7.98
# Sat, 05 Aug 2023 00:08:23 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Sat, 05 Aug 2023 00:08:25 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:2bd6dfc5281e13a0ca9fb8d9238ac9f14a0de04489913030c8e33b9398b4a4af`  
		Last Modified: Thu, 27 Jul 2023 23:51:28 GMT  
		Size: 27.0 MB (26983508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43634693dc45545c293fda492eb4f141f2b087433a414fed71a8c2998c94abc0`  
		Last Modified: Fri, 28 Jul 2023 10:50:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb29dd2916110f9f66685596a6f36d103c85cd94872346b64856e09acdcfa231`  
		Last Modified: Fri, 28 Jul 2023 10:51:15 GMT  
		Size: 82.0 MB (82026710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82a300dcb955c723d0598ac4b79be08dd1e67007d1c247b744b49e036d3eddc`  
		Last Modified: Fri, 28 Jul 2023 10:50:58 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd5d3a845c53c271a52c66ffa4eb90ca53d7a84f9ab677b1168ab16ebc11514`  
		Last Modified: Fri, 28 Jul 2023 10:51:47 GMT  
		Size: 19.6 MB (19607888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1e6710bfde9f7c78e80d6e1ecba2a7ce6b895ead420acf2bc013605ab54a1f`  
		Last Modified: Fri, 28 Jul 2023 10:51:42 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e5bb634477bbca05ea901034c7d6dd2b5909717e6d0d4788ef4781c4c4a654`  
		Last Modified: Fri, 28 Jul 2023 10:51:42 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4cfb4b617def143321ad5ea91b6e7e999e4f519c6979470a75e9b4b8b134b6`  
		Last Modified: Fri, 04 Aug 2023 23:02:27 GMT  
		Size: 12.1 MB (12139438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7250435e87863ddbad54670913e664b68334acb2739cf07016d6f9518ccf2c2`  
		Last Modified: Fri, 04 Aug 2023 23:02:24 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcb05396b571239ab16b7850f058248389b5518affd246a2ed88d3ccd033a49`  
		Last Modified: Fri, 04 Aug 2023 23:02:27 GMT  
		Size: 10.1 MB (10106877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8f6e9da3024742622bc8d2cff8e38894070c73ff1589fd6a4a1e6b92ead6ae`  
		Last Modified: Fri, 04 Aug 2023 23:02:24 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a91991f2d05f7b3bfa9949f265270761f076c0e227c0c941a52f5d06fdca0af`  
		Last Modified: Fri, 04 Aug 2023 23:02:24 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f79ebdb9d94a09095936359b5a5d24cc9f71f0ace8780c87f9ad945ea29280`  
		Last Modified: Fri, 04 Aug 2023 23:02:24 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bd430908e6b2c2bdd8fde0e4fa554f7e8e2293e4af4122eda0a4bd8fdd08c9`  
		Last Modified: Sat, 05 Aug 2023 00:10:57 GMT  
		Size: 1.7 MB (1664884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ab50f1d64b82f24628378d03b195bceb568cc5f96143e55f3778f8472c7817`  
		Last Modified: Sat, 05 Aug 2023 00:10:56 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d60502cea1842c8dd3d8343c2af1c56399aae732dc4f0e75b7aea092c7f968`  
		Last Modified: Sat, 05 Aug 2023 00:10:57 GMT  
		Size: 3.4 MB (3410781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache` - linux; arm variant v7

```console
$ docker pull drupal@sha256:38c08deec2e596006570de506743d44453220737f8c7096c2348bb17b200eec7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146740013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc5fda2658b45572fd11a496606412967b45ea9cb5a53beb8b3c02d84b8928e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:57:46 GMT
ADD file:b23161e9856801127e0136a920bcf075410ac23de605c82ca91d285b9f35941c in / 
# Thu, 27 Jul 2023 23:57:47 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 04:14:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 04:14:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 04:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 04:14:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 04:14:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 04:17:18 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 04:17:18 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 04:17:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 04:17:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 04:17:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 04:17:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 04:17:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 04:17:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 05:25:24 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 04 Aug 2023 23:12:24 GMT
ENV PHP_VERSION=8.1.22
# Fri, 04 Aug 2023 23:12:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Fri, 04 Aug 2023 23:12:25 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Fri, 04 Aug 2023 23:12:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Aug 2023 23:12:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Aug 2023 23:15:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Aug 2023 23:15:02 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 04 Aug 2023 23:15:02 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Aug 2023 23:15:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Aug 2023 23:15:02 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Aug 2023 23:15:02 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Aug 2023 23:15:03 GMT
WORKDIR /var/www/html
# Fri, 04 Aug 2023 23:15:03 GMT
EXPOSE 80
# Fri, 04 Aug 2023 23:15:03 GMT
CMD ["apache2-foreground"]
# Sat, 05 Aug 2023 00:28:06 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 05 Aug 2023 00:28:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 05 Aug 2023 00:36:23 GMT
ENV DRUPAL_VERSION=7.98
# Sat, 05 Aug 2023 00:36:23 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Sat, 05 Aug 2023 00:36:25 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:bb5b735234291ca6f672f489206ea5b6354d358f7d75a05036bdf84a6858d9f9`  
		Last Modified: Fri, 28 Jul 2023 00:03:11 GMT  
		Size: 24.8 MB (24805329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec008ebecf1d5fd92a5913c050e101aa3e5310c66507826423f082a03d6842a`  
		Last Modified: Fri, 28 Jul 2023 06:31:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe9fcd4dba6ea446dd434cfff4b2ede073967422738a9805bcd41e70be50cb5`  
		Last Modified: Fri, 28 Jul 2023 06:31:33 GMT  
		Size: 76.2 MB (76216888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c3c9eebfa26ad2ed1cb26a786e57a3201cda07ed2942048fd4f91633b8c13e`  
		Last Modified: Fri, 28 Jul 2023 06:31:14 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5898036522058e2c9e91104d190eecb2a0a3520370db5479d1cbf578bfde61`  
		Last Modified: Fri, 28 Jul 2023 06:32:00 GMT  
		Size: 19.0 MB (19044677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56576b92476424c16fdbfbf005931616549a49daa031a44d75a6b43fc03d051f`  
		Last Modified: Fri, 28 Jul 2023 06:31:57 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d91da2cf4dbddf6db37a8f0998410f487458b25c60c19442643a4b8a233e201`  
		Last Modified: Fri, 28 Jul 2023 06:31:57 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79bc5c4e5ce2603a9e988d526d5dc7253b55f425e43bfca30fdfacab2b70b54`  
		Last Modified: Sat, 05 Aug 2023 00:07:34 GMT  
		Size: 12.1 MB (12139357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c46e161e586f8f8d54266fa7f37390793639a8a56dd426b72cd578d716895c`  
		Last Modified: Sat, 05 Aug 2023 00:07:31 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12462a04e34678797bf44d9dfa47a284fba9ee096a3ecd50aa4a1dc2a02ab91b`  
		Last Modified: Sat, 05 Aug 2023 00:07:33 GMT  
		Size: 9.6 MB (9569232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ebe543696128b56a07eff5f9349b142a55a444ed24401cf9270f97df96562c`  
		Last Modified: Sat, 05 Aug 2023 00:07:31 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96dbac9f39a0acbdd82290106ac7f99743b2a9f8d4e9f58cb05bdcdc4fcd9a6f`  
		Last Modified: Sat, 05 Aug 2023 00:07:31 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de71979628f727155b4d4160a2be783a9a54595992326b46314415f59b782f65`  
		Last Modified: Sat, 05 Aug 2023 00:07:31 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7658651889714f29fb7c94f2819a8996772217cac3fa76084882b05ccf95b7`  
		Last Modified: Sat, 05 Aug 2023 00:39:34 GMT  
		Size: 1.5 MB (1547865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c056eb7874d1af81b695697f6cc4dd8613f660739a1c41a9202c5d5593978faf`  
		Last Modified: Sat, 05 Aug 2023 00:39:33 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92638402ed2321fc85430ba821e0154ca7773124c3630c49853149c0fe842b1f`  
		Last Modified: Sat, 05 Aug 2023 00:48:27 GMT  
		Size: 3.4 MB (3410781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:39f6b160dbd7479b9766614cecfc1a77061b32c78f3f0fc1cc22d5f6f0ffac26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176776582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b799ab2c13ccb030fd065fa740092504768816466df05f49ae4359580f476dc4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:43:00 GMT
ADD file:1de2ba0dc88aa343332814e19adc6b850d08e62c31589fe902b8eb2cb465934e in / 
# Thu, 27 Jul 2023 23:43:00 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 11:16:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 11:16:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 11:16:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 11:16:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 11:16:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 11:20:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 11:20:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 11:20:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 11:20:19 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 11:20:20 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 11:20:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 11:20:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 11:20:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 12:38:21 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 28 Jul 2023 13:04:22 GMT
ENV PHP_VERSION=8.1.21
# Fri, 28 Jul 2023 13:04:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.21.tar.xz.asc
# Fri, 28 Jul 2023 13:04:22 GMT
ENV PHP_SHA256=e634a00b0c6a8cd39e840e9fb30b5227b820b7a9ace95b7b001053c1411c4821
# Fri, 28 Jul 2023 13:04:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 28 Jul 2023 13:04:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Jul 2023 13:07:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Jul 2023 13:07:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 28 Jul 2023 13:07:46 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Jul 2023 13:07:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Jul 2023 13:07:46 GMT
STOPSIGNAL SIGWINCH
# Fri, 28 Jul 2023 13:07:46 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 28 Jul 2023 13:07:46 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 13:07:46 GMT
EXPOSE 80
# Fri, 28 Jul 2023 13:07:46 GMT
CMD ["apache2-foreground"]
# Fri, 28 Jul 2023 20:51:01 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 20:51:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Jul 2023 21:02:46 GMT
ENV DRUPAL_VERSION=7.98
# Fri, 28 Jul 2023 21:02:46 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Fri, 28 Jul 2023 21:02:47 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:90524f7dc01b4ce9b387992acc6cbdbcc2a9ee8c6addfd632429ca06ea18751e`  
		Last Modified: Thu, 27 Jul 2023 23:46:17 GMT  
		Size: 29.2 MB (29157226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8caf6560dfee8e778fccc649da83bc14c208c742ddd3462fe0d11697c98cd3e7`  
		Last Modified: Fri, 28 Jul 2023 13:47:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff9bc0aae4453ed6665099c6d31bd0959613fa486241fbbc414764c9cbf1569`  
		Last Modified: Fri, 28 Jul 2023 13:47:37 GMT  
		Size: 98.1 MB (98110025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ee322441492fcefb9b148e3dd41e4f3764c57506e0cc6ffba91cf2531c34ec`  
		Last Modified: Fri, 28 Jul 2023 13:47:27 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b6b6383c913c3b2453be2c3b6d97730356c03d814617ae4b222978f68ded80`  
		Last Modified: Fri, 28 Jul 2023 13:48:04 GMT  
		Size: 20.3 MB (20304561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98014587705891e3097ccc65ceeac1f58e35e1485feaa113c947b7059400841`  
		Last Modified: Fri, 28 Jul 2023 13:48:02 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714e052e0a815e0f234c7d0e6f3ca725b628f92336360477f0d861baddb38352`  
		Last Modified: Fri, 28 Jul 2023 13:48:02 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53152ccd9f09b0ca4dfdb9a74b0708c167a76bff1a67d24b8b9daabdda22e103`  
		Last Modified: Fri, 28 Jul 2023 13:58:41 GMT  
		Size: 12.2 MB (12193909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb255e0a71da0156ec221d827d78f1cdbfd87dcea0ee58382dbc707fdd3f2c8`  
		Last Modified: Fri, 28 Jul 2023 13:58:38 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4877b60b70439713d642e8fd95b3ea608f74c0339c16fd7c2fb50c818e7ea7`  
		Last Modified: Fri, 28 Jul 2023 13:58:40 GMT  
		Size: 11.1 MB (11139204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f422e810923cef88aa0b0b4cca028cd979bb8862cfa3690bc06f010b34e2f053`  
		Last Modified: Fri, 28 Jul 2023 13:58:38 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbf4bac87d9f3e3e542281c51c7702069a19bc84e6e9d33feccac1863dbc451`  
		Last Modified: Fri, 28 Jul 2023 13:58:38 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c854f9c53806bb73dd542c8172c2e5cd349f7068fc6f5ca7d3c6abe7ba40d780`  
		Last Modified: Fri, 28 Jul 2023 13:58:38 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59512c74cc7ae7a40c187ed03e6380af6c26d67679244f9699adb977274a24c8`  
		Last Modified: Fri, 28 Jul 2023 21:08:46 GMT  
		Size: 2.5 MB (2454976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5197616ebd3629af6e3bbd28c607bf4b204d8eb2cc9fdbb7e76f29053923bc`  
		Last Modified: Fri, 28 Jul 2023 21:08:45 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5dfd5f176f821d97e7c236669a097152d65c8075eea3d9e9390993e8b2e2e8`  
		Last Modified: Fri, 28 Jul 2023 21:19:14 GMT  
		Size: 3.4 MB (3410786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache` - linux; 386

```console
$ docker pull drupal@sha256:b98e07f121d32a48092dce6915c9512e314ac6eb0f7824ccc2716d38e7d15af6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.7 MB (181688498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f47fb7410409465939c0e03fbbafc3a21f7e1dd87ca82ced2058aaff9e7a13`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:38:56 GMT
ADD file:3d6e6f3e900e480a7e060fcaf57313c0f954bf906967a7fa0317567c387cf5aa in / 
# Thu, 27 Jul 2023 23:38:57 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:56:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 03:56:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 03:56:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:56:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 03:56:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 04:02:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 04:02:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 04:03:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 04:03:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 04:03:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 04:03:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 04:03:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 04:03:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 06:20:53 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 28 Jul 2023 07:05:12 GMT
ENV PHP_VERSION=8.1.21
# Fri, 28 Jul 2023 07:05:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.21.tar.xz.asc
# Fri, 28 Jul 2023 07:05:12 GMT
ENV PHP_SHA256=e634a00b0c6a8cd39e840e9fb30b5227b820b7a9ace95b7b001053c1411c4821
# Fri, 28 Jul 2023 07:05:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 28 Jul 2023 07:05:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 28 Jul 2023 07:11:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 28 Jul 2023 07:11:14 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 28 Jul 2023 07:11:15 GMT
RUN docker-php-ext-enable sodium
# Fri, 28 Jul 2023 07:11:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 28 Jul 2023 07:11:15 GMT
STOPSIGNAL SIGWINCH
# Fri, 28 Jul 2023 07:11:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 28 Jul 2023 07:11:15 GMT
WORKDIR /var/www/html
# Fri, 28 Jul 2023 07:11:16 GMT
EXPOSE 80
# Fri, 28 Jul 2023 07:11:16 GMT
CMD ["apache2-foreground"]
# Fri, 28 Jul 2023 21:31:15 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 21:31:15 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 28 Jul 2023 21:46:30 GMT
ENV DRUPAL_VERSION=7.98
# Fri, 28 Jul 2023 21:46:30 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Fri, 28 Jul 2023 21:46:32 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:3a8b0c4b1a83609d978d576be6174f951ff27084d7c9aef91892b60b223a5104`  
		Last Modified: Thu, 27 Jul 2023 23:43:26 GMT  
		Size: 30.1 MB (30141788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76eefc4f044829a4fb54a28aee1ecbdc191c27802c7e44c0f0e1733655606ecc`  
		Last Modified: Fri, 28 Jul 2023 08:27:19 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af44072e615c202c447ce0a3f4eee5b57b458c42da585a8cabc300132320dff6`  
		Last Modified: Fri, 28 Jul 2023 08:27:41 GMT  
		Size: 101.5 MB (101506268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6e4dfe670c503c36a4c3d9e949993d31aae6c5d34769f67d21c90539714c31`  
		Last Modified: Fri, 28 Jul 2023 08:27:19 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5835c7fe46fa74e12b354a2ca46547fee1d2115c6857a8cf59428f26048338e`  
		Last Modified: Fri, 28 Jul 2023 08:28:10 GMT  
		Size: 20.8 MB (20825248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b456e0aaccec57708995d3bf6e46639c9775bf14c0eecef29b03a5fef6cd8757`  
		Last Modified: Fri, 28 Jul 2023 08:28:06 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8993ec4922a29c59b6960c76a489ec7d599641fca32a24de324e5a0a2237727`  
		Last Modified: Fri, 28 Jul 2023 08:28:06 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f0fc973f991638e41e3ca4753f5a0773966d66d167003e8d756cdea7ae695d`  
		Last Modified: Fri, 28 Jul 2023 08:40:18 GMT  
		Size: 12.2 MB (12193462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5b01e30bd40748f08c3410ac52400acbb0a593888ab452fc43ba1357229cfe`  
		Last Modified: Fri, 28 Jul 2023 08:40:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e711643ee7aa4b0d185391f87802c52118f06613e07eed8ce5616e88388a5670`  
		Last Modified: Fri, 28 Jul 2023 08:40:18 GMT  
		Size: 11.4 MB (11355101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8a80d4d5027e63d1bcef66c9af7baa7706408df47e17e4e13e4dd07e30ccf`  
		Last Modified: Fri, 28 Jul 2023 08:40:15 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35b29d889acd08e25f369f65aa9f46e09d6addec79a1ebb8d885ef9da6cf7180`  
		Last Modified: Fri, 28 Jul 2023 08:40:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec6d8ac1cb4a1cac1cb1d4011134ef0d55d27c7685aec7a80d8b411d6c6d0ec`  
		Last Modified: Fri, 28 Jul 2023 08:40:15 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b3b06c3ab1e6003c9d1d1678b4f7c884e64d91bbc3db345cc2b3bb6c745908`  
		Last Modified: Fri, 28 Jul 2023 21:52:56 GMT  
		Size: 2.2 MB (2249964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8580c2931063de39b1f92f8eb7b6dcf49b65c34e72c4570ee03c2a360a6dab2d`  
		Last Modified: Fri, 28 Jul 2023 21:52:55 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd64cf6177bf56e071e4db80bf1c1854d186f58efad9b8da3276c8a618d22532`  
		Last Modified: Fri, 28 Jul 2023 22:05:45 GMT  
		Size: 3.4 MB (3410777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache` - linux; mips64le

```console
$ docker pull drupal@sha256:a21cd7f1db2a829ae99cb618f51030d72c1f503ee81c12e5da70288920e91c00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (157028102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5720bfcd551d113405201402e0e1a4a2f4701f065acb8cfe5c96602b4dc4bf9c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:23 GMT
ADD file:90cbcf9a2aaf48a433b00118dd0821eeb291092da7b7f67ce6a525ce2cba1e3f in / 
# Thu, 27 Jul 2023 23:11:27 GMT
CMD ["bash"]
# Sat, 29 Jul 2023 06:01:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 29 Jul 2023 06:01:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 29 Jul 2023 06:02:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 29 Jul 2023 06:02:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 29 Jul 2023 06:03:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 29 Jul 2023 06:19:40 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 29 Jul 2023 06:19:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 29 Jul 2023 06:20:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 29 Jul 2023 06:20:45 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 29 Jul 2023 06:20:51 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 29 Jul 2023 06:20:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 29 Jul 2023 06:20:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 29 Jul 2023 06:21:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 29 Jul 2023 12:32:45 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 29 Jul 2023 14:33:50 GMT
ENV PHP_VERSION=8.1.21
# Sat, 29 Jul 2023 14:33:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.21.tar.xz.asc
# Sat, 29 Jul 2023 14:33:58 GMT
ENV PHP_SHA256=e634a00b0c6a8cd39e840e9fb30b5227b820b7a9ace95b7b001053c1411c4821
# Sat, 29 Jul 2023 14:34:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 29 Jul 2023 14:34:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 29 Jul 2023 14:50:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 29 Jul 2023 14:50:26 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 29 Jul 2023 14:50:32 GMT
RUN docker-php-ext-enable sodium
# Sat, 29 Jul 2023 14:50:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 29 Jul 2023 14:50:39 GMT
STOPSIGNAL SIGWINCH
# Sat, 29 Jul 2023 14:50:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 29 Jul 2023 14:50:46 GMT
WORKDIR /var/www/html
# Sat, 29 Jul 2023 14:50:49 GMT
EXPOSE 80
# Sat, 29 Jul 2023 14:50:53 GMT
CMD ["apache2-foreground"]
# Sat, 29 Jul 2023 21:17:35 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 29 Jul 2023 21:17:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 29 Jul 2023 21:17:45 GMT
ENV DRUPAL_VERSION=7.98
# Sat, 29 Jul 2023 21:17:48 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Sat, 29 Jul 2023 21:17:58 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:3252778e08fa8eb67ab052ad63281284b5ef1afdc40a36021228133487ab5d52`  
		Last Modified: Thu, 27 Jul 2023 23:22:26 GMT  
		Size: 29.1 MB (29121405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af07b716bf7a574ec3a1df6cf5b176ef70b2874a9d60ea9469132b7fe383e47`  
		Last Modified: Sat, 29 Jul 2023 17:17:03 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e394bb28d5651326ad7cec988e29093b6a8c08db2ba72ccfcb3a48b62ae5b35`  
		Last Modified: Sat, 29 Jul 2023 17:17:59 GMT  
		Size: 80.7 MB (80670282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220eb526892e1170829d762f7a9c4a60a6ffafcf19c1bcc3e9842eb4c7449bdc`  
		Last Modified: Sat, 29 Jul 2023 17:17:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a50e548e00760b9d777989c4c8c514ca1efbf7e4faa04b2d6b1cca64a083ee`  
		Last Modified: Sat, 29 Jul 2023 17:18:48 GMT  
		Size: 20.1 MB (20053811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d5f086dd94ba06f32a048bd50e2a5f73c2540287580ca172d9770d224c7300`  
		Last Modified: Sat, 29 Jul 2023 17:18:30 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae4622cd0a870b2efa59c1047cb0331cc97358773ea5e9ff17e7557c497585b`  
		Last Modified: Sat, 29 Jul 2023 17:18:30 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb9cd16ee6143a20bff455beff2b72361fb330af34c2fef708e58847f83bc555`  
		Last Modified: Sat, 29 Jul 2023 17:37:11 GMT  
		Size: 12.0 MB (11988314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdc570a471ba5127d7e6e702b07c2966f67363ea95a8a4f3db1f6395fb4b034`  
		Last Modified: Sat, 29 Jul 2023 17:37:06 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9dbe8924379519b66dbdc1ccbe9935b2819dbadba7262a3d299e51b322da7e`  
		Last Modified: Sat, 29 Jul 2023 17:37:14 GMT  
		Size: 10.2 MB (10215028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25755e76a25ed02b2190096a0049a9f9770f7883a0460a52f896c8d6ae9884eb`  
		Last Modified: Sat, 29 Jul 2023 17:37:06 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade249a24c1b7adbe9d6386fb4d3697cef7efb6bc28925d3c4eebc1d222ae0e9`  
		Last Modified: Sat, 29 Jul 2023 17:37:06 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5387f5588b3d65abe65b3433e5372117c2fc941cc3597f5927573ebf61391b0`  
		Last Modified: Sat, 29 Jul 2023 17:37:06 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6902b7cd5c9991737259492f040d6cf52c999289b8712c11e8504eb99eb3705d`  
		Last Modified: Sat, 29 Jul 2023 21:35:12 GMT  
		Size: 1.6 MB (1563041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aebb6dda04ec677ae83a57eb8811061eba08b6e830bca0e3dc336cd17c701b7`  
		Last Modified: Sat, 29 Jul 2023 21:35:10 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb416ae79b51fe48762c1d01757b3ee4adf4f33d48c8b3e8c5b792602fe5bb9`  
		Last Modified: Sat, 29 Jul 2023 21:35:14 GMT  
		Size: 3.4 MB (3410427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache` - linux; ppc64le

```console
$ docker pull drupal@sha256:f4aeaee6e392545ecc5547279e598539f69a1532c41155c8768f9678d0285530
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.0 MB (187044444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00dccc9c8e2d5977d48ff5f2a42a82fd1e5814d53ddc86769232eba7eff4398f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:23:01 GMT
ADD file:774a99e5c40757d27c981eb5ad6e03eb72970bb0c54f799eab1442624238ea3e in / 
# Thu, 27 Jul 2023 23:23:03 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 15:45:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 15:45:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 15:46:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 15:46:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 15:46:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 15:51:45 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 15:51:45 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 15:52:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 15:52:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 15:52:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 15:52:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 15:52:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 15:52:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 17:55:53 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 04 Aug 2023 22:32:54 GMT
ENV PHP_VERSION=8.1.22
# Fri, 04 Aug 2023 22:32:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Fri, 04 Aug 2023 22:32:55 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Fri, 04 Aug 2023 22:33:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Aug 2023 22:33:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:38:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Aug 2023 22:38:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:38:25 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Aug 2023 22:38:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Aug 2023 22:38:27 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Aug 2023 22:38:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:38:28 GMT
WORKDIR /var/www/html
# Fri, 04 Aug 2023 22:38:28 GMT
EXPOSE 80
# Fri, 04 Aug 2023 22:38:29 GMT
CMD ["apache2-foreground"]
# Sat, 05 Aug 2023 00:25:41 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 05 Aug 2023 00:25:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 05 Aug 2023 00:47:08 GMT
ENV DRUPAL_VERSION=7.98
# Sat, 05 Aug 2023 00:47:08 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Sat, 05 Aug 2023 00:47:11 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:ad974e0ada84177d519dec70d0d7d9ff6a4f468bc7306425feb8429bc276bd8a`  
		Last Modified: Thu, 27 Jul 2023 23:29:24 GMT  
		Size: 33.1 MB (33119211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73baf1bc3c2c4f849db7df84a0bf32fcb24e8531d299f993f05f1a7604299a39`  
		Last Modified: Fri, 28 Jul 2023 19:29:58 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2235bb37879b53292425b549642e073f60427733b2ce0bd84a0bee6bf8b15b6c`  
		Last Modified: Fri, 28 Jul 2023 19:30:25 GMT  
		Size: 103.3 MB (103306001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522d99b114002fc6058eed334bf93b1e6aab2be6b9fded811f0314eb8c02eaff`  
		Last Modified: Fri, 28 Jul 2023 19:29:58 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782d10f4c9c664f971ef340e3b18a68c814f63583693886fa89cddace6318399`  
		Last Modified: Fri, 28 Jul 2023 19:31:06 GMT  
		Size: 21.5 MB (21488902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac5658e1e2158da838a829adc92fb1da5ab115740aa4e16b41638f36301f37da`  
		Last Modified: Fri, 28 Jul 2023 19:31:01 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7823b7085d9b4d21742ea5277d02301692be96e659cb163b54e94ef4b3a45f3a`  
		Last Modified: Fri, 28 Jul 2023 19:31:01 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac3c5c11192c2d5ae020a1d2b5bdc8b06c5f9fe0d5cc8e8fbf7b5145c0aeae9`  
		Last Modified: Sat, 05 Aug 2023 00:01:22 GMT  
		Size: 12.1 MB (12140907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d209a4b102cefe26c0ed19146754216e44059a76afb7e200135e111ad8b15267`  
		Last Modified: Sat, 05 Aug 2023 00:01:19 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f10b757460a662f07c73828141dbe299292a1a457a7d1308c73848b05627d7`  
		Last Modified: Sat, 05 Aug 2023 00:01:22 GMT  
		Size: 11.5 MB (11521123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dca1a2248271ab4cb64ddf61efe0fd919a55224bf1d56f9b55bd611cdc8a46b`  
		Last Modified: Sat, 05 Aug 2023 00:01:19 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b68ff87e15de77837cdb60fb021ba446133fff7ccff3c8f3ca51d35ee57d83`  
		Last Modified: Sat, 05 Aug 2023 00:01:19 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53959184b0594c539a89908beca09044852d34125459adcea5d04d442638a4fb`  
		Last Modified: Sat, 05 Aug 2023 00:01:19 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd2b7407885d6d12117f37c1c1647cbbb7e0066d0bf81b6cd98ce3826573076`  
		Last Modified: Sat, 05 Aug 2023 00:52:32 GMT  
		Size: 2.1 MB (2051620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488479ad35c699d02798351dce61e58d72ba16a6e61cfc8aac6526bb9c5a6715`  
		Last Modified: Sat, 05 Aug 2023 00:52:31 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd68e4bc862f6e96d6c41d107bca1fc1eb64e7c7c04f04c9d772f86095cb6a2`  
		Last Modified: Sat, 05 Aug 2023 01:09:36 GMT  
		Size: 3.4 MB (3410777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.1-apache` - linux; s390x

```console
$ docker pull drupal@sha256:ffd45d8906984edbc3c21eb1289f54c0d6075f904be771e80de1db6cf0879d97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.9 MB (155884780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6377fd1abd1e2c9e445f31f3f606a1013275932a33c7fa653539b57818600579`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 27 Jul 2023 23:47:11 GMT
ADD file:0a5e1e86b375d60637d0829f77a12085777cf2ca07495b0f6249d8efea84e958 in / 
# Thu, 27 Jul 2023 23:47:13 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 12:58:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 28 Jul 2023 12:58:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 28 Jul 2023 12:58:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 12:58:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 28 Jul 2023 12:58:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 28 Jul 2023 13:01:14 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 28 Jul 2023 13:01:14 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 28 Jul 2023 13:01:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 28 Jul 2023 13:01:23 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 28 Jul 2023 13:01:24 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 28 Jul 2023 13:01:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 13:01:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 28 Jul 2023 13:01:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 28 Jul 2023 14:05:47 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 04 Aug 2023 22:28:43 GMT
ENV PHP_VERSION=8.1.22
# Fri, 04 Aug 2023 22:28:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.22.tar.xz.asc
# Fri, 04 Aug 2023 22:28:43 GMT
ENV PHP_SHA256=9ea4f4cfe775cb5866c057323d6b320f3a6e0adb1be41a068ff7bfec6f83e71d
# Fri, 04 Aug 2023 22:28:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 04 Aug 2023 22:28:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:31:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Aug 2023 22:31:20 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:31:20 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Aug 2023 22:31:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Aug 2023 22:31:20 GMT
STOPSIGNAL SIGWINCH
# Fri, 04 Aug 2023 22:31:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 04 Aug 2023 22:31:21 GMT
WORKDIR /var/www/html
# Fri, 04 Aug 2023 22:31:21 GMT
EXPOSE 80
# Fri, 04 Aug 2023 22:31:21 GMT
CMD ["apache2-foreground"]
# Sat, 05 Aug 2023 00:27:55 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 05 Aug 2023 00:27:55 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 05 Aug 2023 00:39:12 GMT
ENV DRUPAL_VERSION=7.98
# Sat, 05 Aug 2023 00:39:12 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Sat, 05 Aug 2023 00:39:14 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:f4301d25bb1bea85fcc5b364aec84ff58274f714cea191ab22d9b1b1e4f78527`  
		Last Modified: Thu, 27 Jul 2023 23:52:17 GMT  
		Size: 27.5 MB (27489697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505140a8d4e846fbb62f3b3f5c042a1db814660d1b674985aba6b2312dc41747`  
		Last Modified: Fri, 28 Jul 2023 14:58:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf930a3b25a984a929b6b75d17a0301d95966405125f8cb009b2587b31b8bc6`  
		Last Modified: Fri, 28 Jul 2023 14:58:32 GMT  
		Size: 80.8 MB (80803578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c6295803847084254e34eea846cd541acbc968ac9c350c9818e000ddb3d3d0`  
		Last Modified: Fri, 28 Jul 2023 14:58:21 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b133fc86a7d2674c4946377934b924b3658d374622a76cf279d8d3741e2749`  
		Last Modified: Fri, 28 Jul 2023 14:58:50 GMT  
		Size: 20.1 MB (20082317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40aba6cccce8202804cd37d922b4d9e327ef736846e833e4fee63b104c1d748`  
		Last Modified: Fri, 28 Jul 2023 14:58:48 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a45c736687a72bb765e0987d284a31150153d576978b263ad7421d0549c946`  
		Last Modified: Fri, 28 Jul 2023 14:58:48 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c4766d0250084e9cd0c5f074b2e980e687c5b1ab64d567e1598a834dda1528`  
		Last Modified: Fri, 04 Aug 2023 23:21:54 GMT  
		Size: 12.1 MB (12139753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b150e51225ae7e2fb87e14a4c45dcf3218a387c2b77207b55b48e490e5c42cc0`  
		Last Modified: Fri, 04 Aug 2023 23:21:51 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbe856a201a925ef5ccc23eb99566ea1a0eb3735988b8efba7300b41cc36585`  
		Last Modified: Fri, 04 Aug 2023 23:21:53 GMT  
		Size: 10.2 MB (10203902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274db552a69e6f9919fa48d89dd30c3d0e215cc528ba8ba06ede3dd10098b0ec`  
		Last Modified: Fri, 04 Aug 2023 23:21:51 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef266e01af79dc0f9754f181384275e2eab22d22568999832a44af1ad6587b`  
		Last Modified: Fri, 04 Aug 2023 23:21:51 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cbeba0dffa94bbad951e3681c050b94bb8b3d44829d80f68d6b19640929f505`  
		Last Modified: Fri, 04 Aug 2023 23:21:51 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84de0fca04ce76569a3bf46cafc5aefaedc2186966767f1ef7dd76cefb0d9c3e`  
		Last Modified: Sat, 05 Aug 2023 00:43:44 GMT  
		Size: 1.7 MB (1748847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5ac00cb80b56cfec99bf2687323a54fd9f56ce9c4f4cc7b3de50a25abf26a`  
		Last Modified: Sat, 05 Aug 2023 00:43:44 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a682e91563965c5b395cefba8ea054a247a78f2ed349aa84ad89b5a7450b2db`  
		Last Modified: Sat, 05 Aug 2023 00:49:47 GMT  
		Size: 3.4 MB (3410785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
