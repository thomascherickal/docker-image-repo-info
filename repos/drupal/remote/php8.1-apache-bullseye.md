## `drupal:php8.1-apache-bullseye`

```console
$ docker pull drupal@sha256:b85854c97dbd10421131f1eeae71d4fc9b78e7fd354eb4cac20d842ace1e5f1e
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 12
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `drupal:php8.1-apache-bullseye` - linux; amd64

```console
$ docker pull drupal@sha256:20061d3ca25bd56e2d8d50e08ee39731bba2ed65b27504a77fb2c7e0e4a2060d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.7 MB (186737436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:796f795915ae930238fa03c53b38dee2ebea06d4b7669bf328a324c083bbbf92`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 17:45:09 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 01 Nov 2023 17:45:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Nov 2023 17:45:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_VERSION=8.1.26
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 17:45:09 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 17:45:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 17:45:09 GMT
STOPSIGNAL SIGWINCH
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
EXPOSE 80
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["apache2-foreground"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0754b57b9b7d3a089ca18ba98121861a56ce2624c2875a8e7bf8b21a7957eec8`  
		Last Modified: Tue, 21 Nov 2023 16:37:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71e5060f3937930b5fa3d39f56adf3c2acfea72741014d1969f3f437e5835631`  
		Last Modified: Tue, 21 Nov 2023 16:37:56 GMT  
		Size: 91.6 MB (91635313 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f25a6e74b7f558f50a59c2efa94a62c44a6323861b0c76e6d2144078ab6c5ed4`  
		Last Modified: Tue, 21 Nov 2023 16:37:43 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5d33b602102b183f8435dd317aff8889153fbf7eb46df307891feaa427a627c`  
		Last Modified: Tue, 21 Nov 2023 16:38:15 GMT  
		Size: 19.3 MB (19259224 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:866c9e44fbd45ff348f92197e8339f30a9888e80f74473a4354e370b3039760f`  
		Last Modified: Tue, 21 Nov 2023 16:38:12 GMT  
		Size: 473.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd2572036f7c292392aafb9fb89d2ce0215b5dcb6c8046f4e3eba4933e1f16d0`  
		Last Modified: Tue, 21 Nov 2023 16:38:12 GMT  
		Size: 512.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e16fcd567f28dcf22888ee0caf43845c4e7f4db39e68b6b0b8514d5550f465c`  
		Last Modified: Tue, 28 Nov 2023 00:21:14 GMT  
		Size: 12.2 MB (12150756 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73f4404bb6e057be5fb6c457525bd1ab691a86da5c223d147db7bfcd71bc7009`  
		Last Modified: Tue, 28 Nov 2023 00:21:11 GMT  
		Size: 494.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2745d10cb90124b66db79cfcec43bb1e7e3f49e58423467f9fd536578e64545f`  
		Last Modified: Tue, 28 Nov 2023 00:21:13 GMT  
		Size: 11.1 MB (11084729 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc4a8ef0c2f5e304c276de975cdd21cb20c261cbe8544a2190e34543adaa1df1`  
		Last Modified: Tue, 28 Nov 2023 00:21:11 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bd8a0241915293301827fab7488cd4a755adfafbc6c0ad0ae4949b54dc55b854`  
		Last Modified: Tue, 28 Nov 2023 00:21:11 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5dc099515e163becb8fbdc71bfe0e58b3b7f22fd9cd8067fbb1415895d0b546`  
		Last Modified: Tue, 28 Nov 2023 00:21:11 GMT  
		Size: 895.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d75922a1c7b1d1a693d1cf762953cf20d240be602df143ac3335a1b052b99d2`  
		Last Modified: Tue, 28 Nov 2023 02:24:08 GMT  
		Size: 1.9 MB (1923881 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e2094212e919eb723fbb99880df4e2dd4f97b002333f3edc25521fb8eb7b4a58`  
		Last Modified: Tue, 28 Nov 2023 02:24:08 GMT  
		Size: 314.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aa15d4f3bb165baeade906b4cb792273dd3cc92b57acdd22b5ce014b9c858479`  
		Last Modified: Tue, 28 Nov 2023 02:24:08 GMT  
		Size: 705.0 KB (705004 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d21fafda1718488db18442dbd3051506b188aa0a02017072dc3275c382b850d3`  
		Last Modified: Tue, 28 Nov 2023 02:24:08 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3621220709339089add3a2e19e560dcca05a1ee5af8337d2992d79738e31e07c`  
		Last Modified: Tue, 28 Nov 2023 02:24:10 GMT  
		Size: 18.6 MB (18554701 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:8442b4b56ee1a7fb2f1b849d3aadfddcd5ac2e0b5e551fd2e7e2b3eec7ae7030
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6004610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b976deb8bd7a08fb1618c4d972a8caa89b240510980028804ada24163fd6ca6e`

```dockerfile
```

-	Layers:
	-	`sha256:26a4be7df842f5f143ab13fd01ca217b31b45cc414a1061e920763bda2ebb04a`  
		Last Modified: Tue, 28 Nov 2023 02:24:08 GMT  
		Size: 6.0 MB (5965486 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:47e2bd1a055dcf3eb3142840f4f7c85f4c53ca42328a5245a93157c007310b45`  
		Last Modified: Tue, 28 Nov 2023 02:24:07 GMT  
		Size: 39.1 KB (39124 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:php8.1-apache-bullseye` - linux; arm variant v7

```console
$ docker pull drupal@sha256:deddadeff82faf5099c2938baf76fea143762e3a2a1d47b3c7c2210616280f5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156202748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b2a4eb8ed3e4d4d2357946781b7d9fdfd37900224538309d2ebfb12f9e126ad`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 17:45:09 GMT
ADD file:c4afced274aaa80ab3018b368ed739c1c55e49b41e9637ac44d63e61344fe865 in / 
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 01 Nov 2023 17:45:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Nov 2023 17:45:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_VERSION=8.1.26
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 17:45:09 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 17:45:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 17:45:09 GMT
STOPSIGNAL SIGWINCH
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
EXPOSE 80
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["apache2-foreground"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:6dc4ed5513793308b8e30b08e03f97fa54025c3d3f3172c6edccb1dbbc7ff139`  
		Last Modified: Tue, 21 Nov 2023 04:02:35 GMT  
		Size: 26.6 MB (26579014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f00118114a1839c710dff505972914cfb60bfc81927081b4315a18f6c424531f`  
		Last Modified: Tue, 21 Nov 2023 10:52:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9fbdada88591659c80fda241d952db57844abfa1bddf9bd59aed59eb4e756389`  
		Last Modified: Tue, 21 Nov 2023 10:52:37 GMT  
		Size: 69.3 MB (69322894 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:898f115413ab5c0481075f5e637d041f9c76020e040854004fd7188869d6cf2d`  
		Last Modified: Tue, 21 Nov 2023 10:52:25 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5bccac24513cce414ff6f596621792454590cfcfebd2d8f3db79651bbd72050`  
		Last Modified: Tue, 21 Nov 2023 10:52:57 GMT  
		Size: 18.0 MB (18017813 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c712ec22d9e608ec098ccfd3d6f03dc49ad78131e6f220bb9d8c9b0412998b1a`  
		Last Modified: Tue, 21 Nov 2023 10:52:53 GMT  
		Size: 475.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:35499e190aed7216d431797b167104750ed92b22ab148e52b96bca41bb1c4784`  
		Last Modified: Tue, 21 Nov 2023 10:52:53 GMT  
		Size: 511.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fdaef2b5402f785a8bc7165719601b970cd4df096f840bc6bfa5d89b99036cec`  
		Last Modified: Mon, 27 Nov 2023 23:58:23 GMT  
		Size: 12.1 MB (12149358 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5cc7128ddf298e6e0809b2a467d7412ea2cd2403bf840b8aafc9185ece401652`  
		Last Modified: Mon, 27 Nov 2023 23:58:20 GMT  
		Size: 494.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f79b0f75f251b7bcbeb85b3850c329f2388aa020de1473e3db734725b41437b`  
		Last Modified: Mon, 27 Nov 2023 23:58:23 GMT  
		Size: 9.6 MB (9569243 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f911f18d20867f2aa922be2f6dfde0bf496e31cd3dcf20a0c29df3705a3ab776`  
		Last Modified: Mon, 27 Nov 2023 23:58:20 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f62818ed1085bbad7b76d3c3a475db909a60434d079c55acb1bd83774055a777`  
		Last Modified: Mon, 27 Nov 2023 23:58:20 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a88d5f5fa0306e263d3bdf17e5aec82ad10fd806766ef95a03e565d50277d031`  
		Last Modified: Mon, 27 Nov 2023 23:58:20 GMT  
		Size: 897.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a3fc557a03953a4439d757cc7de90fafbd496d8ee2084d202278761b619bf24`  
		Last Modified: Tue, 28 Nov 2023 03:40:20 GMT  
		Size: 1.3 MB (1298863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8086ad593e88f942ae8b5163ec2428ebed0479f5cc15309a492de66ec2b3f8`  
		Last Modified: Tue, 28 Nov 2023 03:40:19 GMT  
		Size: 314.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b1f11507fcc68104c913217acf1747343e36e4ad6d454f01a88383b816b7003`  
		Last Modified: Tue, 28 Nov 2023 03:40:19 GMT  
		Size: 705.0 KB (705007 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6468cb04f040d9643d1a53430a5088380eaa58a837e45db5f010bc35e1efd6c6`  
		Last Modified: Tue, 28 Nov 2023 03:40:20 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77e9cc6c8b55804d5598ada8d418835039aa3e4b885b2f813567728eb81f8c06`  
		Last Modified: Tue, 28 Nov 2023 03:40:22 GMT  
		Size: 18.6 MB (18554547 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:2327876e21de6495e2babad873929ab7fe808c44eb6b7b06d7c36e552cc5c8d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5834803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccd48b96f71b2976b73301f2fc3e1c589f11b0267ef4eb711d22592551aaf3ef`

```dockerfile
```

-	Layers:
	-	`sha256:f1e94954aa79db7465504af845d6dbd5b1ac836fb5e59407de152f2876279f0c`  
		Last Modified: Tue, 28 Nov 2023 04:19:50 GMT  
		Size: 5.8 MB (5799954 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d46abcdfeb8fbf72a9e0638ade6f7a2d6cd08bc5af0bd899128ac90b6f03f043`  
		Last Modified: Tue, 28 Nov 2023 04:19:49 GMT  
		Size: 34.8 KB (34849 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:php8.1-apache-bullseye` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:c039f1c1271eb8fbcd084a1e0a25f50768c5bd8ea947c8ff6fed566667bad47e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.9 MB (180927727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4f6eb38c473354313a097f4e2e1963e7c91d448cabfd567903817148d6a1fa8`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 17:45:09 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 01 Nov 2023 17:45:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Nov 2023 17:45:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_VERSION=8.1.26
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 17:45:09 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 17:45:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 17:45:09 GMT
STOPSIGNAL SIGWINCH
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
EXPOSE 80
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["apache2-foreground"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d962dd5329fe78a5b7771f5e8185e57fa02ab85dd0e29d06209fd0c765e4fcfe`  
		Last Modified: Tue, 21 Nov 2023 16:36:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:343833a8d9a793ce2a45a7c002adfa6a3bb5a7979770e9179de28b8e5adf8ca7`  
		Last Modified: Tue, 21 Nov 2023 16:36:48 GMT  
		Size: 86.9 MB (86933577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2591c5ed67a6732c68cab0f741ba7fc77bb24bab13c72c0c116435b6a4009c6`  
		Last Modified: Tue, 21 Nov 2023 16:36:39 GMT  
		Size: 272.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a83b5f940f44725d68bd99daece80d68f31be2e8556e630a054c3f25c95caea7`  
		Last Modified: Tue, 21 Nov 2023 16:37:06 GMT  
		Size: 19.2 MB (19177585 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe40c918833f655210f1f82dacfd83abd2298a6dbef516604dae8e314a41368e`  
		Last Modified: Tue, 21 Nov 2023 16:37:04 GMT  
		Size: 475.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a9ad5a90509716966c24807c6e5995b82c37154367e22c79ea4d3802cf30ef65`  
		Last Modified: Tue, 21 Nov 2023 16:37:03 GMT  
		Size: 512.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:371f532178608a0f60d012c5e27de236024cbdff83015e0d64b7f7141acd9094`  
		Last Modified: Mon, 27 Nov 2023 23:46:19 GMT  
		Size: 12.2 MB (12150088 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b97d4aa1afd24ba2dfa7087b9b145fdb3c05890badf39fd46a663f14b702bda`  
		Last Modified: Mon, 27 Nov 2023 23:46:17 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e38d1e9a50c971da9c3865c382e3ca5b4cc075d90b80fa5fc430661545edd18`  
		Last Modified: Mon, 27 Nov 2023 23:46:18 GMT  
		Size: 11.2 MB (11151226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e11721c95ac37c34c92cebfc9928ab7108342caad71e37a3a09e6d465b5f45e4`  
		Last Modified: Mon, 27 Nov 2023 23:46:16 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f5620a09123f19c3a88020d84a2acfcc57dd8f6f49dcd2854e0f9ea8ecd3f33`  
		Last Modified: Mon, 27 Nov 2023 23:46:16 GMT  
		Size: 244.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:487dd6665a79a042a6430b97b485713ae2725b6ad7ad497cc6a0eec83806d37a`  
		Last Modified: Mon, 27 Nov 2023 23:46:17 GMT  
		Size: 895.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4305fd90b8fbbd8d34e7500ef211e472a27aa5d9f459be83f39dd9c627521ed7`  
		Last Modified: Tue, 28 Nov 2023 04:02:41 GMT  
		Size: 2.2 MB (2185545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:911ab5edde41c40fd41be21e717254891cfffe1c03f216e363cef704e73d15db`  
		Last Modified: Tue, 28 Nov 2023 04:02:41 GMT  
		Size: 312.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3f6f23f42a781ef65991668a34b7f406111f9992cffec947b2cee6ba570a4b8`  
		Last Modified: Tue, 28 Nov 2023 04:02:41 GMT  
		Size: 705.0 KB (705005 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c694695010c9fd710a977310958870702e53717bb7ac3dc73f4a63c22bac2c2c`  
		Last Modified: Tue, 28 Nov 2023 04:02:41 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:640f9ef3572ee7b5590809dc803c189cf25b03ab6d2e8df6d4d8257cc2a9b444`  
		Last Modified: Tue, 28 Nov 2023 04:02:43 GMT  
		Size: 18.6 MB (18554577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:e73606c9ca1f8a788b3061db791087640c2e8b50fd392ca72a2dace1e22c2f5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6002927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8001ab0f205e82d5e6e4168f9a2261340040b6afb78460a608fedc3be9a66992`

```dockerfile
```

-	Layers:
	-	`sha256:9f9f3c86bed7ee660e0874cbda91a99b2eefb92022659e7145584b3100a3fce4`  
		Last Modified: Tue, 28 Nov 2023 04:28:46 GMT  
		Size: 6.0 MB (5968174 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:c56e06c83942296d61e7781e3fefe60a33338858eb1f6134033a9e7f7dd9a39e`  
		Last Modified: Tue, 28 Nov 2023 04:28:46 GMT  
		Size: 34.8 KB (34753 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:php8.1-apache-bullseye` - linux; 386

```console
$ docker pull drupal@sha256:aad6186c23b2e219b63963244c7cafafb74134038b2487f85c5907e0272bef8e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.7 MB (189670817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3885ee2662d9dbd81464bedef6b216087a9cf0524a584eaa86a2dd3ae3df6372`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 17:45:09 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 01 Nov 2023 17:45:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Nov 2023 17:45:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_VERSION=8.1.25
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.25.tar.xz.asc
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_SHA256=66fdba064aa119b1463a7969571d42f4642690275d8605ab5149bcc5107e2484
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 17:45:09 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 17:45:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 17:45:09 GMT
STOPSIGNAL SIGWINCH
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
EXPOSE 80
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["apache2-foreground"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d0d5ea5604b9d5e6c2327efcf70a55b5b343d4efb21ef7682636424a47f89122`  
		Last Modified: Tue, 21 Nov 2023 14:13:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9e173b0090b614752b3bd03186bedc273001922e0a82892b5757b5574a1a4425`  
		Last Modified: Tue, 21 Nov 2023 14:14:08 GMT  
		Size: 92.7 MB (92724390 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c70549cb086ee59c11e9f8d36cf19fac1d8073b169bc9127df1982ff7a4f510`  
		Last Modified: Tue, 21 Nov 2023 14:13:45 GMT  
		Size: 272.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38f030b6f6639a9b3c6a1074505ddeeaa67a60444f563ecb6aae3deb95a3e9d2`  
		Last Modified: Tue, 21 Nov 2023 14:14:29 GMT  
		Size: 19.7 MB (19745363 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7776c262cb5d6956a7cac217bcb580059ed29b4f47d660bf8f5e13dea14d16b`  
		Last Modified: Tue, 21 Nov 2023 14:14:24 GMT  
		Size: 474.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f670f3cebd80e8fa34c0c681b25a47f54eb403fd511bea894ada7deaa4f25c5`  
		Last Modified: Tue, 21 Nov 2023 14:14:24 GMT  
		Size: 513.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9112a0f7b46b4bf9669eb7e565162ccaa656c8966c8e610a04f46114d670e18e`  
		Last Modified: Tue, 21 Nov 2023 14:26:45 GMT  
		Size: 12.2 MB (12229318 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:387eb8593215fbf710df8ae725d1579477735f020265b98b8447b86638772b2e`  
		Last Modified: Tue, 21 Nov 2023 14:26:41 GMT  
		Size: 495.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:325f4da522b95a154b9c86eb3479e29bed6d925e189ce8644c664b13a83ba474`  
		Last Modified: Tue, 21 Nov 2023 14:26:45 GMT  
		Size: 11.3 MB (11314116 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21bbb6cb78a6f519cd5cbdbf21aa6ce7e6f9742cb4f488621516143f24d73a97`  
		Last Modified: Tue, 21 Nov 2023 14:26:41 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53d315acdc51830d9de2d809cd00a3188493105f51018ce7ec62c2d5c8c2f053`  
		Last Modified: Tue, 21 Nov 2023 14:26:41 GMT  
		Size: 245.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2c1f34824ec187de727234db4d8a190d53b69cbf5b583ea489f5f8ce16c62b6b`  
		Last Modified: Tue, 21 Nov 2023 14:26:41 GMT  
		Size: 895.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fec259d5182b2ba3a7fc85baae145f3f8c17c50938a2dd927d32fe97b29e4016`  
		Last Modified: Tue, 21 Nov 2023 17:31:59 GMT  
		Size: 2.0 MB (1990027 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:13aef2388ad58fcb321595dce150c3d2a058f39acbe304f253ded65a92eb0099`  
		Last Modified: Tue, 21 Nov 2023 17:31:59 GMT  
		Size: 311.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a33479a94bd0319d6c9f57f422512d188bfed7ff187433d858d39f22f7a2d839`  
		Last Modified: Tue, 21 Nov 2023 17:31:59 GMT  
		Size: 705.0 KB (705008 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6aa5d29fcaef1674a01a9f10b62c43a14f91419b8ab6f42c8a3b9cc1a6911c5d`  
		Last Modified: Tue, 21 Nov 2023 17:31:59 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:535f71436e28f2f5e43794277c48a14bffebe392757c72f937706ac4af7cf3b4`  
		Last Modified: Tue, 21 Nov 2023 17:32:00 GMT  
		Size: 18.6 MB (18553960 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:0c5a4389520c2bd4e1285319c12430571a4b105a2a01fa1a297981c17dbf205d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.9 KB (38872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:884bad554e650f77e5d79e18b8c02d54c4f586c1fe3ca85f8565e356644274ad`

```dockerfile
```

-	Layers:
	-	`sha256:7aca7a99d28292c45b1eb4fe56aa8fbaaa3b0350d8ea2dda91a9160eb9f9ea72`  
		Last Modified: Tue, 21 Nov 2023 17:31:55 GMT  
		Size: 38.9 KB (38872 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:php8.1-apache-bullseye` - linux; ppc64le

```console
$ docker pull drupal@sha256:4482523517d2bb1b3bc62f48aa5cab08adecf3b1e32cba8f001825846fbc92fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187098194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a057ec899bb5866c10391712017e181a979ed9d50639416e1fa1bbd75c0ced0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 17:45:09 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 01 Nov 2023 17:45:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Nov 2023 17:45:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_VERSION=8.1.26
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 17:45:09 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 17:45:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 17:45:09 GMT
STOPSIGNAL SIGWINCH
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
EXPOSE 80
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["apache2-foreground"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c773c547f3c0aa5a48c6fdc0bf9f6db649f30bbe51f8daf375233167a64f10d2`  
		Last Modified: Tue, 21 Nov 2023 15:19:28 GMT  
		Size: 225.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aac6a64a4258db247aea2855fa6bd828091c762a0e58c3124dc996c30c18ba13`  
		Last Modified: Tue, 21 Nov 2023 15:19:42 GMT  
		Size: 86.6 MB (86641900 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17ac2fa78b90aba05f0034a35e87616e7518f6c301fab6e4b1613890d37fe258`  
		Last Modified: Tue, 21 Nov 2023 15:19:27 GMT  
		Size: 272.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de7fa080c9b88b1c4f5a1e2df863ee5959df92a489942604eef19cbeb84e2ea9`  
		Last Modified: Tue, 21 Nov 2023 15:20:04 GMT  
		Size: 20.5 MB (20474886 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2bff0fab872b4e553d8e83a67b9e361becf709b9ff03f198075f966b8ed6e7bc`  
		Last Modified: Tue, 21 Nov 2023 15:20:01 GMT  
		Size: 480.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f99af5918931dafd542d3792c914f9c64ee2b2b449e92023bab1dad63e3d5f18`  
		Last Modified: Tue, 21 Nov 2023 15:20:01 GMT  
		Size: 516.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:76746e28a602f01798e7a3a39d3e128193dc147d1e75b5b22fa6385abbc52d12`  
		Last Modified: Mon, 27 Nov 2023 23:59:30 GMT  
		Size: 12.2 MB (12150661 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03471c0d796123947bc3705c8b2fed1f080c9d7df9a5f48b20db953096d9818d`  
		Last Modified: Mon, 27 Nov 2023 23:59:27 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2d4e67359b8c1e291c4a93e9f127daadabb486a21e9b41c1ee2a66562cb0df0`  
		Last Modified: Mon, 27 Nov 2023 23:59:29 GMT  
		Size: 11.5 MB (11484752 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37ed7cb15b5f592a10e12d212e1bb7be4f736a1ac3133293905be1f0b1428374`  
		Last Modified: Mon, 27 Nov 2023 23:59:27 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f61fd0175aafa6adc980703fd65d60cb058784227e8b7fd27657c4f5a76494b`  
		Last Modified: Mon, 27 Nov 2023 23:59:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f4269a1d076e15bc68b2e3df8df1210a1bfb47738a79dbdf3f55b130ac78a129`  
		Last Modified: Mon, 27 Nov 2023 23:59:27 GMT  
		Size: 896.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed45b4e36246d5b269fdbc223f1b2d4c851c0e87cbb46664377dacc035dc0f9d`  
		Last Modified: Tue, 28 Nov 2023 04:41:49 GMT  
		Size: 1.8 MB (1787007 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:44b2d7717f2529d49b16866611e657940e5e83526f93cd100921c68cea2cee63`  
		Last Modified: Tue, 28 Nov 2023 04:41:49 GMT  
		Size: 313.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:03f3438c6ce4e72fa4e8c3c8502225eb948108132ab511cac1637319903d77b4`  
		Last Modified: Tue, 28 Nov 2023 05:00:01 GMT  
		Size: 705.0 KB (705006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:984b6253f0d880ecd9fcb73a29a014cad08d5d774bd1eed9477f4de9dbbd1edd`  
		Last Modified: Tue, 28 Nov 2023 05:00:01 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d5b2371830d1ad9df598c5e00065e9158850c4fd82a59e0bc415b433f38c5007`  
		Last Modified: Tue, 28 Nov 2023 05:00:02 GMT  
		Size: 18.6 MB (18554238 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:bcfd020688e42a494c5b3b171586f9b8786f7e5413a52a35cade0ed9777a2b29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5972152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df352279abf804f6d1c84ed9656333f775c26fca5ddcf834da046184757cc2b7`

```dockerfile
```

-	Layers:
	-	`sha256:8788f1eced2275513ca8c9fea1e4565f4462756697118000311d6d9359d853e9`  
		Last Modified: Tue, 28 Nov 2023 05:00:01 GMT  
		Size: 5.9 MB (5937363 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0894ea65df8285b84ca51a91b6cbd86e65b07eaa34bc5c7330001833dadef66a`  
		Last Modified: Tue, 28 Nov 2023 05:00:00 GMT  
		Size: 34.8 KB (34789 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:php8.1-apache-bullseye` - linux; s390x

```console
$ docker pull drupal@sha256:fb569e712cd2ee0efd7cad70c06a44af8a7750f4efa35bd15b0483d515ff723c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.5 MB (163515936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea27597c61f5072a937718c6fd07ff35431f6f07af9b56a82a654ab324eda0d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 17:45:09 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 01 Nov 2023 17:45:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 01 Nov 2023 17:45:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Nov 2023 17:45:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_VERSION=8.1.26
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 17:45:09 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 17:45:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 17:45:09 GMT
STOPSIGNAL SIGWINCH
# Wed, 01 Nov 2023 17:45:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 17:45:09 GMT
EXPOSE 80
# Wed, 01 Nov 2023 17:45:09 GMT
CMD ["apache2-foreground"]
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV DRUPAL_VERSION=10.1.6
# Wed, 01 Nov 2023 17:45:09 GMT
WORKDIR /opt/drupal
# Wed, 01 Nov 2023 17:45:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 01 Nov 2023 17:45:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:476bca1ea6c08be1ec94ee496638c7817fc00e1abf5e7632dade763277d2de21`  
		Last Modified: Tue, 21 Nov 2023 12:27:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c47ec361932640295dd75780322a98f75f70e435f8f56b05b58b400867dc3f1`  
		Last Modified: Tue, 21 Nov 2023 12:27:21 GMT  
		Size: 71.6 MB (71634805 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8cb940181fc77e81f32c4d45baf6dde8b85e0042b5cd72f62eba874d80045ec3`  
		Last Modified: Tue, 21 Nov 2023 12:27:11 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2553cb36f5fea2add77a1fbef961dee3ef80b510860b1ba9404497a9fd32cd6b`  
		Last Modified: Tue, 21 Nov 2023 12:27:33 GMT  
		Size: 19.1 MB (19080552 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:23daf5f61d8cbed800e6a5f5435cdc61ec12ca276e3c300fc4b02f04d6c01363`  
		Last Modified: Tue, 21 Nov 2023 12:27:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96a1471d871a3bd567cd588f3e5122b5983df3cd2e990caa6146e7995e0d9781`  
		Last Modified: Tue, 21 Nov 2023 12:27:31 GMT  
		Size: 510.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be5444c9a5de1486522e9e0b5a7ca35b580b1aaae661f2d3187e1f6ea660f159`  
		Last Modified: Mon, 27 Nov 2023 23:33:06 GMT  
		Size: 12.1 MB (12149757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:53948f62e5bc8922a044e1e5b8a420a64637e75ed529bf7c307c9c3b871481e4`  
		Last Modified: Mon, 27 Nov 2023 23:33:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8292ec73377d86da52c98cb20246604c793daaf106b0a105e81cb38466458739`  
		Last Modified: Mon, 27 Nov 2023 23:33:06 GMT  
		Size: 10.2 MB (10215751 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:67a08ce169e0f65af4613fe3b9810b1805b4aaeb0899b7f754a3ca171ef417ee`  
		Last Modified: Mon, 27 Nov 2023 23:33:04 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9b7724b1357f3c9eb2ea2e74fa8eb20d3c290e5af4d81d2bd326bbc0d3a9225e`  
		Last Modified: Mon, 27 Nov 2023 23:33:04 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ca95da3471f4d0a963661c7dc976de826a5c5c009702988c52b4ad6e3277c05`  
		Last Modified: Mon, 27 Nov 2023 23:33:04 GMT  
		Size: 896.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:274ad468ef319c55667ccf4223691722167d910295c6f754be82c01fc659d57a`  
		Last Modified: Tue, 28 Nov 2023 01:58:15 GMT  
		Size: 1.5 MB (1513018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37b8f6ab23ef7490c23cd76cc5c363b4bddb31ea209158325da85f6db6e1d935`  
		Last Modified: Tue, 28 Nov 2023 01:58:15 GMT  
		Size: 313.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c831662dad587b6a9bf9f665f1f37e5656d1287aa85fcc1cfdf410411035ff82`  
		Last Modified: Tue, 28 Nov 2023 01:58:15 GMT  
		Size: 705.0 KB (705002 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64f61ee35484a411911dc5a858f9e131a8d641aefe4d1ab96a556b219448e98e`  
		Last Modified: Tue, 28 Nov 2023 01:58:15 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27f9526ddb5b2708f5a492bb373649b03ac26e974e7fd51c62fd827dcd871b44`  
		Last Modified: Tue, 28 Nov 2023 01:58:16 GMT  
		Size: 18.6 MB (18554110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache-bullseye` - unknown; unknown

```console
$ docker pull drupal@sha256:25376890974b06ee3144afc0dcef8ac512ac4291bb80aa79bd45e6c164610b55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5854460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b2cad231a8977a47573acbfda41a807335ac943fcb99e0f1233eed007e5e18`

```dockerfile
```

-	Layers:
	-	`sha256:5b9d595c6601649a5e5a369d0785bdc3564f9c14e3ea070650e95c662fc086e9`  
		Last Modified: Tue, 28 Nov 2023 01:58:13 GMT  
		Size: 5.8 MB (5817609 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:01187d87c6475604018fd54edc900f90f5ad728a46f55a621af506ff8e7ad4de`  
		Last Modified: Tue, 28 Nov 2023 01:58:13 GMT  
		Size: 36.9 KB (36851 bytes)  
		MIME: application/vnd.in-toto+json
