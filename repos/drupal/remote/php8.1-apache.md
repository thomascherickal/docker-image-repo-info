## `drupal:php8.1-apache`

```console
$ docker pull drupal@sha256:16e609c9239b09e53faca94e50ca514d4f0fe7c12372218fe80a8fbb1d8c44cf
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

### `drupal:php8.1-apache` - linux; amd64

```console
$ docker pull drupal@sha256:278af94bd3c6ad0219dae27ba8bfa68178409e1c007d819b445eceee1e0f1968
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.4 MB (198446193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd78b99759e367d33398d50f34035dfe54be797163b80c502421cadde74ad52a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:49 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 01 Nov 2023 00:20:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 05:16:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Nov 2023 05:16:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Nov 2023 05:16:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 05:16:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Nov 2023 05:16:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 01 Nov 2023 05:20:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 01 Nov 2023 05:20:41 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 01 Nov 2023 05:20:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 01 Nov 2023 05:20:50 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 01 Nov 2023 05:20:51 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 01 Nov 2023 05:20:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 05:20:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 05:20:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Nov 2023 06:18:01 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Nov 2023 06:18:01 GMT
ENV PHP_VERSION=8.1.25
# Wed, 01 Nov 2023 06:18:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.25.tar.xz.asc
# Wed, 01 Nov 2023 06:18:01 GMT
ENV PHP_SHA256=66fdba064aa119b1463a7969571d42f4642690275d8605ab5149bcc5107e2484
# Wed, 01 Nov 2023 06:18:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Nov 2023 06:18:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:21:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 06:21:42 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:21:42 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 06:21:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 06:21:42 GMT
STOPSIGNAL SIGWINCH
# Wed, 01 Nov 2023 06:21:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 01 Nov 2023 06:21:43 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 06:21:43 GMT
EXPOSE 80
# Wed, 01 Nov 2023 06:21:43 GMT
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
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c053f6f43c122d10a9ed41f0b4fee4f12737d55a220a275d58bd89a57754e3fb`  
		Last Modified: Wed, 01 Nov 2023 07:10:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65cebbf4d847e8ee87513e58c95b420844aff691e0d07e4a6d76246c9e0c685d`  
		Last Modified: Wed, 01 Nov 2023 07:10:24 GMT  
		Size: 104.4 MB (104353572 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:34045bc939601f7e76df95a46ca7bf42e99dcdb879b149a6c705a8924a707d9a`  
		Last Modified: Wed, 01 Nov 2023 07:10:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da31f94fbeef57a5035b3f90c4128531c28059dc206c1ede76a6bdbea6089c8a`  
		Last Modified: Wed, 01 Nov 2023 07:10:53 GMT  
		Size: 20.3 MB (20305084 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c755cb948935c20aca0d800bd380ee8d1f6a354a22ebe9bcc932a77fd647e022`  
		Last Modified: Wed, 01 Nov 2023 07:10:49 GMT  
		Size: 479.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47863fce0cd3df8ca85ef1300f854bd99373bd00d3a30be040e074a7cd1fb7b3`  
		Last Modified: Wed, 01 Nov 2023 07:10:49 GMT  
		Size: 515.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d84c2648afeaad07738ac591ab7f29aba7886a4430abd3fd44325ac16fc358d5`  
		Last Modified: Wed, 01 Nov 2023 07:17:01 GMT  
		Size: 12.2 MB (12222897 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:021a1d0b43dbc7c36e745daad769bbb21c53bb8ea6faa5f0eb229549561d9fb1`  
		Last Modified: Wed, 01 Nov 2023 07:16:57 GMT  
		Size: 494.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47c9a3d76b0577f5868da977debce325a64281dfce5ea4253389582f7985b7eb`  
		Last Modified: Wed, 01 Nov 2023 07:16:59 GMT  
		Size: 11.2 MB (11154619 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:592bacd8742dc7b93c2540b54e93685551a535bc951f1f9e0fb56f7b5c7719c1`  
		Last Modified: Wed, 01 Nov 2023 07:16:57 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3ff649b14feddd2cefc8c205d6da9106747398855ca19bb461fdf7139bf90d06`  
		Last Modified: Wed, 01 Nov 2023 07:16:58 GMT  
		Size: 246.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71cde5c5aca723320843cbaf87a7fe055a777f8db6f70bb07771ad6b8d7ab22b`  
		Last Modified: Wed, 01 Nov 2023 07:16:57 GMT  
		Size: 896.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f53499921b09b762feeeb07606a6606f9888dcdee30eb5b72d236dfb270c4593`  
		Last Modified: Wed, 08 Nov 2023 20:23:55 GMT  
		Size: 2.0 MB (1995239 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:24fb4ed4b92d941a68a8ef7c9273d981765c63f7ee925f37bfbe4ab29f4b9fd6`  
		Last Modified: Wed, 08 Nov 2023 20:23:55 GMT  
		Size: 317.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ffb936b76321a438056fea4b85d9d4b8f50c485a7acbd1d94a28354959345ab4`  
		Last Modified: Wed, 08 Nov 2023 20:23:55 GMT  
		Size: 705.0 KB (705006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5059addf276e13f6e4a372794d450e1d32d442648deebfb7e77151d82f9fe51`  
		Last Modified: Wed, 08 Nov 2023 20:23:56 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:349e0544ec40026c45762e9090c99d8ea7a0f6143cd1be98e4fa6991f3407b2d`  
		Last Modified: Wed, 08 Nov 2023 20:23:57 GMT  
		Size: 18.6 MB (18553921 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache` - unknown; unknown

```console
$ docker pull drupal@sha256:b5ad4b03ff4434585f592f8a15a1efa954ebd35a30e658ff9dc625a9961f90d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5954014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0111e36c132eff0296eb22aeca3b2e16822bbdb6dbebb3bdb1158b9cc99338`

```dockerfile
```

-	Layers:
	-	`sha256:a65446a672da0e7444458c0f96a5e5c8dee5f71fe1771fa4a80e53bf3ffdecb4`  
		Last Modified: Wed, 08 Nov 2023 20:23:51 GMT  
		Size: 5.9 MB (5912383 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d448ce908d2c8d459aa06eaa1cd12a5b55e78f271efddc1547996e0841c6345`  
		Last Modified: Wed, 08 Nov 2023 20:23:51 GMT  
		Size: 41.6 KB (41631 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:php8.1-apache` - linux; arm variant v7

```console
$ docker pull drupal@sha256:90afd78d71bb3f0fb190c41f06aabb03d980b3fc763547785ef32e1326a2844f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.4 MB (162431159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f009e92326859d29aa4e5c7506d8ac9eea6dbc2bfbe362455c36f071891e2753`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 17:45:09 GMT
ADD file:b693944382a95fa47622fde77eb98f0cdeafa40261e7334bd355e00f650b6632 in / 
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
	-	`sha256:b4ce590529bbcf84326048a22fce76fcfcb5c60af5519debd7935a74c1e9126e`  
		Last Modified: Tue, 21 Nov 2023 04:01:50 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:14c1c4147c53597e5b07cc3da6a4f2bc1153b627dbf415b2b595b2b6433ace84`  
		Last Modified: Tue, 21 Nov 2023 10:50:48 GMT  
		Size: 228.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ccd91a599fb4e546a1b11496c7cde449b0a62782471ca6b57c7ccd447c465ff`  
		Last Modified: Tue, 21 Nov 2023 10:51:04 GMT  
		Size: 76.2 MB (76225648 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f28aecabad1653a96793880791ff49eaacb2fcb0b9498620f8bc5a9f4e2d4c67`  
		Last Modified: Tue, 21 Nov 2023 10:50:48 GMT  
		Size: 274.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bdd22fd75afd798303c122a7847b5a3dd3d553fc6308430df3331c76f5c27884`  
		Last Modified: Tue, 21 Nov 2023 10:51:32 GMT  
		Size: 19.0 MB (19046541 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0b37c46693beec8e40b5ca3291b55d05bf05c91bfa505abf03f1ae41aa7312d`  
		Last Modified: Tue, 21 Nov 2023 10:51:29 GMT  
		Size: 476.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a8e1883ef04ccbbb0af337e641a9d7fc88368c310238fa8d58e40e58166091`  
		Last Modified: Tue, 21 Nov 2023 10:51:29 GMT  
		Size: 514.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27f5ae91e3669bfd83935a1a785dc6b12236e54d829f9f5d8e02886b1a785877`  
		Last Modified: Tue, 21 Nov 2023 11:03:07 GMT  
		Size: 12.2 MB (12220890 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e6db5f8903bb23368cc222a30ae9d019161ae69aafd7ff166336bcfe5b913a5`  
		Last Modified: Tue, 21 Nov 2023 11:03:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc028b07d5c1b5c7d0f5f806610534a2f0cb4358bca1014594f32df2da4d750a`  
		Last Modified: Tue, 21 Nov 2023 11:03:07 GMT  
		Size: 9.6 MB (9579496 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2855f1e2bf175f3cf47a5b83725c538e567b2ed7d343a9bbc00c374a7adf75ed`  
		Last Modified: Tue, 21 Nov 2023 11:03:05 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0b3d720fd114963c282900f4801ffadf3168c6cc2327267c2533959eda2b52e`  
		Last Modified: Tue, 21 Nov 2023 11:03:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d5ea85571b19c19afde5804265cc3f1749fce2e49b0a54d5b2046b4d1ca152b`  
		Last Modified: Tue, 21 Nov 2023 11:03:05 GMT  
		Size: 896.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d6bcb6f9721888e0c89d4266f5e5eed259171a2e2f4588fd7ad609d9a49a9159`  
		Last Modified: Wed, 22 Nov 2023 00:09:01 GMT  
		Size: 1.3 MB (1344478 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9fa99c2880e24f575ed8575bfea7cb3bed16da23032a3cc0b6b0b170f1ff78ab`  
		Last Modified: Wed, 22 Nov 2023 00:09:01 GMT  
		Size: 314.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9036f0a3bb10c884b6962bcdd619e339bff34aaf8dc7e3147ae6a41982b89ff`  
		Last Modified: Wed, 22 Nov 2023 00:09:02 GMT  
		Size: 705.0 KB (705006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cab7e8e2e75a9faeaadb0b2998151759510837bc30df09b40cf5fb5bd9b8d442`  
		Last Modified: Wed, 22 Nov 2023 00:09:02 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e9a98afeb75f32a504213b2064112e38cbf1d137537bb71fecb532a107ecb7af`  
		Last Modified: Wed, 22 Nov 2023 00:09:04 GMT  
		Size: 18.6 MB (18554161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache` - unknown; unknown

```console
$ docker pull drupal@sha256:072518e745d63ab8e77ed5e6c1f3da79f6780e80738415d74554f76407e8f19f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5791570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:867b32255b88f60d07acade09951f750511126cc8d5374bd10545e7323c35c2a`

```dockerfile
```

-	Layers:
	-	`sha256:e0174f1a45c8df6d746b5302d36a7a2ea0441aeb8c41cbff7ab4e7ad81177063`  
		Last Modified: Wed, 22 Nov 2023 00:09:00 GMT  
		Size: 5.8 MB (5752050 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d56be9609f6b573bd09add9cf3de36ee3eba7f12191c622c68aaca65ad88aecf`  
		Last Modified: Wed, 22 Nov 2023 00:09:00 GMT  
		Size: 39.5 KB (39520 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:php8.1-apache` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:a7b2e6ad36f483ac4834c4c53add3bf472c2a4f8dc32185924f741033510a3ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.5 MB (192508375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41ff8abeb9d16d0d20f6da9fbbbfd9b62f803fdfc6ef7e0fd1c67ddc31bd9fb`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:51:07 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Nov 2023 11:51:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Nov 2023 11:51:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:51:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Nov 2023 11:51:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 01 Nov 2023 11:55:14 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 01 Nov 2023 11:55:15 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 01 Nov 2023 11:55:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 01 Nov 2023 11:55:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 01 Nov 2023 11:55:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 01 Nov 2023 11:55:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 11:55:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Nov 2023 11:55:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Nov 2023 12:49:53 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Nov 2023 12:49:54 GMT
ENV PHP_VERSION=8.1.25
# Wed, 01 Nov 2023 12:49:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.25.tar.xz.asc
# Wed, 01 Nov 2023 12:49:54 GMT
ENV PHP_SHA256=66fdba064aa119b1463a7969571d42f4642690275d8605ab5149bcc5107e2484
# Wed, 01 Nov 2023 12:50:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Nov 2023 12:50:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Nov 2023 12:53:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Nov 2023 12:53:20 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 01 Nov 2023 12:53:21 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Nov 2023 12:53:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Nov 2023 12:53:21 GMT
STOPSIGNAL SIGWINCH
# Wed, 01 Nov 2023 12:53:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 01 Nov 2023 12:53:21 GMT
WORKDIR /var/www/html
# Wed, 01 Nov 2023 12:53:21 GMT
EXPOSE 80
# Wed, 01 Nov 2023 12:53:21 GMT
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
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74a1d4347681dafacc4fd7807e0fd4250100fd23d88a3a5bb93ba9de6ebfa853`  
		Last Modified: Wed, 01 Nov 2023 13:32:59 GMT  
		Size: 228.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:381c9f838d23f8118bfd5cbaf969e6781ce721288fdbf4811d4613b8c94a0acb`  
		Last Modified: Wed, 01 Nov 2023 13:33:10 GMT  
		Size: 98.1 MB (98131824 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:acb23c56d5c248ab07de2c65e6805408398ad24b9e7f68b76a772fd923a541f0`  
		Last Modified: Wed, 01 Nov 2023 13:32:59 GMT  
		Size: 270.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59d3602892ec55ef6fa41b79e63f381805cacfdd794280d67a0b4babd0bec43b`  
		Last Modified: Wed, 01 Nov 2023 13:33:38 GMT  
		Size: 20.3 MB (20306772 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:339958c8b19db06ee2019751c64cb419ac60d5e696023999e381ac3d84a8511f`  
		Last Modified: Wed, 01 Nov 2023 13:33:36 GMT  
		Size: 476.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:663bea60fafb0c6c43b3bf486910e7685edaa95e7b4794a8b5f952cc546ca561`  
		Last Modified: Wed, 01 Nov 2023 13:33:36 GMT  
		Size: 512.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:24fd3bc3cf2c30ed1cf840853c3c4def1f65052fc214234daac7ec82a3305631`  
		Last Modified: Wed, 01 Nov 2023 13:39:45 GMT  
		Size: 12.2 MB (12222563 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c76b281efbbce580fa2d78d9bb8405d9c4ce03b63b56eabb3c53e67a621f7b5`  
		Last Modified: Wed, 01 Nov 2023 13:39:42 GMT  
		Size: 492.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89d42d23c585dbd3d5b6f8128374b23ea02d9ea7150f8b10e0639b4a98ba141e`  
		Last Modified: Wed, 01 Nov 2023 13:39:44 GMT  
		Size: 11.2 MB (11150416 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de946440e878c565797c75a4ef1451eca4737aa7c6894f9cd4c1117707b30605`  
		Last Modified: Wed, 01 Nov 2023 13:39:42 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8e2dc25626e374568cdcd5d4e790d5e6b8547e805d677f5cff590509cf22ed5`  
		Last Modified: Wed, 01 Nov 2023 13:39:42 GMT  
		Size: 246.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8f5b834c006ad3f01146dbc2c40786c38e3df7f2870c29f053782e1ff1f6b233`  
		Last Modified: Wed, 01 Nov 2023 13:39:42 GMT  
		Size: 895.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf135c7c5cb0b6d405c8375179880ec7d41c5c00b7b2bf576b857bd06f9208fb`  
		Last Modified: Wed, 08 Nov 2023 21:14:53 GMT  
		Size: 2.3 MB (2252386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b7bc7bdc80fcd28972061c3c876a17d15e569bd83a3d96e74bda8f3cb2b83f17`  
		Last Modified: Wed, 08 Nov 2023 21:14:53 GMT  
		Size: 314.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbbb629b502cbab094c5c2ebc4a7169cec562c46747170606cf56b6bb13e1e7a`  
		Last Modified: Wed, 08 Nov 2023 21:14:53 GMT  
		Size: 705.0 KB (705007 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:640610009507de15e03bb35a678731660ddb4b9bdaba2beb8a41c5aabfc2c5fb`  
		Last Modified: Wed, 08 Nov 2023 21:14:53 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c42c4127f3933f1882ac1a5e83a90eb99e9a752c8e870472983917a0385726a`  
		Last Modified: Wed, 08 Nov 2023 21:14:56 GMT  
		Size: 18.6 MB (18554282 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache` - unknown; unknown

```console
$ docker pull drupal@sha256:d7e7ac57828668dea15483ba8b0aa510e37507b1c1b7ff40e6ea25eb70b9c5ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5976783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:980addf32ccaabc44e497cb5e3519f7f79e22ae0bbb459a2b5b5d9f3169a5a70`

```dockerfile
```

-	Layers:
	-	`sha256:429d6ac8b31bccf8ba20f40d20e4195053f2b6ea582913bd9e7b1e70f7eac544`  
		Last Modified: Wed, 08 Nov 2023 21:14:51 GMT  
		Size: 5.9 MB (5937406 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:cd234fc63fbab0ae2a547c42b048337b42faabe392b02f031caed23d6256f42b`  
		Last Modified: Wed, 08 Nov 2023 21:14:51 GMT  
		Size: 39.4 KB (39377 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:php8.1-apache` - linux; 386

```console
$ docker pull drupal@sha256:d676fb9e0c23d194e234206c38e63fa26bc816b657972a2ada2a53d184ece260
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.4 MB (197431856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daeb771f78afe3f693a64803ef8b7269f8bfed0e21ab6d9311b908b0403d248d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 17:45:09 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
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
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c89090867ba89e0914603f0aaa2982d94d141eefc215d406364d3347331a329e`  
		Last Modified: Tue, 21 Nov 2023 14:11:55 GMT  
		Size: 229.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ef61714f071aa04227b826da64a97bb2a4b31b44dfac6bf42e6f5cde2f75b196`  
		Last Modified: Tue, 21 Nov 2023 14:12:19 GMT  
		Size: 101.5 MB (101532658 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa0f5dd0a218260c92c9896edbbf6aa33e888ee38871d1cc023fa1ff75ba32d5`  
		Last Modified: Tue, 21 Nov 2023 14:11:54 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22e5f5952e6b664a76523d4b17e66236eea681362ec18717f95d41b420858056`  
		Last Modified: Tue, 21 Nov 2023 14:12:48 GMT  
		Size: 20.8 MB (20826790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f30f614ac19ae735734c0b1774377e18e36c8677093210616a2227fc388c83b`  
		Last Modified: Tue, 21 Nov 2023 14:12:43 GMT  
		Size: 475.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e744e7aec12e0fcb8f62be92f065cab544fab292b20911946fcd9031b575095f`  
		Last Modified: Tue, 21 Nov 2023 14:12:43 GMT  
		Size: 511.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd95f2157d2d19c4ff8da2e0c53baf860ec91d5bcc5a91a9354bfa9f152a8777`  
		Last Modified: Tue, 21 Nov 2023 14:25:24 GMT  
		Size: 12.2 MB (12221942 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6ac9730817784870554eb907e56482ba6aa20b43466180541c291211eba66e36`  
		Last Modified: Tue, 21 Nov 2023 14:25:21 GMT  
		Size: 492.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12da06c6f5ae671d6184dc5d30ebc04ab466a726db9b920c0f853ada3218727f`  
		Last Modified: Tue, 21 Nov 2023 14:25:24 GMT  
		Size: 11.4 MB (11374400 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e71cdad63fc1877e877755977b33b93387fee9e0f89d3942c26b521ab80ce0b0`  
		Last Modified: Tue, 21 Nov 2023 14:25:21 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:760968aba9aeefd39b50e73c896fad821d097eccbd0f9dc457519700c994ca87`  
		Last Modified: Tue, 21 Nov 2023 14:25:21 GMT  
		Size: 247.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4aaef687bb41d84df1fc24677496361d5daa7842041e2185f98e5f8a5275b8e5`  
		Last Modified: Tue, 21 Nov 2023 14:25:21 GMT  
		Size: 893.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9ff58eebbb129a6b147b32c4b5730fd83aa298df7064fc3dd82ae0246a117ec3`  
		Last Modified: Tue, 21 Nov 2023 17:32:08 GMT  
		Size: 2.0 MB (2046597 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db5da3b7e43479ff37f770f706b359075ee2c094d6eb4a48e75681b97f77abe6`  
		Last Modified: Tue, 21 Nov 2023 17:32:07 GMT  
		Size: 314.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50c0b0f7c1ea48f52f8bf993e6a8e66b057f60258a810e4f3e781851d5be0a72`  
		Last Modified: Tue, 21 Nov 2023 17:32:07 GMT  
		Size: 705.0 KB (705010 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89be3b52bfe3a8e319e0aca28dc2774f837f1f34891431753bd47c7ed0ef3ef7`  
		Last Modified: Tue, 21 Nov 2023 17:32:07 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8876722621bd5f0c5c1069a0ab27639ae43cb7ec1b50dd98ae2a867445e9fc1d`  
		Last Modified: Tue, 21 Nov 2023 17:32:10 GMT  
		Size: 18.6 MB (18554346 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache` - unknown; unknown

```console
$ docker pull drupal@sha256:c8821f0e38da4feb6cbd20c33e58c3a9a5d38911c4ee53f51ce6fc5190ed6a7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 KB (41339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51108554d52908a4e26d307f195fd38a83f445542522be57e04f1ae6785b1ed5`

```dockerfile
```

-	Layers:
	-	`sha256:d599d5801481d94d2465a85447ac6f75050d6166f1e44bedd5f5da362b7a0eb6`  
		Last Modified: Tue, 21 Nov 2023 17:32:07 GMT  
		Size: 41.3 KB (41339 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:php8.1-apache` - linux; ppc64le

```console
$ docker pull drupal@sha256:a87257ee059969f120a31a01faac2355d6bf8735455d162a714441b77f7c4e12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.8 MB (202817717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4ebdadb15a67e27bc4258ee2b53ba25bb062915f049dbc2643bb80743fffbdf`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 17:45:09 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
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
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c82a664b07ee97a51b3cda0d3c288ec64eb5e92be846f5cff8a7015b7e67d418`  
		Last Modified: Tue, 21 Nov 2023 15:17:42 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c5ee042a03e72d648db3e608b3e68c6776cd32dabe79f650b4666305f6820ea0`  
		Last Modified: Tue, 21 Nov 2023 15:17:59 GMT  
		Size: 103.3 MB (103321918 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d869be71ab64ef6b34e324746d041204b8262173bd6e64c32f0cc0b6f081576c`  
		Last Modified: Tue, 21 Nov 2023 15:17:42 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a84070310a80e6e1d601e77d02287d05158e8dc837d53c55d5029555207f4fa`  
		Last Modified: Tue, 21 Nov 2023 15:18:30 GMT  
		Size: 21.5 MB (21490294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19fda3039825248ac15db201f1eac41f62065888a5efbf2fb317c7c9fceac313`  
		Last Modified: Tue, 21 Nov 2023 15:18:26 GMT  
		Size: 478.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dab7bddb2a35d16d0c9b4aa82769f4121b3684f949ef72d7aa45301d45d8b0be`  
		Last Modified: Tue, 21 Nov 2023 15:18:26 GMT  
		Size: 514.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:363cc9c3d9d402535d903a683da431743055a85a9efef50df549b769d83e3b98`  
		Last Modified: Tue, 21 Nov 2023 15:30:46 GMT  
		Size: 12.2 MB (12222137 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:73971abae19463326b709aeb8b00787fc985131eae1ea11b1043e12c0c635c7e`  
		Last Modified: Tue, 21 Nov 2023 15:30:42 GMT  
		Size: 490.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:795a3bad035e7c78ff6b129c60cabad590f1a8f42dc9fb0831efbafee5c085c6`  
		Last Modified: Tue, 21 Nov 2023 15:30:45 GMT  
		Size: 11.5 MB (11528242 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:76e0ca1299c510417cfdd9a804f81170bad53318542a1d3610c98dc7c21f1f97`  
		Last Modified: Tue, 21 Nov 2023 15:30:42 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72ff2119ed8cda209a67d090e2c2eb80508cb8fab8d5b387aeba2801f890c5e7`  
		Last Modified: Tue, 21 Nov 2023 15:30:42 GMT  
		Size: 244.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c498535d8a58996f488c0f967be5d936418176fa0a86d8b12b2cdf9404ba6ffb`  
		Last Modified: Tue, 21 Nov 2023 15:30:42 GMT  
		Size: 892.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c1a35b1ba8ee6239d318215ef6bce471492cd9fefec9427aa7491b678778936`  
		Last Modified: Wed, 22 Nov 2023 02:02:48 GMT  
		Size: 1.8 MB (1848518 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29286f22e22b332f63948d971a08480051ba0dee2f39c0baed8e1100083bbb12`  
		Last Modified: Wed, 22 Nov 2023 02:02:47 GMT  
		Size: 314.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:efd731d38828215029b4522f1a0eb97754858364de5322484610be49475c67c6`  
		Last Modified: Wed, 22 Nov 2023 02:02:48 GMT  
		Size: 705.0 KB (705009 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e961c740c652a3fb2c45db057847869199149bb43044131806cfc2442acbd30b`  
		Last Modified: Wed, 22 Nov 2023 02:02:48 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4946f1f9ee73b9bdd611059401209241a0379e01bcf188af906fe7bcba863afc`  
		Last Modified: Wed, 22 Nov 2023 02:02:49 GMT  
		Size: 18.6 MB (18553995 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache` - unknown; unknown

```console
$ docker pull drupal@sha256:6f91d938a862351cd9ce75452bb822546aaf41949aace9a75149b4ce879aa525
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5933210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59049751e11f7d9a75102db85d1b3050d11359c16fc9f4041b9019f49b8beee6`

```dockerfile
```

-	Layers:
	-	`sha256:84b36840ba23eb7ab19d37579ef0520523b312279cca02cbd9be133f68d72025`  
		Last Modified: Wed, 22 Nov 2023 02:02:46 GMT  
		Size: 5.9 MB (5893758 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9323edaf26f24c58c132e02fc400bce08a47064fe21d7c99c683dc5d76ba5434`  
		Last Modified: Wed, 22 Nov 2023 02:02:45 GMT  
		Size: 39.5 KB (39452 bytes)  
		MIME: application/vnd.in-toto+json

### `drupal:php8.1-apache` - linux; s390x

```console
$ docker pull drupal@sha256:28a268778da7127c4e5b8f418c4cfc08498a273e0c1801751e556f4f0c9628b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.7 MB (171661009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a03e3d75d39f70c5b7adbf394526eae8ce8f37a3523995297d38c9eb3399c922`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 01 Nov 2023 17:45:09 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
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
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41b073bc5f3b6460a2e86e6384462103c710b42906361c6fbf338c39d9c58ceb`  
		Last Modified: Tue, 21 Nov 2023 12:25:59 GMT  
		Size: 226.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fca956902ffd9934a4d2fb043c2f4c6e1fb6f0642f0568699e799c560c20ea15`  
		Last Modified: Tue, 21 Nov 2023 12:26:10 GMT  
		Size: 80.8 MB (80819423 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a3b8dfba35b49398dd688150d0c85decd88885387485c3525ac75e093b667ed3`  
		Last Modified: Tue, 21 Nov 2023 12:25:59 GMT  
		Size: 271.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cd69aaa769727a63be006dd6fa255115d2086b2833811e887149e906a3bd92aa`  
		Last Modified: Tue, 21 Nov 2023 12:26:30 GMT  
		Size: 20.1 MB (20084572 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:29b0f2410c9e7b7bdff692338f17dc61648dd4c4d36f9bcb4acffe5800ea041e`  
		Last Modified: Tue, 21 Nov 2023 12:26:28 GMT  
		Size: 472.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ac15cf9228cfb1e9d2f6feb3fcdffb4de33873052e9f846e1ec24778ad1c9b4`  
		Last Modified: Tue, 21 Nov 2023 12:26:28 GMT  
		Size: 511.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aaa1a492ba92d04a8d2f9fe63c72b195049b5fdc6678f87fc9ecd61cc021809f`  
		Last Modified: Tue, 21 Nov 2023 12:35:04 GMT  
		Size: 12.2 MB (12221252 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:429ebfb01666e15b4a406bc1783b2d1ce65eb335f490ab0e02eab01a870e615e`  
		Last Modified: Tue, 21 Nov 2023 12:35:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ff4c2d113b23d7fd2e8837373b1c8dda85c3922dba3400196ac9f0cf762177e`  
		Last Modified: Tue, 21 Nov 2023 12:35:04 GMT  
		Size: 10.2 MB (10211575 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:020ccf4d41bfb5ad5fca5e70f9bd821312723171255e13855321171d37fa9767`  
		Last Modified: Tue, 21 Nov 2023 12:35:02 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8373d5ee72730f08e1fe657e8ab0ab6f488d5b67edb71f6c74e52119f9bda969`  
		Last Modified: Tue, 21 Nov 2023 12:35:02 GMT  
		Size: 244.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b57c887bbec8fbfb658ba2b61fd50ef071c4152be7d773be76d21b0e30ebf8f`  
		Last Modified: Tue, 21 Nov 2023 12:35:02 GMT  
		Size: 895.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1a8ea7b58bb11093361c18d9dbc94ee91f3fcd3ed878e26034bdcf8c3188f5`  
		Last Modified: Tue, 21 Nov 2023 20:33:43 GMT  
		Size: 1.5 MB (1546300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f3ca703b92c4643d364c90f7f7f0d76cf48da69e26d7f4f31522bc59ad66a063`  
		Last Modified: Tue, 21 Nov 2023 20:33:43 GMT  
		Size: 311.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:82d072aebf88a53322b71f65b25ca0e73e844efbb2c9acb60392a48bc11bf53c`  
		Last Modified: Tue, 21 Nov 2023 20:33:44 GMT  
		Size: 705.0 KB (705009 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7c5a9ea606b5acb3f231e49cb259bd7c1918c85e1120c0b8e851890cb6ac0527`  
		Last Modified: Tue, 21 Nov 2023 20:33:43 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab166e2ece689c688079175e7d1c7dab77f98cedb8d249a32f5c9212b01429a3`  
		Last Modified: Tue, 21 Nov 2023 20:33:45 GMT  
		Size: 18.6 MB (18553997 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `drupal:php8.1-apache` - unknown; unknown

```console
$ docker pull drupal@sha256:a93f347b028c61875f030d752284585e5a6b4da02c45be7ee70d2825d1b51737
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5813236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fdf35ef54e6977e5a2d40eb007758e389482ae4684ec127abfc57b0a6b1a4e4`

```dockerfile
```

-	Layers:
	-	`sha256:b7189d39be8a2187dfa835f08a4f5ae06007724f908bdf533c55585fda04aac2`  
		Last Modified: Tue, 21 Nov 2023 20:33:42 GMT  
		Size: 5.8 MB (5773885 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b82f1dd6ef76528638ba3a98eb3ead14d08e35971625af38047e101c4e21f888`  
		Last Modified: Tue, 21 Nov 2023 20:33:42 GMT  
		Size: 39.4 KB (39351 bytes)  
		MIME: application/vnd.in-toto+json
