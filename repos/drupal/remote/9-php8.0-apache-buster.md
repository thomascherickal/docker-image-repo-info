## `drupal:9-php8.0-apache-buster`

```console
$ docker pull drupal@sha256:da1c4d1ad466de7c41a4b59d762c9a98533e603aeb3e992e6480af53cee09d95
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown

### `drupal:9-php8.0-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:6d26d5368811b9acd9a0534503b4cd9e6b083181fe111842034714656a972ea8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170096644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835a10cb3d2cc534e5b9563abb2b56b9cc5a52888115b9438004bbb432bccd2d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 22:07:44 GMT
ADD file:7672eb709be933bb0edec47b8141cd2ebff266a770dfae1278205f7cee43c71a in / 
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 22:07:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 22:07:44 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 80
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:0fc9206bc4affb32fe13185a20b8184271c753e9b7cb81484bf770054fc69737`  
		Last Modified: Tue, 21 Nov 2023 05:27:19 GMT  
		Size: 27.2 MB (27187457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bed65b9e29f233decd32bcd9a254eaf55bd0629cd15c3b194812fe0d2c19d3f2`  
		Last Modified: Tue, 21 Nov 2023 16:51:13 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a44acfee715f069e498c6da70604e05beacf650dce5eb7569011ab306526311`  
		Last Modified: Tue, 21 Nov 2023 16:51:23 GMT  
		Size: 76.7 MB (76700232 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7893973ff1ce152c4b384b60cd6be9b6a01f9f0b7c863c2c9f5ce902947b5aad`  
		Last Modified: Tue, 21 Nov 2023 16:51:12 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7062932f2f01a9fae37b8a206940483bacc83b65c31374170197b13e3c25a5f6`  
		Last Modified: Tue, 21 Nov 2023 16:51:42 GMT  
		Size: 18.7 MB (18690018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e66ff722ee714b347a34beb39035c32211ef7aff591463320700fa5a23a68d6`  
		Last Modified: Tue, 21 Nov 2023 16:51:39 GMT  
		Size: 471.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4b7c00f2f09021ae5d567885d28f7cbc06f37f39d111723ecb6a08307b3e8df1`  
		Last Modified: Tue, 21 Nov 2023 16:51:39 GMT  
		Size: 512.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:84f6a8dc7d4a02f14efa75de6ef202e15afe1b4b0e2a5dcca6169b3c19954f74`  
		Last Modified: Tue, 21 Nov 2023 16:51:40 GMT  
		Size: 11.2 MB (11160914 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a19d1114b376722b3cd311a2d7dd9406744a4933afb7bf8eb5db1c7e7df1fbcc`  
		Last Modified: Tue, 21 Nov 2023 16:51:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59b3d407f1e33a2b6f2f08ca8944855f1204b7ac26e8b0dbd8ea0000b6df75b9`  
		Last Modified: Tue, 21 Nov 2023 16:51:39 GMT  
		Size: 10.7 MB (10734874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7488943c2ea3e53288d93677ef3a197990c6ba73508af69610d9ee43fa88d3a1`  
		Last Modified: Tue, 21 Nov 2023 16:51:37 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:66d64067209824f61a11291e422bf1371f710c40f07f58517e94e9e2fcd46fae`  
		Last Modified: Tue, 21 Nov 2023 16:51:37 GMT  
		Size: 244.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73ed246496631a684a79aaf1517f4161de16788ff41da7d296cf7ec62ed9d7ee`  
		Last Modified: Tue, 21 Nov 2023 16:51:37 GMT  
		Size: 895.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fd7f22e504c8e615ff5161c80e330794be2370b70d1c63a53fa12409d22caec`  
		Last Modified: Tue, 21 Nov 2023 21:05:19 GMT  
		Size: 2.0 MB (2033751 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3eac7381e4d971f3bedb1198d89fc6c62ff9bd289e13025d4684f299635d61f0`  
		Last Modified: Tue, 21 Nov 2023 21:05:19 GMT  
		Size: 313.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:10aefbdc33e43bbee4ef048714ad55104ac97d587b218d935ef841e40b1efd6e`  
		Last Modified: Tue, 21 Nov 2023 21:05:19 GMT  
		Size: 705.0 KB (705010 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a892609e78777e58e0d53a489b69525d61384a99f1f78588d729b80ada338d74`  
		Last Modified: Tue, 21 Nov 2023 21:05:19 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1096e7b2b37b64eaf58b274a4d2a5399806a453b5cd2476e535b655ca0473aa3`  
		Last Modified: Tue, 21 Nov 2023 21:05:20 GMT  
		Size: 22.9 MB (22878391 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.0-apache-buster` - unknown; unknown

```console
$ docker pull drupal@sha256:e6013aba8149ab58a096e127965deabb618d69b372a20d806423d91fd40615ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5619471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f4b8f058ec327f9879ec653e135dde8467935ef3174ee7cf7f252c12261bdd6`

```dockerfile
```

-	Layers:
	-	`sha256:4cc2b9522901d50bc6ff0858f8291ee5bf3d7de4a10f1556d0ec76e868e6b25c`  
		Last Modified: Tue, 21 Nov 2023 21:05:19 GMT  
		Size: 5.6 MB (5580590 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:804edcd7438d63dee9ba423a3196343cfc1f54c3caebe2c335e4bb2b9b132814`  
		Last Modified: Tue, 21 Nov 2023 21:05:19 GMT  
		Size: 38.9 KB (38881 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.0-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:9340153f716560a425e4f350dce8b9fd271f5eefa2f574249bc74a1423d5c598
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.3 MB (145253279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32cb53ea7d0f8241f722036770fdf53a628f5877f5d8704bc4704465b47f3d63`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 22:07:44 GMT
ADD file:407ef80699946b8a8560ae436dfc9ca6148067b3012c02b4cb4e54d6d0aca674 in / 
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 22:07:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 22:07:44 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 80
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:d0b016a8027330736e9ca5c23b846a6a9c1eb0a32da6459047c95d22e9544cb7`  
		Last Modified: Tue, 21 Nov 2023 04:03:19 GMT  
		Size: 22.8 MB (22795884 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16cf628769b7921f1260cc18c491a08f2d49c3a806076bb7c6f89e1ff0015c38`  
		Last Modified: Tue, 21 Nov 2023 11:06:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a171157a85e1165ddeaa15261ef3b4492563893ccebeff15342d6edab1db4670`  
		Last Modified: Tue, 21 Nov 2023 11:06:42 GMT  
		Size: 59.5 MB (59544686 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87e91a567560ec1519ba85f8011d1ed158ac42ff5ade112b1f51aa3464df5df7`  
		Last Modified: Tue, 21 Nov 2023 11:06:31 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d25bc1b544a7a6aa429013ea83ce22434ea603189dd604f086b6ecae8f110403`  
		Last Modified: Tue, 21 Nov 2023 11:07:02 GMT  
		Size: 17.5 MB (17482200 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14116c1eae2395c888fc617a64858d494e2b83b04344a4fd8dd878aa8d6c3aaa`  
		Last Modified: Tue, 21 Nov 2023 11:06:59 GMT  
		Size: 473.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d1628012c058ab558ea3399b9dd5a0d02f3622032b21f34354be1e304021cf13`  
		Last Modified: Tue, 21 Nov 2023 11:06:59 GMT  
		Size: 512.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7cf030e1d19b42f68179c5457ee5d7f01b6e533fd772dfaa7d15e057c151042e`  
		Last Modified: Tue, 21 Nov 2023 11:07:00 GMT  
		Size: 11.2 MB (11158987 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a0f088a39184436f37a8c2963020fdbcedc85a2f7b60616efc5b48821cdcb65`  
		Last Modified: Tue, 21 Nov 2023 11:06:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2419c32c8b315348bf3f11455e7b3faa5c31e9185b6cf5ec2fa8cdeb4e919089`  
		Last Modified: Tue, 21 Nov 2023 11:07:00 GMT  
		Size: 9.3 MB (9262610 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e3a67a0b930d66ed29c31ce5e245630bc914b62f7cb5e5584fdd4b9cb394fde4`  
		Last Modified: Tue, 21 Nov 2023 11:06:57 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f4a5a6e66c34e0727dbaf622112ca2602366cb3a888451789984fdb0467cbd10`  
		Last Modified: Tue, 21 Nov 2023 11:06:57 GMT  
		Size: 243.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b84d1e29652b765a7bbe2505e10d0346dbea97e27c9f8145c46a06fbbb78c6fe`  
		Last Modified: Tue, 21 Nov 2023 11:06:57 GMT  
		Size: 892.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3125e919fc6f56248960485ea23915dfd6341ae588386203e95312846181c093`  
		Last Modified: Wed, 22 Nov 2023 00:36:47 GMT  
		Size: 1.4 MB (1419438 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:332378c90851aa81c34f7348c410a6730b0e5e5ed6ca08dc92bb3ee6071f7ee4`  
		Last Modified: Wed, 22 Nov 2023 00:36:45 GMT  
		Size: 312.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab4254a3d915d13d77a4e0a58cad57c6b1d9a5b0ee981bd08b7955193e1637e1`  
		Last Modified: Wed, 22 Nov 2023 00:36:46 GMT  
		Size: 705.0 KB (705003 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:40b0b22eb7be1c34b58b4ca4ba6f5fd1ca5d1458d06e93653bb574a258df1554`  
		Last Modified: Wed, 22 Nov 2023 00:36:47 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cee63172a1e626cb719c032832b13f94ba7ae5b07e030da694e0981bd1c0c9d2`  
		Last Modified: Wed, 22 Nov 2023 00:36:48 GMT  
		Size: 22.9 MB (22878476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.0-apache-buster` - unknown; unknown

```console
$ docker pull drupal@sha256:d263922b4b3539d93ea647fecfaa54457f4d73b1c7946487155ea449eaf33541
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5449482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec0c1e5321ca22f6e0f6349053c30a8eecc0e27dcc64e204d83edc847bc1df2`

```dockerfile
```

-	Layers:
	-	`sha256:1cc27ce82c22df30bff872d8cfeb70badfc69a4d88b0fc4556b2058513619276`  
		Last Modified: Wed, 22 Nov 2023 00:36:42 GMT  
		Size: 5.4 MB (5412775 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d3db86ac5f2448bbccdfcfc7e6c520bbfab991384a14bcc4df843e4c5bab1d3d`  
		Last Modified: Wed, 22 Nov 2023 00:36:41 GMT  
		Size: 36.7 KB (36707 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.0-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:2602738a179ad8c8b3142aa120bab6d96f5293cb78efc2b5ea31f16efb8d4cfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161573044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6da5038d04aa8b042fa264a19b1a0eaf78142baff690d5b859c5a3040682079`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 22:07:44 GMT
ADD file:475e94b9a8f65c7cd4d4156af31e83190240ff35d8038f3fa86ad124d4d5d299 in / 
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 22:07:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 22:07:44 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 80
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:78b429e3efdd9f2b163abf0bca6b1462a25b1c5eddc1dd47f5d3445c6413cfa1`  
		Last Modified: Tue, 21 Nov 2023 06:31:45 GMT  
		Size: 26.0 MB (25967796 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ac5ea5ac4eb4dbb61d3da80b1818bb26fbf377e92053ec3f0f73bf5814bda32`  
		Last Modified: Tue, 21 Nov 2023 16:50:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4aba9cbdbe83fb73c9173931869e1a6f54d9e032cd8ff6d535267d2b41659fd4`  
		Last Modified: Tue, 21 Nov 2023 16:50:26 GMT  
		Size: 70.4 MB (70369692 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3d9e020beea91ef46539185b02cac49a9428322089f920897583f5bdae6bbccf`  
		Last Modified: Tue, 21 Nov 2023 16:50:19 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dcbd95c4954e2f58fbbd6a487828e5545fa4bd8ad849c139665927c486b2a8e2`  
		Last Modified: Tue, 21 Nov 2023 16:50:44 GMT  
		Size: 18.6 MB (18587164 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ea7c2d322729cd897f4ff4ef01fb26184b39c336de439483fd6d65d1f8bfe2d`  
		Last Modified: Tue, 21 Nov 2023 16:50:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:253647ea53161431e3ac0e1163d583af59c7060469974be339b09d0405500a64`  
		Last Modified: Tue, 21 Nov 2023 16:50:42 GMT  
		Size: 513.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:85ddb0cabec18ed514a24aa19b44b416d5f7083b33457896fc4d5eda3aa10a3c`  
		Last Modified: Tue, 21 Nov 2023 16:50:43 GMT  
		Size: 11.2 MB (11159731 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e4f7ba60c28ee3a8346e778a7417d04533e0ebaface2acc0c644f4261c4fa6f4`  
		Last Modified: Tue, 21 Nov 2023 16:50:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cfc784a3fbc75521ece2385ba2cfa3365af5663aab9eb8504328b0aa14104837`  
		Last Modified: Tue, 21 Nov 2023 16:50:41 GMT  
		Size: 10.2 MB (10211952 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6049d3351ca1443607f533b737652b4ca0ba952906fab6f800b731031c8a2d6e`  
		Last Modified: Tue, 21 Nov 2023 16:50:40 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:645523c28aebe38b5f1fa6174d59281f91ea1df8f9ddf652d3778f4733ead078`  
		Last Modified: Tue, 21 Nov 2023 16:50:40 GMT  
		Size: 245.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:970888150889049cf18856a45af335775ca854ada90cf51086360c0ee86fded5`  
		Last Modified: Tue, 21 Nov 2023 16:50:40 GMT  
		Size: 895.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1b9b8daf304e3b210afb3e85598a3b7a3e65243dc12fbd4a9499177013444a5`  
		Last Modified: Wed, 22 Nov 2023 06:17:31 GMT  
		Size: 1.7 MB (1687307 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:31d585cf2d485a2dc0512438bf244901888315db7b9e09b8d3b64c0a1e9da66e`  
		Last Modified: Wed, 22 Nov 2023 06:17:31 GMT  
		Size: 313.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65251945cc361e25c72db7bd95b930131054913e74b3445df9c0c70a52cdd2d7`  
		Last Modified: Wed, 22 Nov 2023 06:17:31 GMT  
		Size: 705.0 KB (705008 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04e6126371d96c8d57c998eb7581b0217a3ac8d42b6b6c6eee8533bed5fdb293`  
		Last Modified: Wed, 22 Nov 2023 06:17:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f4ec7f1b6ba370c8068d6965554663d4631dc35e4bb24ef960db16355e1d6a1`  
		Last Modified: Wed, 22 Nov 2023 06:17:33 GMT  
		Size: 22.9 MB (22878388 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.0-apache-buster` - unknown; unknown

```console
$ docker pull drupal@sha256:8f7e8c7b4fa965a7b2519d5bd1a228ce3b140cb87e7539f505e0facc218e0bc1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.6 MB (5609519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28d3ac10ed63d5768fb6eee4b6a813b380aef9f9f6e550f1ad0cac466bd601c7`

```dockerfile
```

-	Layers:
	-	`sha256:513127fdd1b89de032e7b60d9654902dfab53b3410fa13fbb4032aa56e0fa661`  
		Last Modified: Wed, 22 Nov 2023 06:17:27 GMT  
		Size: 5.6 MB (5572901 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3f4c6ee2fb73b03225f832d2387e3cef391e092974bd2ddba98b5f845e3936a8`  
		Last Modified: Wed, 22 Nov 2023 06:17:26 GMT  
		Size: 36.6 KB (36618 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:9-php8.0-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:e2c7a4a3a709c890c27833084b5b21bbfceeb13b79bbddb32f3303a570a302bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.0 MB (175998831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc2173d76b0edbc5afa35f127d31dc47cd7247f32e71bb05b4ce1bfc9e44956a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 22:07:44 GMT
ADD file:a04f70df2aa61b210935e80ad2a655ad282407ef0b8e8e0acf47479c73f64f95 in / 
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 22:07:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 22:07:44 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 22:07:44 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 22:07:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 22:07:44 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 22:07:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 22:07:44 GMT
EXPOSE 80
# Wed, 20 Sep 2023 22:07:44 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/* # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
COPY /usr/bin/composer /usr/local/bin/ # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV DRUPAL_VERSION=9.5.11
# Wed, 20 Sep 2023 22:07:44 GMT
WORKDIR /opt/drupal
# Wed, 20 Sep 2023 22:07:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME" # buildkit
# Wed, 20 Sep 2023 22:07:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:071d917b80792914c4da1ecc1adf7e2503440a8c7a2a5508542e0850d9187060`  
		Last Modified: Tue, 21 Nov 2023 04:46:12 GMT  
		Size: 27.8 MB (27846916 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:08a9e9dc1bc76ac3ef594e946c5f5eab2131263a9bbe23e76b33c6784e98fa61`  
		Last Modified: Tue, 21 Nov 2023 14:29:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3df649b388c6ba6ed91483f65f5943d2b2e68e1f86fbed801a8ac87413b70769`  
		Last Modified: Tue, 21 Nov 2023 14:29:19 GMT  
		Size: 81.2 MB (81237776 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b019be63e0c212b9074a709b3173019138375a4a79cd80cc21818c12a58b5c2`  
		Last Modified: Tue, 21 Nov 2023 14:29:01 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbcb6ca8c3ad2b3e24da4fb98982dcb44d953da00d11181d3ed20de5da28a7ac`  
		Last Modified: Tue, 21 Nov 2023 14:29:39 GMT  
		Size: 19.1 MB (19117622 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8a7119d0ac318254b2555e0606ac15a599eda903e1b5550eb8592bcb5cd70d64`  
		Last Modified: Tue, 21 Nov 2023 14:29:35 GMT  
		Size: 474.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fedd0805eb3f60cf0b9598a4336c37195dd6454e4661c358191de17cc1a39def`  
		Last Modified: Tue, 21 Nov 2023 14:29:34 GMT  
		Size: 513.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cd77312800b6ff0c83836b7ff36903912b36728d0a10f3dd792a9da4324d8251`  
		Last Modified: Tue, 21 Nov 2023 14:29:36 GMT  
		Size: 11.2 MB (11160273 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19d500539fd6aa7d2f8292f8917a5299c90292f7cacf2c7107fb7246d5727c09`  
		Last Modified: Tue, 21 Nov 2023 14:29:33 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bdfb96f60afff75561c34e132ff622ce947e51d620f88bf434452f60b426f52a`  
		Last Modified: Tue, 21 Nov 2023 14:29:36 GMT  
		Size: 10.9 MB (10943625 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89b4c46cebc06f1919841ea6a924f16ee768a2b4c4c8368ea39a44237e01fe64`  
		Last Modified: Tue, 21 Nov 2023 14:29:33 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48890416eb35d7085f87bef3e096d521304ee517798517a0da82092bc156f4ca`  
		Last Modified: Tue, 21 Nov 2023 14:29:33 GMT  
		Size: 248.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7100daf6f6441ec7f42846e4157a9be97734047ab202da0c3ad0f59213cab024`  
		Last Modified: Tue, 21 Nov 2023 14:29:33 GMT  
		Size: 894.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed5b20fd492b6344090ef42a8a350d69167b79fe098a8591c6f3c99d4fce0baa`  
		Last Modified: Tue, 21 Nov 2023 17:32:18 GMT  
		Size: 2.1 MB (2102881 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f4de9ce2b85e0ff655f2f9d7fbc5e1833b1a631a9ad078f6e1581ec9a92694e0`  
		Last Modified: Tue, 21 Nov 2023 17:32:17 GMT  
		Size: 315.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:014b71157d662bab04d3f74430357c791079f9506dec7219dc9e18b114223db7`  
		Last Modified: Tue, 21 Nov 2023 17:32:18 GMT  
		Size: 705.0 KB (705008 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:26b2ed8a225a580c2a8b307714959603e98851876efa99318c52b94457d8a51a`  
		Last Modified: Tue, 21 Nov 2023 17:32:18 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a1e26a997f781a30090e9ee3f8205acd05d8d9017bd2e3e4eb26e17050b8703b`  
		Last Modified: Tue, 21 Nov 2023 17:32:20 GMT  
		Size: 22.9 MB (22878721 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:9-php8.0-apache-buster` - unknown; unknown

```console
$ docker pull drupal@sha256:4c4c921fd4c128c4a904be41852640475d144d6135b76164f1a1235190936ac6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 KB (38636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:676a3dfb45da7c3071cb2b5b85ce4ae2706ab1e1186a38f316409173f9852c6a`

```dockerfile
```

-	Layers:
	-	`sha256:309bc878a40ae5990d115cea9ac6c98f30818dfcf9edf7110b6591eea9503229`  
		Last Modified: Tue, 21 Nov 2023 17:32:17 GMT  
		Size: 38.6 KB (38636 bytes)  
		MIME: application/vnd.in-toto+json
