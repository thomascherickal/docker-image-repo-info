## `drupal:apache-buster`

```console
$ docker pull drupal@sha256:c984f883772a228fe8b9b7c5fbfd9fb7b841cc9460c2267442846ad299337bdd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:4f15d615b3bba9eaa32f7b3a950be32970970eeb98c29f6d6087c5950582cdd9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.9 MB (169924457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c932eba63548791495bdf88d79a87b40dc0aff5f839b3e25684621d3b6bf1c3e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 19:55:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 19:55:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 19:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 19:55:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 19:55:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 20:03:53 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Dec 2021 20:03:54 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Dec 2021 20:04:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Dec 2021 20:04:14 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Dec 2021 20:04:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Dec 2021 20:04:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 20:04:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 20:04:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 21:08:04 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 20 Jan 2022 20:41:52 GMT
ENV PHP_VERSION=8.0.15
# Thu, 20 Jan 2022 20:41:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Thu, 20 Jan 2022 20:41:53 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Thu, 20 Jan 2022 20:42:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 20 Jan 2022 20:42:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:49:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 20 Jan 2022 20:49:37 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:49:37 GMT
RUN docker-php-ext-enable sodium
# Thu, 20 Jan 2022 20:49:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 20 Jan 2022 20:49:38 GMT
STOPSIGNAL SIGWINCH
# Thu, 20 Jan 2022 20:49:38 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:49:38 GMT
WORKDIR /var/www/html
# Thu, 20 Jan 2022 20:49:39 GMT
EXPOSE 80
# Thu, 20 Jan 2022 20:49:39 GMT
CMD ["apache2-foreground"]
# Thu, 20 Jan 2022 22:15:43 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 22:15:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 24 Jan 2022 20:03:35 GMT
COPY file:3713581496added9c148c20084b87b399428028bf2a1d7bf85f3574a00a0b8f3 in /usr/local/bin/ 
# Mon, 24 Jan 2022 20:09:00 GMT
ENV DRUPAL_VERSION=9.2.11
# Mon, 24 Jan 2022 20:09:00 GMT
WORKDIR /opt/drupal
# Mon, 24 Jan 2022 20:09:15 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 24 Jan 2022 20:09:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf13c1e88c3d5ec6b06b45a8a6014f2e6dad30b6d4e3f2a08e653b2d2e3fd46`  
		Last Modified: Tue, 21 Dec 2021 22:44:37 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cddf9116140097c570dbf83d0301fe37fed9551b2f476c69cecd86397bdc239e`  
		Last Modified: Tue, 21 Dec 2021 22:44:52 GMT  
		Size: 76.7 MB (76680919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c396aa97b98688e4530e154aad60e27418f8e2c467e807f8f73efb42b62fe45`  
		Last Modified: Tue, 21 Dec 2021 22:44:36 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9707294ce1de6d169b3f08b5dee9e60e872ea53564a7a21236507197d5877a`  
		Last Modified: Tue, 21 Dec 2021 22:45:25 GMT  
		Size: 18.7 MB (18679928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443be0efd1a3affd98bc62c3d179c1275a6a00932be3aa2c441c3485755a3c50`  
		Last Modified: Tue, 21 Dec 2021 22:45:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40e54f5a6bb4df3533473e34b9a865afcdc3fd3023e38ed604aea453c7f8335`  
		Last Modified: Tue, 21 Dec 2021 22:45:20 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e157b83fa74e38ca6881d92213bafab42408af5d033210a0e394281def58ce9c`  
		Last Modified: Thu, 20 Jan 2022 21:52:12 GMT  
		Size: 11.1 MB (11102535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfba06ea24db6b1a9c6793eda07d1949d16bbfce27aed70dcccfce509ea425f`  
		Last Modified: Thu, 20 Jan 2022 21:52:08 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ede55b6a637b114194c18fa838c2fb2d24a65970ca0197a5850b0dd60ba9ae1`  
		Last Modified: Thu, 20 Jan 2022 21:52:11 GMT  
		Size: 14.5 MB (14506034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eba4e3533c63310bb5e3c3fbb45793b09a5eb45be1b4263d1713d9e88eae84e`  
		Last Modified: Thu, 20 Jan 2022 21:52:08 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35ce4e947df8ae26f634f167a4fe44c805b2f63e5a87cb2c3fb9f7472eff90c`  
		Last Modified: Thu, 20 Jan 2022 21:52:08 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f69508b612ae4868cfad7415b55602175b563218e904fe99a008ddf8b6dc34`  
		Last Modified: Thu, 20 Jan 2022 21:52:08 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fda95c1e5cc45003f06ae08532aa2fd133d3ffb1553a133dba9bf41711a07f`  
		Last Modified: Thu, 20 Jan 2022 22:29:35 GMT  
		Size: 2.0 MB (2016759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c748666e9471652b65bdefe12573d5fd76e1009a4554ddb82f67b76b4fa07b6`  
		Last Modified: Thu, 20 Jan 2022 22:29:35 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472b638699c3ffb7b456ba3024f97ee04c9946875d311685ecf0540216d7714d`  
		Last Modified: Mon, 24 Jan 2022 20:21:06 GMT  
		Size: 574.6 KB (574584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939d1a5a041d216edb342fb7c673e788780dac378d71ed224b959bad93722810`  
		Last Modified: Mon, 24 Jan 2022 20:39:17 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecfcc1a1db5585a4561d8e9354a12de1e150fa76dc0d0fe58d7f116c69473ac`  
		Last Modified: Mon, 24 Jan 2022 20:39:22 GMT  
		Size: 19.2 MB (19204060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:994f87d11632c1445e2e1dc05fb2a3922f7e3ed040afa3ed0c1f725265135ef3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144597287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b28c045d345363e9616e0aeda925588c670c20db4fea7a0661c4fccd63ae914`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Dec 2021 02:00:52 GMT
ADD file:1381e18e2847f24ebd16d8e83ad940adeff45aca2c327d4e07d7451816f29420 in / 
# Tue, 21 Dec 2021 02:00:52 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 10:26:49 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 10:26:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 10:27:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 10:27:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 10:27:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 10:33:13 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Dec 2021 10:33:14 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Dec 2021 10:33:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Dec 2021 10:33:37 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Dec 2021 10:33:39 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Dec 2021 10:33:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 10:33:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 10:33:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 11:15:23 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 20 Jan 2022 20:53:17 GMT
ENV PHP_VERSION=8.0.15
# Thu, 20 Jan 2022 20:53:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Thu, 20 Jan 2022 20:53:18 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Thu, 20 Jan 2022 20:53:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 20 Jan 2022 20:53:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:58:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 20 Jan 2022 20:58:34 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:58:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 20 Jan 2022 20:58:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 20 Jan 2022 20:58:37 GMT
STOPSIGNAL SIGWINCH
# Thu, 20 Jan 2022 20:58:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:58:38 GMT
WORKDIR /var/www/html
# Thu, 20 Jan 2022 20:58:38 GMT
EXPOSE 80
# Thu, 20 Jan 2022 20:58:39 GMT
CMD ["apache2-foreground"]
# Thu, 20 Jan 2022 22:15:18 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 22:15:20 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 24 Jan 2022 20:18:32 GMT
COPY file:3713581496added9c148c20084b87b399428028bf2a1d7bf85f3574a00a0b8f3 in /usr/local/bin/ 
# Mon, 24 Jan 2022 20:28:52 GMT
ENV DRUPAL_VERSION=9.2.11
# Mon, 24 Jan 2022 20:28:53 GMT
WORKDIR /opt/drupal
# Mon, 24 Jan 2022 20:29:20 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 24 Jan 2022 20:29:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b597e1a6bc27aa2a24a587cb687c9551dfbcfa730a11d48c5a44ff77ff6fdd75`  
		Last Modified: Tue, 21 Dec 2021 02:16:50 GMT  
		Size: 22.8 MB (22754324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31790e78e71da3493063e5402d65c27e8cb5f7140f9aba0ff2de9aaba77773b4`  
		Last Modified: Tue, 21 Dec 2021 13:13:41 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f548eb2e152190a56328e2a5f34e6655f41f1c332c9d678629753a97745ee82d`  
		Last Modified: Tue, 21 Dec 2021 13:14:13 GMT  
		Size: 59.5 MB (59515646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab7c2ab078879c469beb21215d355e69eb2acc2fcb85a2ad377e45c4e95c36`  
		Last Modified: Tue, 21 Dec 2021 13:13:41 GMT  
		Size: 272.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeaf1c1024c01ee445d31e937dc994e626716da6b9705e29345681bf6265f0f2`  
		Last Modified: Tue, 21 Dec 2021 13:15:02 GMT  
		Size: 17.5 MB (17481468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665705be425f7e835310c58a9ef3028ce6dd76bb509be9e7e4d9de43a351ba9f`  
		Last Modified: Tue, 21 Dec 2021 13:14:52 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7b9681b33fd145ac0facba259d73e6e16547c07a25e706affb3786fe6a5fed`  
		Last Modified: Tue, 21 Dec 2021 13:14:52 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4f3e4d1e18849091dde2ba9968bc98477ee05493b727830fc46b7bf6b41f24`  
		Last Modified: Thu, 20 Jan 2022 21:58:32 GMT  
		Size: 11.1 MB (11100646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:525066dfd0a700b23c1687a98c29c083e6637fc869856ed2044c248b63a6b2b7`  
		Last Modified: Thu, 20 Jan 2022 21:58:27 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376e4e7cee9a3699c33dc6d3d2be857002da7c8390773aefb7cc2cf1343a3ea1`  
		Last Modified: Thu, 20 Jan 2022 21:58:36 GMT  
		Size: 12.5 MB (12508656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af8dad8963c5fbe02ef0478cb5aca843c05d59afeb3c86736f0ad500c0d99dc`  
		Last Modified: Thu, 20 Jan 2022 21:58:27 GMT  
		Size: 2.3 KB (2316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5be530defea9d415e2afd6c8f727b4ab0e403ecfd409d8c6bee61e3bb105b948`  
		Last Modified: Thu, 20 Jan 2022 21:58:27 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4cfdc48eb2fe67258d77bcd47a33868238e37bd203b24110b34aa64ddc2651`  
		Last Modified: Thu, 20 Jan 2022 21:58:27 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004f632d6323716516096962ef73d3dc4a4e23611dc8fff084140fc6aceeb2e2`  
		Last Modified: Thu, 20 Jan 2022 22:51:42 GMT  
		Size: 1.5 MB (1452225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f410fb60ac9261d96573ba38660f3c28a2294b4341cbc8ca6837c0361f75a45c`  
		Last Modified: Thu, 20 Jan 2022 22:51:42 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a5f1174ced574bdc64a37f36abcf145013c92bbd9fc7c16cc47753336e5749`  
		Last Modified: Mon, 24 Jan 2022 20:56:43 GMT  
		Size: 574.6 KB (574576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0da5c079a90ccb5cb6b22ee2c9dcec7163f0f083f97163bcf2947f26c3e33b6`  
		Last Modified: Mon, 24 Jan 2022 21:09:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d900033c2cd7fc261219c322a0e863debf331168765fcbdf25c3cd3497c0ee47`  
		Last Modified: Mon, 24 Jan 2022 21:10:00 GMT  
		Size: 19.2 MB (19203821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:f6258bb9e76e0986c561d32a10d94357c6f5a8f78bb2633e5b1ba83d637faba8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.7 MB (160717600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:107d2e5d42130daa81799a69da5ebdde3c9128f2f7b38f0932ce68a60707e151`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:48 GMT
ADD file:9810440ab841e71bd153282c21cfcd46d3f40bd5099e60c332e05bf066e390ac in / 
# Tue, 21 Dec 2021 01:42:49 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:52:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 03:52:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 03:52:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:52:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 03:52:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 03:57:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Dec 2021 03:57:21 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Dec 2021 03:57:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Dec 2021 03:57:30 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Dec 2021 03:57:31 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Dec 2021 03:57:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 03:57:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 03:57:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 04:25:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 20 Jan 2022 20:00:52 GMT
ENV PHP_VERSION=8.0.15
# Thu, 20 Jan 2022 20:00:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Thu, 20 Jan 2022 20:00:53 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Thu, 20 Jan 2022 20:01:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 20 Jan 2022 20:01:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:03:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 20 Jan 2022 20:03:51 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:03:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 20 Jan 2022 20:03:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 20 Jan 2022 20:03:53 GMT
STOPSIGNAL SIGWINCH
# Thu, 20 Jan 2022 20:03:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:03:55 GMT
WORKDIR /var/www/html
# Thu, 20 Jan 2022 20:03:56 GMT
EXPOSE 80
# Thu, 20 Jan 2022 20:03:57 GMT
CMD ["apache2-foreground"]
# Thu, 20 Jan 2022 21:03:07 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 21:03:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 24 Jan 2022 19:57:50 GMT
COPY file:3713581496added9c148c20084b87b399428028bf2a1d7bf85f3574a00a0b8f3 in /usr/local/bin/ 
# Mon, 24 Jan 2022 20:05:05 GMT
ENV DRUPAL_VERSION=9.2.11
# Mon, 24 Jan 2022 20:05:06 GMT
WORKDIR /opt/drupal
# Mon, 24 Jan 2022 20:05:36 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 24 Jan 2022 20:05:38 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:753408153c81560bc4244b14524c404cbf483c8afa8ac924272545400536a9d8`  
		Last Modified: Tue, 21 Dec 2021 01:49:44 GMT  
		Size: 25.9 MB (25923149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399cd382f74b9333921ab9450361ddfc29e07826cfb4906582618a1665ba6ba0`  
		Last Modified: Tue, 21 Dec 2021 05:25:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978dcfbedcedd2e259c7988f1c18e962e16d5ca4aaf0371c8d53e57eeb7411b6`  
		Last Modified: Tue, 21 Dec 2021 05:25:19 GMT  
		Size: 70.4 MB (70359361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f787b5a5e5d17b19845cd143a04fc6d2bc76cc9432e2ef888079bcf12142b6`  
		Last Modified: Tue, 21 Dec 2021 05:25:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddea69969cce0cd061920b09c53b87bfaa4f22bd200e665ca39b1b53f80bba21`  
		Last Modified: Tue, 21 Dec 2021 05:25:56 GMT  
		Size: 18.4 MB (18365255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dcaca783979ecf373cc99da723cd1da88c2e82df4996e8cdc91d5a72c051be`  
		Last Modified: Tue, 21 Dec 2021 05:25:53 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45e6c5a9aba6e73fe091cc78eda737bc67e6650c252a596a254dd8309aca36a`  
		Last Modified: Tue, 21 Dec 2021 05:25:53 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc66cd94a9a918c09264e18374d50d87ab12672384ee9a45c68e7e45bf06473`  
		Last Modified: Thu, 20 Jan 2022 20:37:51 GMT  
		Size: 10.9 MB (10889442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc17f18fd59e328fa122f280b9928e2b5dfdfd353a78ecb1579220731f6d3148`  
		Last Modified: Thu, 20 Jan 2022 20:37:48 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae77fe726d7e0aad13d3e73825dc21245a28563103fa6cc6b39945bf91a0b01`  
		Last Modified: Thu, 20 Jan 2022 20:37:51 GMT  
		Size: 13.9 MB (13932497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f71c3e2feedb9d618a6152288c0a2ef0df6fa9bd58a544dc8f3cbdafad73b0b`  
		Last Modified: Thu, 20 Jan 2022 20:37:48 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faed083b0021c7971f3c279202012538317fbe2b1cc41341bcae7c4a6a684f8`  
		Last Modified: Thu, 20 Jan 2022 20:37:48 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0ab51443a7e4d513979fb471f03154f6eaecc1a35ec7ae3db17ac664d8b571`  
		Last Modified: Thu, 20 Jan 2022 20:37:48 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108fabd2792ee13abb1276a80023a7f6cd5d54aed46ca94305b8a57bdd496288`  
		Last Modified: Thu, 20 Jan 2022 21:21:04 GMT  
		Size: 1.5 MB (1464926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e3ec7339a18ab184ed912bb05cbbe9e19ecbd62a9e480acaf76465b1a7843c`  
		Last Modified: Thu, 20 Jan 2022 21:21:03 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf39f55d389a5e17a1c759bdf7214d416f5c8fe19061ef30a185be709bca0ef`  
		Last Modified: Mon, 24 Jan 2022 20:19:09 GMT  
		Size: 574.6 KB (574575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f243398fcb037c7ad4a4baf31553c21b0c69dd83005ec66d3502b48fe18a6daa`  
		Last Modified: Mon, 24 Jan 2022 20:26:16 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33001fe7e9f704454bef0cbf489e7e735ba63367b3c92a25c500086e224f15e`  
		Last Modified: Mon, 24 Jan 2022 20:26:21 GMT  
		Size: 19.2 MB (19202635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:a44709e1dd38bcaea37565bda2091e28228e7bf46a46bd5072f62ddabf70f0d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.9 MB (175899104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccae9210f1af4a9bcc64296176ec6166ae1ed0a358680e36b0055d373e05791b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Dec 2021 01:40:45 GMT
ADD file:78342a77df22ca22804ea5aec6415ce10c1fdc35687f1b25c5f86850f41d3905 in / 
# Tue, 21 Dec 2021 01:40:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 13:24:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 13:24:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 13:24:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 13:24:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 13:24:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 13:31:40 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Dec 2021 13:31:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Dec 2021 13:31:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Dec 2021 13:31:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Dec 2021 13:31:53 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Dec 2021 13:31:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 13:31:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 13:31:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 14:32:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 20 Jan 2022 20:24:02 GMT
ENV PHP_VERSION=8.0.15
# Thu, 20 Jan 2022 20:24:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Thu, 20 Jan 2022 20:24:03 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Thu, 20 Jan 2022 20:24:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 20 Jan 2022 20:24:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:32:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 20 Jan 2022 20:32:41 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:32:42 GMT
RUN docker-php-ext-enable sodium
# Thu, 20 Jan 2022 20:32:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 20 Jan 2022 20:32:42 GMT
STOPSIGNAL SIGWINCH
# Thu, 20 Jan 2022 20:32:43 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 20 Jan 2022 20:32:43 GMT
WORKDIR /var/www/html
# Thu, 20 Jan 2022 20:32:43 GMT
EXPOSE 80
# Thu, 20 Jan 2022 20:32:43 GMT
CMD ["apache2-foreground"]
# Thu, 20 Jan 2022 22:01:41 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 22:01:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 24 Jan 2022 19:58:03 GMT
COPY file:3713581496added9c148c20084b87b399428028bf2a1d7bf85f3574a00a0b8f3 in /usr/local/bin/ 
# Mon, 24 Jan 2022 20:05:20 GMT
ENV DRUPAL_VERSION=9.2.11
# Mon, 24 Jan 2022 20:05:20 GMT
WORKDIR /opt/drupal
# Mon, 24 Jan 2022 20:05:40 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 24 Jan 2022 20:05:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:16e3a221bce3a5f7f4a71f72926f381ff9c6141ccb5918b7ea924ff7f7f09d06`  
		Last Modified: Tue, 21 Dec 2021 01:49:46 GMT  
		Size: 27.8 MB (27804573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afe5aa88d59dd4ea92656db6f71a3adc7d0cc78736ec90239ecf8307475ab78`  
		Last Modified: Tue, 21 Dec 2021 17:13:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edb1663b27790d4fec647c37123dd6b66193226d9729046ca137d2b4f30edd5`  
		Last Modified: Tue, 21 Dec 2021 17:13:29 GMT  
		Size: 81.2 MB (81229369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8a8af335b30cca4be37c6f715065b79e533367f11a6f4b343931bd5e42e55a`  
		Last Modified: Tue, 21 Dec 2021 17:13:07 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cee771aebf79474e747a278b7b6124284a2e5659ba23d9aefd265826dfe0ea9`  
		Last Modified: Tue, 21 Dec 2021 17:14:19 GMT  
		Size: 19.1 MB (19115048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde75a4a5f3df7a926c285ea90079c0fbc357ede5f146d9b2bbd24cbbdfac40e`  
		Last Modified: Tue, 21 Dec 2021 17:14:12 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9dbf38596cc57fea79b6ed0bb8b25700459661cef23119317de8bdd1a3b701`  
		Last Modified: Tue, 21 Dec 2021 17:14:12 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc86cdb7276c4e40125a36aeb8ef27dc1294bc1aea58111325512a761f914b58`  
		Last Modified: Thu, 20 Jan 2022 21:51:39 GMT  
		Size: 11.1 MB (11101881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d311d3976d62024688147ee8f15c5c7baadc07bf747f536fa783711f6d84ff5a`  
		Last Modified: Thu, 20 Jan 2022 21:51:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7285d25272d5bc591970bc227556b01b3539f7c3821e22bd5c6ed9c3e90685`  
		Last Modified: Thu, 20 Jan 2022 21:51:40 GMT  
		Size: 14.8 MB (14794000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5085e69d794d65897744f34721cf3f8aca20c534cde9b9c2e1300fabb8478e`  
		Last Modified: Thu, 20 Jan 2022 21:51:35 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f248e04f71f875007db60cdfbcc5848fcf0cce98024b6c19e6fc353c074296f2`  
		Last Modified: Thu, 20 Jan 2022 21:51:35 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a0e40677e44cd38f03f28ad181b6d2e6734d907729edbcba72d4453eab70ec`  
		Last Modified: Thu, 20 Jan 2022 21:51:35 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded92d9e64b956e73a171bc7632331d92589eb6ba0340e232bd5ef4ffd7f9132`  
		Last Modified: Thu, 20 Jan 2022 22:24:50 GMT  
		Size: 2.1 MB (2069557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d1b03379568efd961753788f5ec7cb67ad5fe3e6493d62d42bb1162dda4c01`  
		Last Modified: Thu, 20 Jan 2022 22:24:49 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0101c84c17cacfdc6456118d9b603aa4ad7fdad392bf9b02513dfd97129768f2`  
		Last Modified: Mon, 24 Jan 2022 20:26:01 GMT  
		Size: 574.6 KB (574575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186c34fb2d5ee349eace14c2a15ef99d132d6b49d66e2373a8c718c8f7fb1702`  
		Last Modified: Mon, 24 Jan 2022 20:46:49 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51524085c9aeba58293781e4ae47abfbd0ff5cb37facfda8e0c750d2216953d`  
		Last Modified: Mon, 24 Jan 2022 20:47:04 GMT  
		Size: 19.2 MB (19204191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:apache-buster` - linux; ppc64le

```console
$ docker pull drupal@sha256:3befcdebd38f2ee8bfacb24e946436ecb19a97f6260b9b4c83f1de912cf5b3e4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **180.7 MB (180693816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e9edf73c1c54e4c3d82d4dac6ce90aad53ce4bd1d943b6a33aae69fa9a16e9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 21 Dec 2021 02:21:09 GMT
ADD file:85a8af105e3fa794598824266068cbb3c0dc66067e10e3263dab26a230458a82 in / 
# Tue, 21 Dec 2021 02:21:13 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 07:02:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 21 Dec 2021 07:02:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 21 Dec 2021 07:03:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 07:03:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 21 Dec 2021 07:03:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 21 Dec 2021 07:09:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 21 Dec 2021 07:09:12 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 21 Dec 2021 07:09:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 21 Dec 2021 07:09:55 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 21 Dec 2021 07:09:59 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 21 Dec 2021 07:10:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 07:10:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 21 Dec 2021 07:10:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 21 Dec 2021 07:50:03 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 20 Jan 2022 21:41:45 GMT
ENV PHP_VERSION=8.0.15
# Thu, 20 Jan 2022 21:41:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Thu, 20 Jan 2022 21:41:49 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Thu, 20 Jan 2022 21:42:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 20 Jan 2022 21:42:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 20 Jan 2022 21:48:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 20 Jan 2022 21:48:40 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 20 Jan 2022 21:48:48 GMT
RUN docker-php-ext-enable sodium
# Thu, 20 Jan 2022 21:48:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 20 Jan 2022 21:48:52 GMT
STOPSIGNAL SIGWINCH
# Thu, 20 Jan 2022 21:48:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 20 Jan 2022 21:48:56 GMT
WORKDIR /var/www/html
# Thu, 20 Jan 2022 21:49:00 GMT
EXPOSE 80
# Thu, 20 Jan 2022 21:49:03 GMT
CMD ["apache2-foreground"]
# Thu, 20 Jan 2022 22:51:04 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 22:51:11 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 24 Jan 2022 19:36:57 GMT
COPY file:3713581496added9c148c20084b87b399428028bf2a1d7bf85f3574a00a0b8f3 in /usr/local/bin/ 
# Mon, 24 Jan 2022 19:56:31 GMT
ENV DRUPAL_VERSION=9.2.11
# Mon, 24 Jan 2022 19:56:36 GMT
WORKDIR /opt/drupal
# Mon, 24 Jan 2022 19:57:43 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 24 Jan 2022 19:57:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:e2c79f8e0929abda2022fed71e090d3c34c8c3fdfb2a513ede1d117020a46821`  
		Last Modified: Tue, 21 Dec 2021 02:30:19 GMT  
		Size: 30.6 MB (30562311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15c9bdb6d9a379869d8c1da6eb5107dfdd8598147fc19f6a0d9509194d3d5bf`  
		Last Modified: Tue, 21 Dec 2021 09:27:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61e3c5a1fa71cf0719b52f3a7251f4495550c9ad79cc0e7e254e3ef0c9242f6`  
		Last Modified: Tue, 21 Dec 2021 09:27:31 GMT  
		Size: 82.3 MB (82291507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cb6020b1fc266273c381d36910555df49ff35872349f3cfedcc4fdc7ac9050`  
		Last Modified: Tue, 21 Dec 2021 09:27:10 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2039beeb74569c64839c020d6dc7707191f446981355b2e62626700d19343e8d`  
		Last Modified: Tue, 21 Dec 2021 09:28:13 GMT  
		Size: 19.8 MB (19818116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a610afe5ab0622e0b1a2e311efe7623c53ce3dcc51341f123571d0babfc246`  
		Last Modified: Tue, 21 Dec 2021 09:28:06 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26f5f3afcec3fc08f3b3c11c1844bb7636fb294dbd73eb8200dd193eec11f14`  
		Last Modified: Tue, 21 Dec 2021 09:28:06 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a1ae17d48d6641a59911076dca0633b4ebf6e7140b5e3f276c6d5d66a3edb3`  
		Last Modified: Thu, 20 Jan 2022 22:39:24 GMT  
		Size: 11.1 MB (11102129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be5c2cc186deb4732fb9dbcdaf3892c5fbc9556a1e782f4d414180f3c8fe7ab`  
		Last Modified: Thu, 20 Jan 2022 22:39:20 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6be4c4a9d9e6a7de3ddffc26cab73ff68dc5c8864aa61bac26b0a8a7662301`  
		Last Modified: Thu, 20 Jan 2022 22:39:23 GMT  
		Size: 15.2 MB (15213535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b26c201de48d9749134855e77d62f446ad85c7b2e7aab601ac038848d660f5`  
		Last Modified: Thu, 20 Jan 2022 22:39:19 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c61badd416650b7686c95a2c86be2a895141d3cef43aa8f015677edac5e91a3`  
		Last Modified: Thu, 20 Jan 2022 22:39:19 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caca9b0dfdf88cd814102e9b699a0d02227a8589bf9224eb33518f98fbb21402`  
		Last Modified: Thu, 20 Jan 2022 22:39:19 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caba18d7db08f9ab91cf9d3de92bf51698a01a4fed1942fc80c9c857e2a483d1`  
		Last Modified: Thu, 20 Jan 2022 23:21:54 GMT  
		Size: 1.9 MB (1922001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b92bfad828775117abe3c80a5c7cacd722a98fb960887056396bf9f5c7daf13`  
		Last Modified: Thu, 20 Jan 2022 23:21:53 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25219580f89ae2eaf73732db655efb4362705483c31674c296babd05074d738`  
		Last Modified: Mon, 24 Jan 2022 20:22:59 GMT  
		Size: 574.6 KB (574575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebc43f8bdfe281379b7fe512649cc4c340fe8777a07fb84c9014cf04ed86778`  
		Last Modified: Mon, 24 Jan 2022 20:43:55 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a4c6b7c3dbbd656223cb4a0e5bd977f8bc12a1eef2ab5425692fb26c2f7ddb`  
		Last Modified: Mon, 24 Jan 2022 20:45:04 GMT  
		Size: 19.2 MB (19203731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:apache-buster` - linux; s390x

```console
$ docker pull drupal@sha256:986bd0a7f418ad0bf8b2853c963295552f395633b4059bac425093707aeb5e29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.9 MB (154936886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3495993315c1eeec7833fcdb939d0dca8eca2340cf9a3f798ad4808a642da193`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:43 GMT
ADD file:27d2ddf8a67fd6bce8ec2eb1a83419b88265bc9b1640c3055d6b36b44586b03a in / 
# Wed, 26 Jan 2022 01:41:44 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 04:01:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Jan 2022 04:01:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Jan 2022 04:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 04:02:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Jan 2022 04:02:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Jan 2022 04:05:36 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 26 Jan 2022 04:05:36 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 26 Jan 2022 04:05:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 26 Jan 2022 04:05:44 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 26 Jan 2022 04:05:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 26 Jan 2022 04:05:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 04:05:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Jan 2022 04:05:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 26 Jan 2022 04:27:11 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 26 Jan 2022 04:27:11 GMT
ENV PHP_VERSION=8.0.15
# Wed, 26 Jan 2022 04:27:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.15.tar.xz.asc
# Wed, 26 Jan 2022 04:27:12 GMT
ENV PHP_SHA256=5f33544061d37d805a2a9ce791f081ef08a7155bd7ba2362e69bba2d06b0f8b2
# Wed, 26 Jan 2022 04:27:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 26 Jan 2022 04:27:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:29:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 26 Jan 2022 04:29:35 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:29:35 GMT
RUN docker-php-ext-enable sodium
# Wed, 26 Jan 2022 04:29:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 26 Jan 2022 04:29:36 GMT
STOPSIGNAL SIGWINCH
# Wed, 26 Jan 2022 04:29:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 26 Jan 2022 04:29:36 GMT
WORKDIR /var/www/html
# Wed, 26 Jan 2022 04:29:36 GMT
EXPOSE 80
# Wed, 26 Jan 2022 04:29:36 GMT
CMD ["apache2-foreground"]
# Wed, 26 Jan 2022 20:19:25 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 20:19:26 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 26 Jan 2022 20:19:26 GMT
COPY file:3713581496added9c148c20084b87b399428028bf2a1d7bf85f3574a00a0b8f3 in /usr/local/bin/ 
# Wed, 26 Jan 2022 20:26:52 GMT
ENV DRUPAL_VERSION=9.2.11
# Wed, 26 Jan 2022 20:26:53 GMT
WORKDIR /opt/drupal
# Wed, 26 Jan 2022 20:27:14 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 26 Jan 2022 20:27:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:72d32cf8184f85de685e3d4f0354385b1ef6ed1ff7ce95a31b81ad20d6ae77c1`  
		Last Modified: Wed, 26 Jan 2022 01:47:30 GMT  
		Size: 25.8 MB (25769120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b25e3bdb440a67637a5b683294eea90e02ec520900140a13bb2146600407791e`  
		Last Modified: Wed, 26 Jan 2022 05:20:59 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797fef2f41f2537e7ccf6744455886981644fbda3c345d3fb52a7c052bec3b3b`  
		Last Modified: Wed, 26 Jan 2022 05:21:08 GMT  
		Size: 64.7 MB (64711865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aaaa8eb39f2fee881a63cec70259c9fdc584abd9d4a2cada28fddf43f8e1bc7`  
		Last Modified: Wed, 26 Jan 2022 05:20:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9162cc6dfcc0e92aad2076c00aef7b12afb66d202b88373cd76c9d1304f7c8`  
		Last Modified: Wed, 26 Jan 2022 05:21:30 GMT  
		Size: 18.5 MB (18525108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bb77b2371fbea32b47bd3bb82000bc83703f7d01fdaeb29a6527cc275854f7`  
		Last Modified: Wed, 26 Jan 2022 05:21:28 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a772e080a75a30c48958bf70d7bb7221339f609ecbeebd1fe0f1e165e5e11b1`  
		Last Modified: Wed, 26 Jan 2022 05:21:28 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdadf43f1d60400b80c8df966c7259c8917eda356ddc5424e9e369186948e4c`  
		Last Modified: Wed, 26 Jan 2022 05:24:21 GMT  
		Size: 11.1 MB (11100894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a21a00dcf2030229fe0e0915657cb98f9f7ec38d800389c8409a5f3518607df`  
		Last Modified: Wed, 26 Jan 2022 05:24:17 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e278200f221482b2713bc79fc2cc39284fe6d792ce7d7958c2879b6d1cc208c`  
		Last Modified: Wed, 26 Jan 2022 05:24:19 GMT  
		Size: 13.4 MB (13374639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3f4f7293561028e3414b3034d800c26a0899c2266284eeda6da9a05aa56bae`  
		Last Modified: Wed, 26 Jan 2022 05:24:17 GMT  
		Size: 2.3 KB (2314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a43e849f663bb79008ab84db854ec0cf8ba89ab21497eb5b4cbb4f93f0147`  
		Last Modified: Wed, 26 Jan 2022 05:24:17 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da63b04f5d02428d92367da35dc4d2123f869307645316ce8a0ce945df6824d`  
		Last Modified: Wed, 26 Jan 2022 05:24:17 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dd6ec7756b30a986203b5b410a4fdb962a188fdc11e6d72bac2f6563bc3a24`  
		Last Modified: Wed, 26 Jan 2022 20:39:14 GMT  
		Size: 1.7 MB (1670735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b716bd328bebf58ce43b1ae679b161b9c80961f5dad05616e2b981f23d5604`  
		Last Modified: Wed, 26 Jan 2022 20:39:13 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0d6b13d941fbd456cdab116b1dc783e1d5f17704bbfb5eff68fe4cf734892d`  
		Last Modified: Wed, 26 Jan 2022 20:39:13 GMT  
		Size: 574.6 KB (574580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e4aa47107c4af2490e5b098d52e4e229d77558b36179bf08e27412a04a72c0`  
		Last Modified: Wed, 26 Jan 2022 20:42:56 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3199140194f2d145884c92b19c09b1b239bd2a7b72c4701d4d4128232d51f73`  
		Last Modified: Wed, 26 Jan 2022 20:43:00 GMT  
		Size: 19.2 MB (19204034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
