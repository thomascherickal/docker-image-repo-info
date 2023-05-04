## `drupal:9-apache`

```console
$ docker pull drupal@sha256:42b7f28426778e3324e064c30b34d7e45baad21eb2ae02e337a3379ff908e05d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:9-apache` - linux; amd64

```console
$ docker pull drupal@sha256:86fa4f6cff945759fb07e378facf728f3e1fcb19271f675251c5b737bb49ef52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.2 MB (191194625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d85efedf0835510ecb8428986837e4970be880965abf7942d80b84cb22f3d7a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:20:06 GMT
ADD file:11b1acca3f68b5c5787e292ff8dbdd114964a7272bf3519ab07710cbc01a0838 in / 
# Wed, 12 Apr 2023 00:20:06 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:30:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 03:30:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 03:31:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:31:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 03:31:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 03:34:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 03:34:32 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 03:34:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 03:34:42 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 03:34:42 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 03:34:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:34:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:34:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 04:27:46 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 14 Apr 2023 18:13:23 GMT
ENV PHP_VERSION=8.1.18
# Fri, 14 Apr 2023 18:13:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.18.tar.xz.asc
# Fri, 14 Apr 2023 18:13:23 GMT
ENV PHP_SHA256=f3553370f8ba42729a9ce75eed17a2111d32433a43b615694f6a571b8bad0e39
# Fri, 14 Apr 2023 18:13:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 14 Apr 2023 18:13:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 14 Apr 2023 18:16:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 14 Apr 2023 18:16:42 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 14 Apr 2023 18:16:42 GMT
RUN docker-php-ext-enable sodium
# Fri, 14 Apr 2023 18:16:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 14 Apr 2023 18:16:43 GMT
STOPSIGNAL SIGWINCH
# Fri, 14 Apr 2023 18:16:43 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 14 Apr 2023 18:16:43 GMT
WORKDIR /var/www/html
# Fri, 14 Apr 2023 18:16:43 GMT
EXPOSE 80
# Fri, 14 Apr 2023 18:16:43 GMT
CMD ["apache2-foreground"]
# Fri, 14 Apr 2023 19:41:34 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 14 Apr 2023 19:41:35 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 14 Apr 2023 19:41:35 GMT
COPY file:3cfddcfffbb1a2b0544304897907e3a08247bd92e3e7f53da87a4646baf89113 in /usr/local/bin/ 
# Thu, 20 Apr 2023 22:22:20 GMT
ENV DRUPAL_VERSION=9.5.8
# Thu, 20 Apr 2023 22:22:20 GMT
WORKDIR /opt/drupal
# Thu, 20 Apr 2023 22:22:32 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 20 Apr 2023 22:22:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:26c5c85e47da3022f1bdb9a112103646c5c29517d757e95426f16e4bd9533405`  
		Last Modified: Wed, 12 Apr 2023 00:23:43 GMT  
		Size: 31.4 MB (31418228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c8021d1258ac2078c39a88a97b3c834df2a1bf40f1b56f88bb237cc837c9cb`  
		Last Modified: Wed, 12 Apr 2023 05:43:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff43c2de6846ddda72bd88d8150e2bb08bca320f1f8ff895a2c09afae223ecb`  
		Last Modified: Wed, 12 Apr 2023 05:43:13 GMT  
		Size: 91.6 MB (91636376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383987c505e89f10b4ef0b1352d7b5e1337ed05746b6e846e0760340080ea1b3`  
		Last Modified: Wed, 12 Apr 2023 05:43:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd742e8a9047948bf878e97e03ed859b2e1ea0166b03d47e9a1499831661afd`  
		Last Modified: Wed, 12 Apr 2023 05:43:37 GMT  
		Size: 19.2 MB (19247938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9807e8362dee86d78138be851a43bc7c3865f9ad66636c29986613ba1986d`  
		Last Modified: Wed, 12 Apr 2023 05:43:34 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc7ce10028c7095e10505e24d1324b220d61f77b4b5665898ec0606c98f9fb`  
		Last Modified: Wed, 12 Apr 2023 05:43:35 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c835f75a2724543f783dbd9708ec2e71181b9f4262cafe42d3c961cc6174b9`  
		Last Modified: Fri, 14 Apr 2023 19:07:19 GMT  
		Size: 12.1 MB (12123100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8d91ebbe831a346729a16c86d75034aa6550d3c283b822d7540374314b5889`  
		Last Modified: Fri, 14 Apr 2023 19:07:16 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c538ea40cd1e971e52381f2cecb0c4d427c09a81c0301ad9592186bf4ef75c`  
		Last Modified: Fri, 14 Apr 2023 19:07:18 GMT  
		Size: 11.1 MB (11059020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf6e657c420a12b9a7030f266118cb634dc05515f2d9119ac26660682e006ef`  
		Last Modified: Fri, 14 Apr 2023 19:07:16 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564cd8aea1b3afac1db975e272ea22ebcfa4fdb0126b1455e2c30ada2f390e58`  
		Last Modified: Fri, 14 Apr 2023 19:07:16 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be10554faca55a3e0b178d2100ab1d4c0b41801b24b87f14f5d3da4d9acbe8ac`  
		Last Modified: Fri, 14 Apr 2023 19:07:16 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adefd2f9c8d5afdde856a051a9f0b83c9036f66302c5db44e436a79e6cb49d0`  
		Last Modified: Fri, 14 Apr 2023 19:57:02 GMT  
		Size: 2.1 MB (2139285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29cfa60d085eb84c368b744a14669dd235b5f20bbfacffd599b69a80fcdea49f`  
		Last Modified: Fri, 14 Apr 2023 19:57:02 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f1aed646bc4579c7b83cfbb3ea5e3f6465882807476d46b6f15e024886397c`  
		Last Modified: Fri, 14 Apr 2023 19:57:02 GMT  
		Size: 697.5 KB (697531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adc81c1b7e114c5c92bb8a636475abd9378318a373cf58c77ca50d47f9a0603`  
		Last Modified: Thu, 20 Apr 2023 22:36:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65460ed97081458153902c71153bb253e0b5be74a9c7d44c55186669d440c02e`  
		Last Modified: Thu, 20 Apr 2023 22:36:52 GMT  
		Size: 22.9 MB (22867103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-apache` - linux; arm variant v7

```console
$ docker pull drupal@sha256:4412552bce105c2d02e115cee4a6ddedc95f0b295c4358a9bc4bcdefd5dc2756
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.7 MB (160668174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cad6a26aa617020fde72819a976b0bab676e0b7f0ba9d69b3925511e28ae156`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:44 GMT
ADD file:e5f4777456ed4424053e9aa1f3d783f57da094c7a6c6d9d7a2fd315e00b5bbb0 in / 
# Tue, 11 Apr 2023 23:59:44 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 02:35:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 02:35:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 02:35:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:35:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 02:35:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 02:38:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 02:38:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 02:39:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 02:39:07 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 02:39:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 02:39:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:39:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 02:39:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 03:24:53 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 14 Apr 2023 19:00:56 GMT
ENV PHP_VERSION=8.1.18
# Fri, 14 Apr 2023 19:00:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.18.tar.xz.asc
# Fri, 14 Apr 2023 19:00:56 GMT
ENV PHP_SHA256=f3553370f8ba42729a9ce75eed17a2111d32433a43b615694f6a571b8bad0e39
# Fri, 14 Apr 2023 19:01:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 14 Apr 2023 19:01:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 14 Apr 2023 19:03:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 14 Apr 2023 19:03:28 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 14 Apr 2023 19:03:29 GMT
RUN docker-php-ext-enable sodium
# Fri, 14 Apr 2023 19:03:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 14 Apr 2023 19:03:29 GMT
STOPSIGNAL SIGWINCH
# Fri, 14 Apr 2023 19:03:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 14 Apr 2023 19:03:29 GMT
WORKDIR /var/www/html
# Fri, 14 Apr 2023 19:03:29 GMT
EXPOSE 80
# Fri, 14 Apr 2023 19:03:29 GMT
CMD ["apache2-foreground"]
# Fri, 14 Apr 2023 20:11:20 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 14 Apr 2023 20:11:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 14 Apr 2023 20:11:21 GMT
COPY file:3cfddcfffbb1a2b0544304897907e3a08247bd92e3e7f53da87a4646baf89113 in /usr/local/bin/ 
# Thu, 20 Apr 2023 23:29:59 GMT
ENV DRUPAL_VERSION=9.5.8
# Thu, 20 Apr 2023 23:29:59 GMT
WORKDIR /opt/drupal
# Thu, 20 Apr 2023 23:30:11 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 20 Apr 2023 23:30:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:99c2a28b4a43ce341eb611e82106b886315f30a250473617f2293828e10d8fff`  
		Last Modified: Wed, 12 Apr 2023 00:03:19 GMT  
		Size: 26.6 MB (26579772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4c3fcca6db962fb49617da5ac21af2abd9525daf0f8e86ce71084de6803ea`  
		Last Modified: Wed, 12 Apr 2023 04:28:06 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069f5e561d5b9a35f200f2b1559ae811ad4ce71d740a69aea8c443d39a7fdba7`  
		Last Modified: Wed, 12 Apr 2023 04:28:17 GMT  
		Size: 69.3 MB (69321908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a726bf573f3daeb69abfd49bd12ad0bd1e6359d8f5cc041c41666d11884385`  
		Last Modified: Wed, 12 Apr 2023 04:28:06 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c57805895b3164ed1094f4447fce0cc777d48119733e38be5422ddd5ca5311a`  
		Last Modified: Wed, 12 Apr 2023 04:28:43 GMT  
		Size: 18.0 MB (18007861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5995fde9a2075e1c9c21a7f309b0f0135cc693659d0bc7f2ae64164ffefc2b28`  
		Last Modified: Wed, 12 Apr 2023 04:28:39 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3130031726a984beae76cea03ce10079aeb4ea8190271f7e37e869992117a9ea`  
		Last Modified: Wed, 12 Apr 2023 04:28:39 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e848c5773fca7d36aebd0c8fe50b55fe1c01667036de6289de5e299020d8cb`  
		Last Modified: Fri, 14 Apr 2023 19:44:08 GMT  
		Size: 12.1 MB (12121305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1772be2cbfff84fe8c90b4a75726cd7640bc6914e5b6a2e0cea5c8c359bc87`  
		Last Modified: Fri, 14 Apr 2023 19:44:05 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fec009a60e04a0c3b230ec97070b5804dd738854904742239583639d677b1c8`  
		Last Modified: Fri, 14 Apr 2023 19:44:08 GMT  
		Size: 9.6 MB (9551829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97fb9c27c36fcf608bd6f803de03e58169ce2f8202b937bed9a1fa6944e1e52`  
		Last Modified: Fri, 14 Apr 2023 19:44:05 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb265034ccedd4a9aad1105bbe975a5c22c9e873fe18f50c6b2378fb3834371b`  
		Last Modified: Fri, 14 Apr 2023 19:44:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d58e9c2108b702793c893fa6264bbe3d8eb32e6a35b1edefe44253f204d220e`  
		Last Modified: Fri, 14 Apr 2023 19:44:05 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0798eec21d8345bd6afb9ee548d1b9db3c2a226a3a7e8b2e0137d25bc8ed309`  
		Last Modified: Fri, 14 Apr 2023 20:26:28 GMT  
		Size: 1.5 MB (1514666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926249958f3050349af9c8fbd87ac01f16dee529e7a4839aaa284c27daffd82e`  
		Last Modified: Fri, 14 Apr 2023 20:26:27 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0984834f08a3291724f42d4b847a0e3a178e99efffb14b077dcc4287f995d398`  
		Last Modified: Fri, 14 Apr 2023 20:26:28 GMT  
		Size: 697.5 KB (697531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0316b75d256603a1e757182e27c36f4ed914037f0b7c7bf88f501f79416621bc`  
		Last Modified: Thu, 20 Apr 2023 23:48:05 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91a3ae84efa9a48869adfe1b427b8547bd0c29dd9a1e0f46ab96d30067d70b1`  
		Last Modified: Thu, 20 Apr 2023 23:48:11 GMT  
		Size: 22.9 MB (22867266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-apache` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:ae972c0c7d2085c5d173cf61d80501a06fba6f862f673d6ae269218daf767b32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.4 MB (185383832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc8aac969210d2413e6e2d80c4ec2717993c1e222db10643b87d169db76dc5f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:52:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 03 May 2023 03:52:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 03 May 2023 03:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:52:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 03 May 2023 03:52:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 03 May 2023 03:56:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 03 May 2023 03:56:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 03 May 2023 03:56:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 03 May 2023 03:56:14 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 03 May 2023 03:56:14 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 03 May 2023 03:56:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 03:56:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 03:56:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 03 May 2023 04:45:47 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 03 May 2023 05:10:08 GMT
ENV PHP_VERSION=8.1.18
# Wed, 03 May 2023 05:10:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.18.tar.xz.asc
# Wed, 03 May 2023 05:10:08 GMT
ENV PHP_SHA256=f3553370f8ba42729a9ce75eed17a2111d32433a43b615694f6a571b8bad0e39
# Wed, 03 May 2023 05:10:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 03 May 2023 05:10:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 03 May 2023 05:13:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 03 May 2023 05:13:10 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 03 May 2023 05:13:10 GMT
RUN docker-php-ext-enable sodium
# Wed, 03 May 2023 05:13:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 03 May 2023 05:13:10 GMT
STOPSIGNAL SIGWINCH
# Wed, 03 May 2023 05:13:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 03 May 2023 05:13:11 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 05:13:11 GMT
EXPOSE 80
# Wed, 03 May 2023 05:13:11 GMT
CMD ["apache2-foreground"]
# Wed, 03 May 2023 23:08:27 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:08:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 03 May 2023 23:08:27 GMT
COPY file:3cfddcfffbb1a2b0544304897907e3a08247bd92e3e7f53da87a4646baf89113 in /usr/local/bin/ 
# Wed, 03 May 2023 23:13:31 GMT
ENV DRUPAL_VERSION=9.5.9
# Wed, 03 May 2023 23:13:31 GMT
WORKDIR /opt/drupal
# Wed, 03 May 2023 23:13:41 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 03 May 2023 23:13:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3582e155c24272674265389c3b317b84bec7ca237a6761ee690aed30a1c5ec9`  
		Last Modified: Wed, 03 May 2023 05:50:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313de6edf03aac188b999f642b424cdc014f9f45e218d5ad620a727ef81fa7e1`  
		Last Modified: Wed, 03 May 2023 05:51:02 GMT  
		Size: 86.9 MB (86928311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a576c500430404ceffd53e7ce6f2898b260e011e85c77bdabd75342c1a6a54`  
		Last Modified: Wed, 03 May 2023 05:50:53 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249c4246fc75d4a1eefb130895fc367d8150e7076da4e329f94094a45c81cf4e`  
		Last Modified: Wed, 03 May 2023 05:51:26 GMT  
		Size: 19.2 MB (19170211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbc677cfb25a8634144c25b4c4f43c1173f08ca1eb16b4f3ae53aa11bc62040`  
		Last Modified: Wed, 03 May 2023 05:51:24 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca53ccc29d8c43aeff9c96a48096d009ccf0ee902bf0b5076defe39003f2a0e`  
		Last Modified: Wed, 03 May 2023 05:51:24 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d4c5c8e5da5ee12d25cc66088d25127c2aae0c6c8ca98e66c5005744849bb09`  
		Last Modified: Wed, 03 May 2023 05:58:52 GMT  
		Size: 12.1 MB (12122246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f2f08835715328d465bff0833e5d47a7040ccc6e81173bcbdfdc590155c1f3`  
		Last Modified: Wed, 03 May 2023 05:58:50 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1543c77ab1471adf87f1e747fcb65dd2848dcdd5a2e57f1d4fbfb85740ee15ad`  
		Last Modified: Wed, 03 May 2023 05:58:51 GMT  
		Size: 11.1 MB (11129781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7254506894587666a75a9f0500cd0d9a57971a3a45a99f54f3a471e1b0601572`  
		Last Modified: Wed, 03 May 2023 05:58:50 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ddcbe89ca469c5d5ee0ad97571f8e481adfc0cc0e47fd850342bdfd4d4c93e`  
		Last Modified: Wed, 03 May 2023 05:58:50 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498e094437d7f9d3c9d688fd05796c57761c88fe959a480e770c1cdbb6f9855d`  
		Last Modified: Wed, 03 May 2023 05:58:50 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10ee8be1a317b9774f538723b02b7f62276a67a3bbdca8c83237d282af14f6b`  
		Last Modified: Wed, 03 May 2023 23:29:16 GMT  
		Size: 2.4 MB (2398993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09744e5227d34eae6455c2f5e47af63a1788995ea3141e7b0b30649ecae8cc12`  
		Last Modified: Wed, 03 May 2023 23:29:15 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db974a24b8920b5758dba5a8644fa35cf4a709314925f54073c8d432e855af2`  
		Last Modified: Wed, 03 May 2023 23:29:16 GMT  
		Size: 697.5 KB (697534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3403e2f95d053dfc8242dd101d80338a21e7afd2b7200ff257debe257d53cc7b`  
		Last Modified: Wed, 03 May 2023 23:31:35 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293701c9d07b7fdd4840abe75ccce9fb8f997b00513e7edae3adb791cf82d845`  
		Last Modified: Wed, 03 May 2023 23:31:39 GMT  
		Size: 22.9 MB (22878005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-apache` - linux; 386

```console
$ docker pull drupal@sha256:25583e04e97717a64cfbe229a6965f2b152332510090eaa56955b63fc5603b55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.0 MB (194042020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d911c4b177e2573983a90358f4fc35a1f4df03a33c5d43eb5d9c9417a5d3d630`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:01 GMT
ADD file:42fc1b4536cdd6823499b0c94d799e9bfbcb280b7df55d8d6c9f6defd61ecb6e in / 
# Wed, 12 Apr 2023 00:39:01 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:10:35 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 05:10:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 05:10:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:10:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 05:10:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 05:16:27 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 05:16:27 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 05:16:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 05:16:40 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 05:16:41 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 05:16:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 05:16:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 05:16:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 06:41:42 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 14 Apr 2023 19:07:57 GMT
ENV PHP_VERSION=8.1.18
# Fri, 14 Apr 2023 19:07:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.18.tar.xz.asc
# Fri, 14 Apr 2023 19:07:57 GMT
ENV PHP_SHA256=f3553370f8ba42729a9ce75eed17a2111d32433a43b615694f6a571b8bad0e39
# Fri, 14 Apr 2023 19:08:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 14 Apr 2023 19:08:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 14 Apr 2023 19:13:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 14 Apr 2023 19:13:08 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 14 Apr 2023 19:13:08 GMT
RUN docker-php-ext-enable sodium
# Fri, 14 Apr 2023 19:13:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 14 Apr 2023 19:13:09 GMT
STOPSIGNAL SIGWINCH
# Fri, 14 Apr 2023 19:13:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 14 Apr 2023 19:13:09 GMT
WORKDIR /var/www/html
# Fri, 14 Apr 2023 19:13:09 GMT
EXPOSE 80
# Fri, 14 Apr 2023 19:13:09 GMT
CMD ["apache2-foreground"]
# Fri, 14 Apr 2023 22:12:26 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 14 Apr 2023 22:12:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 14 Apr 2023 22:12:27 GMT
COPY file:3cfddcfffbb1a2b0544304897907e3a08247bd92e3e7f53da87a4646baf89113 in /usr/local/bin/ 
# Thu, 20 Apr 2023 22:41:29 GMT
ENV DRUPAL_VERSION=9.5.8
# Thu, 20 Apr 2023 22:41:29 GMT
WORKDIR /opt/drupal
# Thu, 20 Apr 2023 22:41:41 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 20 Apr 2023 22:41:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b2ee1f87789d52ef09851b4e5c9745fb8aceafa107b0d3452f9973f1abe65042`  
		Last Modified: Wed, 12 Apr 2023 00:42:45 GMT  
		Size: 32.4 MB (32398925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c63f93493e2a7820d4f2332775c7575bc5ab3d2358b167eadf787455f1f0410`  
		Last Modified: Wed, 12 Apr 2023 08:42:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf8627b0cb08594b65741f86baf83146a59f931e067c980b9b9cbf93b9dae7f`  
		Last Modified: Wed, 12 Apr 2023 08:42:44 GMT  
		Size: 92.7 MB (92720432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef01aa4975c4bb966cd891dd1e9ed26a36289e162af712fae5029523ceba1da2`  
		Last Modified: Wed, 12 Apr 2023 08:42:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5aab49493f783cb3588fbdb360f327923f8203d285c8861c959dc0aab7f583`  
		Last Modified: Wed, 12 Apr 2023 08:43:11 GMT  
		Size: 19.7 MB (19737131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b27c6cf07dac2e735443afa879e4e000d2c84c4066edb2c0e041c77a647ce5`  
		Last Modified: Wed, 12 Apr 2023 08:43:07 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e9b59d0c0e207b2e7d49b56f2ac2b42d4c855c82e136f8abb6909607008f88`  
		Last Modified: Wed, 12 Apr 2023 08:43:07 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0970886119c5b7e2daec028476b25ab66bcfabb5f0485e19c54d4a38618ddc`  
		Last Modified: Fri, 14 Apr 2023 20:33:34 GMT  
		Size: 12.1 MB (12122322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9be5fe514891af9a8b0f5e4ddbfa1597c3e01fb0e3f2bf58af03bfc4a588db`  
		Last Modified: Fri, 14 Apr 2023 20:33:31 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ceb836027083ec640009a7e2efdecf04d1fe01cd6ed3d98f045b2a161721a3`  
		Last Modified: Fri, 14 Apr 2023 20:33:34 GMT  
		Size: 11.3 MB (11289986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce290b38837247733e3f1006e97f0fea79c78bfafbfc7ad98c762b6030bf674`  
		Last Modified: Fri, 14 Apr 2023 20:33:31 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42ccb4c45e23e76803a24b5a4f176ecdc46e7e9f94cc4eba0868bd6b0f60c5c`  
		Last Modified: Fri, 14 Apr 2023 20:33:31 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e947b18ce35072b84266a5939007caca03676c7e84c0cc399cee4f9c4f340459`  
		Last Modified: Fri, 14 Apr 2023 20:33:31 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8099ab8c256023f5ad7c57ea1a73cd234fb9de97cefe10448b8a23a0a5a6e585`  
		Last Modified: Fri, 14 Apr 2023 22:29:40 GMT  
		Size: 2.2 MB (2203376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129fade1ec212471a72e594b8694379946d631ba4147ea0e66ee1a47b9b2d4ff`  
		Last Modified: Fri, 14 Apr 2023 22:29:39 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd044746dc92622b61182e42134f49c2c825341fabce2bb7fca2d3e488bf2539`  
		Last Modified: Fri, 14 Apr 2023 22:29:40 GMT  
		Size: 697.5 KB (697532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f25ec02cc4d8f1458c8b44c60f66387f249d5d7c3e915e1fdfc65b8f5e2813`  
		Last Modified: Thu, 20 Apr 2023 22:57:16 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25068c699b48cb38c0712694e7c925918515ee9f440a84d4a5ed808b0d0dd14`  
		Last Modified: Thu, 20 Apr 2023 22:57:24 GMT  
		Size: 22.9 MB (22866275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-apache` - linux; ppc64le

```console
$ docker pull drupal@sha256:e90cb4e9396b2712b9b9de37981a511b1524fa0fa412f8a6993ade36d88c22e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.5 MB (191546040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ec465337bef2f4b2940115466559d2f5f32808e2cb7ab0cfb48a010c0a02e65`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:08:20 GMT
ADD file:63eb52aaff02c15bceabb87a78eb1b36389066ff4774cf8a754160ca7d509816 in / 
# Wed, 12 Apr 2023 00:08:23 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 02:53:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 02:53:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 02:54:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 02:55:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 02:55:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 03:00:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 03:00:03 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 03:00:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 03:00:30 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 03:00:31 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 03:00:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:00:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:00:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 03:40:32 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 14 Apr 2023 18:11:50 GMT
ENV PHP_VERSION=8.1.18
# Fri, 14 Apr 2023 18:11:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.18.tar.xz.asc
# Fri, 14 Apr 2023 18:11:50 GMT
ENV PHP_SHA256=f3553370f8ba42729a9ce75eed17a2111d32433a43b615694f6a571b8bad0e39
# Fri, 14 Apr 2023 18:12:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 14 Apr 2023 18:12:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 14 Apr 2023 18:16:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 14 Apr 2023 18:16:29 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 14 Apr 2023 18:16:30 GMT
RUN docker-php-ext-enable sodium
# Fri, 14 Apr 2023 18:16:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 14 Apr 2023 18:16:30 GMT
STOPSIGNAL SIGWINCH
# Fri, 14 Apr 2023 18:16:31 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 14 Apr 2023 18:16:31 GMT
WORKDIR /var/www/html
# Fri, 14 Apr 2023 18:16:31 GMT
EXPOSE 80
# Fri, 14 Apr 2023 18:16:31 GMT
CMD ["apache2-foreground"]
# Fri, 14 Apr 2023 19:33:39 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 14 Apr 2023 19:33:40 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 14 Apr 2023 19:33:41 GMT
COPY file:3cfddcfffbb1a2b0544304897907e3a08247bd92e3e7f53da87a4646baf89113 in /usr/local/bin/ 
# Thu, 20 Apr 2023 22:22:20 GMT
ENV DRUPAL_VERSION=9.5.8
# Thu, 20 Apr 2023 22:22:21 GMT
WORKDIR /opt/drupal
# Thu, 20 Apr 2023 22:22:46 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 20 Apr 2023 22:22:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:5b41d5ec640939cf684959234ad3b80909268a32bfd520a31c6720a91521c2fa`  
		Last Modified: Wed, 12 Apr 2023 00:13:13 GMT  
		Size: 35.3 MB (35291995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4881dab4e16a2b31707f063b4a6d06a7622c29a571e9941b45d4f1dbab9fa535`  
		Last Modified: Wed, 12 Apr 2023 04:52:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7112207942602cdd0c4444cb2cf85085ac4ac494a4140f7ad0d4b40bc5d9af2`  
		Last Modified: Wed, 12 Apr 2023 04:53:17 GMT  
		Size: 86.6 MB (86633054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc8a1d48af817593b6b8be59cd4822dcbbf90138a02afc42d1c359a66cef044`  
		Last Modified: Wed, 12 Apr 2023 04:52:52 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eebee4fe70939a7f850866922cd16aca329703d3398407739e4b38a6f027d89`  
		Last Modified: Wed, 12 Apr 2023 04:53:47 GMT  
		Size: 20.5 MB (20464162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbb6aa8a531755afded14a8c4ba085e312d53bcaf78332aeafd1dd4d3d8dbc0`  
		Last Modified: Wed, 12 Apr 2023 04:53:42 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef12174c7227dbbeb6d056ac319756c11bf63363c72a33b9ab7899b9dfc7f097`  
		Last Modified: Wed, 12 Apr 2023 04:53:42 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c38e27804e7de781604fc7987995b611df38c6a144b877111134cb04e95ff00`  
		Last Modified: Fri, 14 Apr 2023 19:01:39 GMT  
		Size: 12.1 MB (12122982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b2d3d9d03551f7b0e4d7a786c89a9612a0aaed6dc9739c38c242de28cec0c3`  
		Last Modified: Fri, 14 Apr 2023 19:01:36 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f9b9401d9b048c57fcd45d13667c1760401834c81f5d480d7f94fed1b8b59b`  
		Last Modified: Fri, 14 Apr 2023 19:01:40 GMT  
		Size: 11.5 MB (11462631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5dddce9d56b1b4fa337645bcd5b1c5713358aed99710c505a83c95cf501945`  
		Last Modified: Fri, 14 Apr 2023 19:01:36 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be96b43a01486cbe7e5cbf79cd3e989b133d1fa4114756332c46998ee86994c0`  
		Last Modified: Fri, 14 Apr 2023 19:01:37 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087bbc8144cc96eb647c719e768a85951d09c41f6aeb2670cbb9313a594c0687`  
		Last Modified: Fri, 14 Apr 2023 19:01:36 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cebc1edbb6ecdae6d5e5879f87e343bbca9a09876b9f89b96d97a2b724730d`  
		Last Modified: Fri, 14 Apr 2023 19:49:30 GMT  
		Size: 2.0 MB (2001028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c19e1ee9927e06f425b215feca94ee6784ac3f8bc950dd9dd686138a7734a15`  
		Last Modified: Fri, 14 Apr 2023 19:49:30 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92a0532bc3a9037cf789faf430ac032b14d76fdd7b6bac6f0a42ff93134146f`  
		Last Modified: Fri, 14 Apr 2023 19:49:30 GMT  
		Size: 697.5 KB (697531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b03ba0e8d8937dfb7b3837320d875192426ba00515567c6f67e8ce2f300f321`  
		Last Modified: Thu, 20 Apr 2023 22:44:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd594b6ec60b4114867019649b7db51a823e45ecd17d900553e773dcf9464f7`  
		Last Modified: Thu, 20 Apr 2023 22:44:33 GMT  
		Size: 22.9 MB (22866617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-apache` - linux; s390x

```console
$ docker pull drupal@sha256:ab14de5ac661476c0e117064ac665256ab2f607a77e9ba1eaf27e196e60fa62d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.0 MB (167979175 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c61e5c9ffe67fa4407a21e1409f32a652ac3a6f291fc0532f5db58c94c5cbfe6`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 12 Apr 2023 00:01:00 GMT
ADD file:b6463dba97ba9c0a29bacfafc4d67bc603ab57e80b75e23cd42d7ef4b0f8e6ae in / 
# Wed, 12 Apr 2023 00:01:04 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 03:36:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 12 Apr 2023 03:36:39 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 12 Apr 2023 03:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 03:37:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 12 Apr 2023 03:37:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 12 Apr 2023 03:41:16 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 12 Apr 2023 03:41:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 12 Apr 2023 03:41:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 12 Apr 2023 03:41:37 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 12 Apr 2023 03:41:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 12 Apr 2023 03:41:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:41:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 12 Apr 2023 03:41:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 12 Apr 2023 04:07:25 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 14 Apr 2023 18:13:27 GMT
ENV PHP_VERSION=8.1.18
# Fri, 14 Apr 2023 18:13:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.18.tar.xz.asc
# Fri, 14 Apr 2023 18:13:27 GMT
ENV PHP_SHA256=f3553370f8ba42729a9ce75eed17a2111d32433a43b615694f6a571b8bad0e39
# Fri, 14 Apr 2023 18:13:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 14 Apr 2023 18:13:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 14 Apr 2023 18:15:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 14 Apr 2023 18:15:40 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 14 Apr 2023 18:15:41 GMT
RUN docker-php-ext-enable sodium
# Fri, 14 Apr 2023 18:15:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 14 Apr 2023 18:15:41 GMT
STOPSIGNAL SIGWINCH
# Fri, 14 Apr 2023 18:15:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 14 Apr 2023 18:15:42 GMT
WORKDIR /var/www/html
# Fri, 14 Apr 2023 18:15:42 GMT
EXPOSE 80
# Fri, 14 Apr 2023 18:15:42 GMT
CMD ["apache2-foreground"]
# Sat, 29 Apr 2023 03:44:51 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 29 Apr 2023 03:44:51 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 29 Apr 2023 03:44:51 GMT
COPY file:3cfddcfffbb1a2b0544304897907e3a08247bd92e3e7f53da87a4646baf89113 in /usr/local/bin/ 
# Sat, 29 Apr 2023 03:48:10 GMT
ENV DRUPAL_VERSION=9.5.8
# Sat, 29 Apr 2023 03:48:10 GMT
WORKDIR /opt/drupal
# Sat, 29 Apr 2023 03:48:21 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 29 Apr 2023 03:48:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:97fe10bc7def58e7938e97e41eec4788ec7a45b6ef2cb1770cec02fa831fd19d`  
		Last Modified: Wed, 12 Apr 2023 00:05:18 GMT  
		Size: 29.7 MB (29653156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943e763db148606393f8c21697bc30f68ac8de11269141ae6e0d5e8483fe3e26`  
		Last Modified: Wed, 12 Apr 2023 04:40:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f8d95603c0d1c5673103183c025b2e49c72c82f4e8b4b3a86201eb804e7ffa`  
		Last Modified: Wed, 12 Apr 2023 04:40:55 GMT  
		Size: 71.6 MB (71629155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e864c428fd73e9e002327cf91695b364814ad36e7552a314e87ab897ca522f`  
		Last Modified: Wed, 12 Apr 2023 04:40:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4dc168720ddd2f3887093d1b990253b126ba4d7c7b85c8cdcaaa56cde796d25`  
		Last Modified: Wed, 12 Apr 2023 04:41:11 GMT  
		Size: 19.1 MB (19077445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994e736e66f1a50d03c9d0c3f816ba709888f0c93602761fdd8ce401cf3393d1`  
		Last Modified: Wed, 12 Apr 2023 04:41:09 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b0a054484820a2aa7ec78a477993298451eb46eb32bedad190e57fb199bee4`  
		Last Modified: Wed, 12 Apr 2023 04:41:09 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2387ee9dff9d5b5cf81e0011e6847dee9e8f781992a1a0148f68a5abf5b468`  
		Last Modified: Fri, 14 Apr 2023 18:45:17 GMT  
		Size: 12.1 MB (12121945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787ea0454acfc935e72d2fc92a5fd610d219efaeeb133d6035a3758c052d9c68`  
		Last Modified: Fri, 14 Apr 2023 18:45:15 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210c25d9e7541485cff7d72e07cb409e9f14cb2d2c932b9642a4070ddaa4b0a`  
		Last Modified: Fri, 14 Apr 2023 18:45:17 GMT  
		Size: 10.2 MB (10198667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b31baa254b0a6b47814da3fc7308afa527a393da5c1417a40e26b06b10e4e9e`  
		Last Modified: Fri, 14 Apr 2023 18:45:15 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff88526626c2a7328a8a69703a90f982cfabfad3b7e7103241b7953e0dd0c0`  
		Last Modified: Fri, 14 Apr 2023 18:45:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28908c07867ac9e17c6538620a358249ad68f992f3a2cd69001577d1c198eb27`  
		Last Modified: Fri, 14 Apr 2023 18:45:15 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f748da1526eee08161754df12fffd48f06df951b320f6c847556c8625a522e37`  
		Last Modified: Sat, 29 Apr 2023 03:56:40 GMT  
		Size: 1.7 MB (1729548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f601ba1ee72d647dbb74c57adc2a18ee37f6c5bf6af64a3c4b683111141240`  
		Last Modified: Sat, 29 Apr 2023 03:56:40 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c6f91c59af432ec9f92235a84cdaa64a06c926f78e7f2db37f45e0e2100818`  
		Last Modified: Sat, 29 Apr 2023 03:56:40 GMT  
		Size: 697.5 KB (697532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2398a7dab029ca6d6baf1cd8ee52f386bf0719973f9a96fcf2f86b4cb03bdf`  
		Last Modified: Sat, 29 Apr 2023 03:57:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e70397d7da09deab4a425910f32aff9454b82119b3bc786e65555d9bc49752`  
		Last Modified: Sat, 29 Apr 2023 03:57:43 GMT  
		Size: 22.9 MB (22865681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
