## `drupal:php8.2-apache-bullseye`

```console
$ docker pull drupal@sha256:a9e48919d1b43be47b29637971fc217329f7606bddd8bc6f3f41444d3a242a68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:php8.2-apache-bullseye` - linux; amd64

```console
$ docker pull drupal@sha256:7d4642430b2021b3a7d3038b1016255d90ca6666663a265ff1eead2cb99374b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.4 MB (187447117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1d53beb4fcd3a4e86d809dc14eebfdd1a70e61d547bfdefc9a5498d639d41e3`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:32:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 17:32:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 17:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:33:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 17:33:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 17:36:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 17:36:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 17:36:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 17:36:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 17:36:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 17:36:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 17:36:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 17:36:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 18:05:03 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 02:35:06 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 02:35:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 02:35:06 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 02:35:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 02:35:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:38:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 02:38:20 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:38:21 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 02:38:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 02:38:21 GMT
STOPSIGNAL SIGWINCH
# Sat, 30 Sep 2023 02:38:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:38:21 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 02:38:22 GMT
EXPOSE 80
# Sat, 30 Sep 2023 02:38:22 GMT
CMD ["apache2-foreground"]
# Sat, 30 Sep 2023 05:10:46 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Sep 2023 05:10:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Oct 2023 18:38:20 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Fri, 06 Oct 2023 19:36:19 GMT
ENV DRUPAL_VERSION=10.1.5
# Fri, 06 Oct 2023 19:36:19 GMT
WORKDIR /opt/drupal
# Fri, 06 Oct 2023 19:36:29 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 06 Oct 2023 19:36:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b9708f27825ba238246d858727fd21c567ca18fb96a94796a6f6178db0de04`  
		Last Modified: Wed, 20 Sep 2023 20:11:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231b648539d7ae8139fbedfd8825a254b9d58408a98c355916a5c25bb4212d7`  
		Last Modified: Wed, 20 Sep 2023 20:11:27 GMT  
		Size: 91.6 MB (91632209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a8193022d3d0b2af1e75d1fd37d6f90660dad2536d49d8096003b8e0cbe1a0`  
		Last Modified: Wed, 20 Sep 2023 20:11:14 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d026a84e3b88ea61c40e22ed7e2cad6699d70af8b80ff3c03427c297d0ed29a`  
		Last Modified: Wed, 20 Sep 2023 20:11:45 GMT  
		Size: 19.2 MB (19248150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954034b3a164067e9b2e95633301cc81f4691880785f87945bca30466da307ee`  
		Last Modified: Wed, 20 Sep 2023 20:11:42 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603ee144b85aa935d6429eedef40c5d6dc997fc874f06c348734d7a684c1208`  
		Last Modified: Wed, 20 Sep 2023 20:11:42 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8041bca4e4f5ef559627939a9cbf197b1723812e9ffaa7e64438312691aabd4d`  
		Last Modified: Sat, 30 Sep 2023 04:20:41 GMT  
		Size: 12.4 MB (12387901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911d9949239d5b80be3d6604894b438434b5c333338cfa7a10b43157897c0670`  
		Last Modified: Sat, 30 Sep 2023 04:20:38 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b97d4cc65d205b0045f139f6661e16110443f996311f276ba515ae5d165963`  
		Last Modified: Sat, 30 Sep 2023 04:20:40 GMT  
		Size: 11.4 MB (11365310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39c9fead51209cfd5ff9f7f432bb551d40782636a1a5bd977d5a639e9c6af17c`  
		Last Modified: Sat, 30 Sep 2023 04:20:38 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:448ca359948959ad196474aacb1ad820126edd12d5c3f183f005e2b615a9e784`  
		Last Modified: Sat, 30 Sep 2023 04:20:38 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce81c57aee31a814c0ffd3854e934f099dcdfbc250c932e8b777f4c6f503413`  
		Last Modified: Sat, 30 Sep 2023 04:20:38 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20a44167841b1db4957dfbfb2c9c7fd384e90eb3acf497443656a78bc052eda`  
		Last Modified: Sat, 30 Sep 2023 05:34:31 GMT  
		Size: 2.1 MB (2143104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c19bf1bce4b71c2b91000be3eb791ed024d3461446806faf2cf6b14099656f7`  
		Last Modified: Sat, 30 Sep 2023 05:34:31 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001a5e37adcc71039d5cea143992ca81b12192143eceed1a8114c57264a0890c`  
		Last Modified: Fri, 06 Oct 2023 18:53:42 GMT  
		Size: 705.0 KB (705007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec390595db475b934b401062d1536be90e45b759b779888894be324ee2be7f84`  
		Last Modified: Fri, 06 Oct 2023 19:45:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e179e8fdd708d7f2fc6079fe4f9deeea86cd34727b5dcbe315b66abf36bca252`  
		Last Modified: Fri, 06 Oct 2023 19:45:15 GMT  
		Size: 18.5 MB (18541689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.2-apache-bullseye` - linux; arm variant v7

```console
$ docker pull drupal@sha256:5d679ee92ace0a067608f6c6addc75305b0efa759d253039504620b97e172066
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.9 MB (156895425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:769526fec1c4f410a2ffe64f8addd0326b0591ac60b1b994884c7fe36889558a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:35 GMT
ADD file:551a2d9bfca9d524e2144fe06246864ea8480a1567dda26f14d99255ae6a89de in / 
# Wed, 20 Sep 2023 04:57:36 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 05:35:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 05:35:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 05:36:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 05:36:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 05:36:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 05:39:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 05:39:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 05:39:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 05:39:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 05:39:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 05:39:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:39:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:39:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 06:03:08 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 02:54:02 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 02:54:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 02:54:02 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 02:54:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 02:54:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:56:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 02:56:32 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:56:32 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 02:56:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 02:56:33 GMT
STOPSIGNAL SIGWINCH
# Sat, 30 Sep 2023 02:56:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:56:33 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 02:56:33 GMT
EXPOSE 80
# Sat, 30 Sep 2023 02:56:33 GMT
CMD ["apache2-foreground"]
# Sat, 30 Sep 2023 05:05:24 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Sep 2023 05:05:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Oct 2023 19:22:34 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Fri, 06 Oct 2023 19:22:35 GMT
ENV DRUPAL_VERSION=10.1.5
# Fri, 06 Oct 2023 19:22:35 GMT
WORKDIR /opt/drupal
# Fri, 06 Oct 2023 19:22:51 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 06 Oct 2023 19:22:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:69e0260f539f90d8f61c40f7822d9c002aa082311842094f6e640751432c0b02`  
		Last Modified: Wed, 20 Sep 2023 05:01:55 GMT  
		Size: 26.6 MB (26578623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be46d87d032255d1d74a28b22497c641d5c78de1ea10fc4274f6bfea499e940f`  
		Last Modified: Wed, 20 Sep 2023 08:28:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f420b687fd925f454f1fa714c356cfeb01d2f9cd85a7c23b07e793f2f3bbc6`  
		Last Modified: Wed, 20 Sep 2023 08:29:09 GMT  
		Size: 69.3 MB (69319721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa56685d9286db848ddaea6f14c5fa17aa60620c11cbfb41bd125c46dabe47c`  
		Last Modified: Wed, 20 Sep 2023 08:28:54 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a8915c3b049fbca34b7f6e599ec7bf349f35939f04a16dfb6080f91af5ff62`  
		Last Modified: Wed, 20 Sep 2023 08:29:29 GMT  
		Size: 18.0 MB (18008041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d19a4b9692c61fa9c1104a41acfc625d3faeca3764cbbd75d95b5c5004c98c`  
		Last Modified: Wed, 20 Sep 2023 08:29:25 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f60f7c98949aecb1037c0c58cf42d97011175abbc2d66b47b630a9209cea454`  
		Last Modified: Wed, 20 Sep 2023 08:29:25 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b323a5374d3b373ec1ab74563bfb47535478ca74c5baecc959d3c0acd20e37`  
		Last Modified: Sat, 30 Sep 2023 04:20:30 GMT  
		Size: 12.4 MB (12386245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797dd14261d1b377800c91d4e4714e99751a6f12aff45d8b5144cb747d78cc8e`  
		Last Modified: Sat, 30 Sep 2023 04:20:27 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfde6b0cc9bcb5fd13645af5eb541cfbc387dfab63c2307d3e2064cac97938f`  
		Last Modified: Sat, 30 Sep 2023 04:20:30 GMT  
		Size: 9.8 MB (9825902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ce2b34ec25fb55da244165ec026bf1d787a129229b57a9f2dfcaea519c6d4c`  
		Last Modified: Sat, 30 Sep 2023 04:20:27 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e2e5b692c1255eefe20058c17fa0c3ce353ac9c4730915c109352b4f138d42`  
		Last Modified: Sat, 30 Sep 2023 04:20:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb8b9d33f8a737ad8826de950adfb8c26138264269d464fd7949062c44a2744`  
		Last Modified: Sat, 30 Sep 2023 04:20:27 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424af30226f16412e02e0545c660ef1338accdaf577cf2c02b4d666f7dab56de`  
		Last Modified: Sat, 30 Sep 2023 05:24:56 GMT  
		Size: 1.5 MB (1524345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16606a284f41092974a3ed3fffdc8c3f482f866b9c15cc32cc0f7c06e3e2e030`  
		Last Modified: Sat, 30 Sep 2023 05:24:55 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616b0ce2865027ae1cf3f348305f93da72ff41a8d167410eab3e1d4021fc36de`  
		Last Modified: Fri, 06 Oct 2023 19:40:46 GMT  
		Size: 705.0 KB (705008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d88f40fa480a3d65d6517a096826b5cea14b56a8d99dfb0e25b3e58728ca5`  
		Last Modified: Fri, 06 Oct 2023 19:40:46 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814ac384ea15651f6789080407f3b9c04c53ca37a0f47cc17dd5dbc6201a3fc1`  
		Last Modified: Fri, 06 Oct 2023 19:41:00 GMT  
		Size: 18.5 MB (18541504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.2-apache-bullseye` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:eb5910003747e1cc2a436c1e4644151c52c59f6f8b39ef055dcd27f8e73dfbcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.7 MB (181664549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6370bf144a1d6cdb7869f6e3d601f3d879420b4c0929d3cd6affb7440f6305c0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:08:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 03:08:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 03:08:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 03:08:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 03:08:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 03:11:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 03:11:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 03:11:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 03:11:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 03:11:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 03:11:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:11:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:11:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:37:30 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 02:03:55 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 02:03:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 02:03:55 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 02:04:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 02:04:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:06:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 02:06:53 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:06:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 02:06:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 02:06:53 GMT
STOPSIGNAL SIGWINCH
# Sat, 30 Sep 2023 02:06:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:06:53 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 02:06:54 GMT
EXPOSE 80
# Sat, 30 Sep 2023 02:06:54 GMT
CMD ["apache2-foreground"]
# Sat, 30 Sep 2023 04:55:14 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Sep 2023 04:55:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Oct 2023 19:10:57 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Fri, 06 Oct 2023 19:10:57 GMT
ENV DRUPAL_VERSION=10.1.5
# Fri, 06 Oct 2023 19:10:57 GMT
WORKDIR /opt/drupal
# Fri, 06 Oct 2023 19:11:07 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 06 Oct 2023 19:11:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011d119a94c0f59e8eabde01f2b7a4da9d92360102426dcaad9d1d0be4b4092c`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2e7320620034b78e6c4122bdaf225b766ba582397845df17e1ca60098d29c`  
		Last Modified: Wed, 20 Sep 2023 06:01:20 GMT  
		Size: 86.9 MB (86929113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff55be7dadd795271386506373641b927cc6f05b8efda3e6ff839f8419b6b1`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db4302c1b3aba16628a8226cbf7e2005246794ffae23f531d4b1f22a5f1ca78`  
		Last Modified: Wed, 20 Sep 2023 06:01:37 GMT  
		Size: 19.2 MB (19170297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e803e16a6eafe2f883ecb377a60f60c91aaf73ce231424cf1a48e5e1434e9b19`  
		Last Modified: Wed, 20 Sep 2023 06:01:34 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd1d1c8a7b06ce97002de91f78a98a9436fe9afd488362c77d57314628bea87`  
		Last Modified: Wed, 20 Sep 2023 06:01:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396b7bce3a9ef60ad925edfb331e2914fad42406bd472c01d0b18c54e630d2a8`  
		Last Modified: Sat, 30 Sep 2023 03:45:08 GMT  
		Size: 12.4 MB (12387163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae12433fdbb6fbaec8a26619a675659895ac37a4d9b237e70ec825c03c1eec9`  
		Last Modified: Sat, 30 Sep 2023 03:45:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f9a49db68a395485f733b772424d7fcbbf024ea92512f78390f6bf7722be0d`  
		Last Modified: Sat, 30 Sep 2023 03:45:07 GMT  
		Size: 11.5 MB (11452112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905bf2141634d969e2a2a11830b17283fed0e273ab9bcf0fb2a371db7cbf140a`  
		Last Modified: Sat, 30 Sep 2023 03:45:05 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90cce65e385d9949ffb8ac1427cb2717069e9237fcf2dc7dfef0b96d3315bea4`  
		Last Modified: Sat, 30 Sep 2023 03:45:05 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40720355ba84cc295b435c7802b01765edcd89ac6c2068a873ccea5ecee4861a`  
		Last Modified: Sat, 30 Sep 2023 03:45:05 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9216e5f7215588fa10b62df7dfb3c81d6a42db2be7ef22c34ca3ce542e19f133`  
		Last Modified: Sat, 30 Sep 2023 05:21:16 GMT  
		Size: 2.4 MB (2408857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa600d7c9f8aa0352ec2cfb6b1319fd5dc5b0ffaa1644fbff053f3ff48d3a837`  
		Last Modified: Sat, 30 Sep 2023 05:21:15 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553038cda8328d3781919ab0d2b50c56ad8194417b4208ae971ff67e69da79c`  
		Last Modified: Fri, 06 Oct 2023 19:25:52 GMT  
		Size: 705.0 KB (705003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4328a4e527d9c40883fa1b302ce1471e5a356f4aeec81b6dc73d94bcc13cde`  
		Last Modified: Fri, 06 Oct 2023 19:25:51 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86211d2185b0227e43fe3505adc44c53a4a29f295160038898e28a39fbf537`  
		Last Modified: Fri, 06 Oct 2023 19:26:04 GMT  
		Size: 18.5 MB (18543111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.2-apache-bullseye` - linux; 386

```console
$ docker pull drupal@sha256:fcc7b81c3720cd10011d2c7829642f4feaa79470d97157fca0157014b199fc14
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.3 MB (190321303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f2fccc2f563cc7f1f8ecf414008ca471f99d35458d476b12c8b2614d2be169f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:18 GMT
ADD file:51db29acb4893b446fcf8a93f7fa809201b49d6ea62a009ab14002cafd3ac4a8 in / 
# Wed, 20 Sep 2023 00:42:18 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 01:21:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 01:21:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 01:22:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 01:22:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 01:22:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 01:27:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 01:27:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 01:28:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 01:28:11 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 01:28:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 01:28:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 01:28:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 01:28:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 02:18:28 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 02:34:23 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 02:34:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 02:34:24 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 02:34:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 02:34:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:39:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 02:39:39 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:39:40 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 02:39:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 02:39:40 GMT
STOPSIGNAL SIGWINCH
# Sat, 30 Sep 2023 02:39:40 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 30 Sep 2023 02:39:40 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 02:39:41 GMT
EXPOSE 80
# Sat, 30 Sep 2023 02:39:41 GMT
CMD ["apache2-foreground"]
# Sat, 30 Sep 2023 05:57:57 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Sep 2023 05:57:58 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Oct 2023 19:09:44 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Fri, 06 Oct 2023 19:09:44 GMT
ENV DRUPAL_VERSION=10.1.5
# Fri, 06 Oct 2023 19:09:44 GMT
WORKDIR /opt/drupal
# Fri, 06 Oct 2023 19:09:56 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 06 Oct 2023 19:09:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:091eb56f13f4be91ea9416e1b67e2c1f228b5e023f447dda2d3f5c56e57ff871`  
		Last Modified: Wed, 20 Sep 2023 00:47:36 GMT  
		Size: 32.4 MB (32397092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072459cfd581346ed5003a3895e56398debbd9b5bc065ce76657ae644b6673b0`  
		Last Modified: Wed, 20 Sep 2023 06:57:22 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02823bdeb40504f3286193851dadde3a5ecebd3f69e46b0e54b2caa3d7de8d8d`  
		Last Modified: Wed, 20 Sep 2023 06:57:45 GMT  
		Size: 92.7 MB (92723518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0441d7f8c9c59d27aae552adce64da332f052ebdd3933b61654f0c1e59819133`  
		Last Modified: Wed, 20 Sep 2023 06:57:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe1792330d2ef3c5ad46a354ef851bd3abd4ed3af02564b4fa0350804b7657`  
		Last Modified: Wed, 20 Sep 2023 06:58:10 GMT  
		Size: 19.7 MB (19737227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227c60e6580fdaab7d2dd0485719dd5398023313891d228a1e2120b28689a746`  
		Last Modified: Wed, 20 Sep 2023 06:58:02 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7dfa4f58f93f200dc90e8cc29f3062bc8c064832da286723fe9f9bc2500adc`  
		Last Modified: Wed, 20 Sep 2023 06:58:02 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df38da7bc1ce46518d6b578c8a2d17116248aeb6981a79353462813ecad26506`  
		Last Modified: Sat, 30 Sep 2023 05:24:39 GMT  
		Size: 12.4 MB (12387092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8383396f947efe16f863806f89b548e8d0e1892d232b3989574a0300611ad7`  
		Last Modified: Sat, 30 Sep 2023 05:24:36 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692e0bb6d074ef7ab30a032d5f0288406f462098bc123f29b04b1bc4cb881966`  
		Last Modified: Sat, 30 Sep 2023 05:24:39 GMT  
		Size: 11.6 MB (11613470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd809811756efdb6944c018725096df74fc236fc922e0f9697aaaa7832e737a2`  
		Last Modified: Sat, 30 Sep 2023 05:24:36 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e938e16f799211376d207e42bcafc065c38c796137747d28455b0461a91d19ba`  
		Last Modified: Sat, 30 Sep 2023 05:24:36 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0347d12f2d33d7a954bdadd25fb96835fba23e3b5e8976d643de47c8dc8248d`  
		Last Modified: Sat, 30 Sep 2023 05:24:36 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c420d4a4ac8ec4d36cf39bc4d1cee30a1f805a1c1a4bec3cdfd1a7df1e5bae8`  
		Last Modified: Sat, 30 Sep 2023 06:24:50 GMT  
		Size: 2.2 MB (2208778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1707b541c5ac73e611665db6ef12012dbb863ee9826050d7d8f00332da533c3`  
		Last Modified: Sat, 30 Sep 2023 06:24:49 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2199a7957712cdf4b2ff4b661ba35b4d019e27e6d860a5f5c7fe0b832ef0dd`  
		Last Modified: Fri, 06 Oct 2023 19:27:08 GMT  
		Size: 705.0 KB (705004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aa95cbde860bba12314d662db5a80fb671fd17fbc6e4b181a4c1f3376f3199`  
		Last Modified: Fri, 06 Oct 2023 19:27:07 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a62796e3f754fdc5c8581cbbedfa1cca0517eff001ee09c2d65affebd1c360b`  
		Last Modified: Fri, 06 Oct 2023 19:27:24 GMT  
		Size: 18.5 MB (18543091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.2-apache-bullseye` - linux; ppc64le

```console
$ docker pull drupal@sha256:b372c13a4151963a19ff034b323175c4d69cd78922afd2a1003a0be9cf2042af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187871555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3ba72cf0162472206a44000a90f5c13827f2ef0b7320e099602e559c9dbeef`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:28 GMT
ADD file:906774443118f59963ef3b425ff702af4588c1cf1d7c32f6f72fff8b1af50339 in / 
# Wed, 20 Sep 2023 07:53:30 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 21:23:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 21:23:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 21:23:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 21:23:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 21:23:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 21:28:39 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 21:28:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 21:29:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 21:29:07 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 21:29:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 21:29:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 21:29:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 21:29:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 22:07:43 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 03:13:51 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 03:13:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 03:13:52 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 03:14:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 03:14:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 03:18:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 03:19:01 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 30 Sep 2023 03:19:03 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 03:19:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 03:19:05 GMT
STOPSIGNAL SIGWINCH
# Sat, 30 Sep 2023 03:19:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 30 Sep 2023 03:19:06 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 03:19:06 GMT
EXPOSE 80
# Sat, 30 Sep 2023 03:19:06 GMT
CMD ["apache2-foreground"]
# Sat, 30 Sep 2023 08:48:52 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Sep 2023 08:48:54 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Oct 2023 18:35:38 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Fri, 06 Oct 2023 20:02:08 GMT
ENV DRUPAL_VERSION=10.1.5
# Fri, 06 Oct 2023 20:02:09 GMT
WORKDIR /opt/drupal
# Fri, 06 Oct 2023 20:02:31 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 06 Oct 2023 20:02:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:e64bfb4d4b8bfd61a4dccfc651ce802e40087cdf6029b3cbf1710fa529e70fcb`  
		Last Modified: Wed, 20 Sep 2023 08:50:44 GMT  
		Size: 35.3 MB (35291079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127f8046f674eab50dc75f55e6cef7a793000dbd8b772da271cdb68306f0ca3e`  
		Last Modified: Thu, 21 Sep 2023 00:33:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc649c20d315ba9f23db7f5d652600aabaf9708e72867362741332bd158a432`  
		Last Modified: Thu, 21 Sep 2023 00:34:10 GMT  
		Size: 86.6 MB (86636811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f3fdde26ce3630f5912d8c9fc88cb49870bda0d82b8686cca2f40a42963827`  
		Last Modified: Thu, 21 Sep 2023 00:33:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbc663291d6000412079723212b5e5a2d3c42420a02d098d9585f6e668b98a5`  
		Last Modified: Thu, 21 Sep 2023 00:34:31 GMT  
		Size: 20.5 MB (20463819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6ef81e1828442813778867428dd30fbc070f4cd52db2b477d47758ca231b1e`  
		Last Modified: Thu, 21 Sep 2023 00:34:27 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7efbe3dd0dee66401b2bf78b02c599b0cf3678eee10597a331d79e991c0285`  
		Last Modified: Thu, 21 Sep 2023 00:34:26 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2279d87b741ba9d823e3fb151c03f9a98b4bd8d0c78ef2ba34e07bbef5c7a0`  
		Last Modified: Sat, 30 Sep 2023 05:25:12 GMT  
		Size: 12.4 MB (12387830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9df486062dbec4114d0073016881027c4ef10f64761411bfd2e8885fc30fc5`  
		Last Modified: Sat, 30 Sep 2023 05:25:09 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bbab14c0a7fea5f0d9d578ceb36423a0048be4f265aefdd4329ffe7c0c3094`  
		Last Modified: Sat, 30 Sep 2023 05:25:12 GMT  
		Size: 11.8 MB (11828037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c606980f8c397a70d315ccbbbbb179a7c4d5e7eb92242787db3ea55218b112`  
		Last Modified: Sat, 30 Sep 2023 05:25:09 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a62c9e309134b643270d091b5b673e353f6b16ea5fce2c8890fd280f5de7581`  
		Last Modified: Sat, 30 Sep 2023 05:25:09 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d1cfecc35a4328eafc6d767b02b1e67a7b140bf920b36931828e7013977bcb`  
		Last Modified: Sat, 30 Sep 2023 05:25:09 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdda9b8c49acec8e9b85ae8186d0a4f852a6bc3acb57ff4dc4d851926c06f02`  
		Last Modified: Sat, 30 Sep 2023 09:31:12 GMT  
		Size: 2.0 MB (2011170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55a2d471b2fefa0d52ffd1d9ccfe88774201d6f05d67959bed7815e0f690c69`  
		Last Modified: Sat, 30 Sep 2023 09:31:12 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e571199ae462e71698099b33df7599197941e67c99d7463e4f7c3643c2fc9d38`  
		Last Modified: Fri, 06 Oct 2023 19:04:10 GMT  
		Size: 705.0 KB (705000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9ab45d0ff17af5826150de7667c87f07679d6d85b06e2d9a6175d75fae9963`  
		Last Modified: Fri, 06 Oct 2023 20:14:04 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68108f2180c451eb23ddeb1dc8058dd3850b407be8a222c37b0fdec783c845b0`  
		Last Modified: Fri, 06 Oct 2023 20:14:12 GMT  
		Size: 18.5 MB (18541760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php8.2-apache-bullseye` - linux; s390x

```console
$ docker pull drupal@sha256:216b34a3aeefd5ab1f9c46f071fd5b10c4c5158ed3c91881bc4740eafca27bcd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.2 MB (164226293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e117682d843f7fbe584e1ab81e5bc16a53f96766510d57280eb78baa138010`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:54 GMT
ADD file:02a97e0d5f41f84ac0284849646284fa41b5e324d24f4d95bb1e2419899da811 in / 
# Wed, 20 Sep 2023 02:54:57 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:28:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 03:28:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 03:28:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 03:28:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 03:28:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 03:31:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 03:31:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 03:32:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 03:32:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 03:32:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 03:32:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:32:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:32:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 03:55:51 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 30 Sep 2023 04:49:40 GMT
ENV PHP_VERSION=8.2.11
# Sat, 30 Sep 2023 04:49:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.11.tar.xz.asc
# Sat, 30 Sep 2023 04:49:41 GMT
ENV PHP_SHA256=29af82e4f7509831490552918aad502697453f0869a579ee1b80b08f9112c5b8
# Sat, 30 Sep 2023 04:49:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 04:49:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 04:51:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 04:51:58 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 30 Sep 2023 04:51:58 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 04:51:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 04:51:58 GMT
STOPSIGNAL SIGWINCH
# Sat, 30 Sep 2023 04:51:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 30 Sep 2023 04:51:59 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 04:51:59 GMT
EXPOSE 80
# Sat, 30 Sep 2023 04:51:59 GMT
CMD ["apache2-foreground"]
# Sat, 30 Sep 2023 07:48:33 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Sep 2023 07:48:35 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 10 Oct 2023 04:02:46 GMT
COPY file:fcefe3e3608e465d39adb0c083a9d7159d02b35d6481adc01191e633245d5673 in /usr/local/bin/ 
# Tue, 10 Oct 2023 04:02:46 GMT
ENV DRUPAL_VERSION=10.1.5
# Tue, 10 Oct 2023 04:02:46 GMT
WORKDIR /opt/drupal
# Tue, 10 Oct 2023 04:03:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 10 Oct 2023 04:03:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:d2d51167e651784cce0bd658d0c2caa328adef8ccf264d8c09860a95bc2a2fc6`  
		Last Modified: Wed, 20 Sep 2023 03:00:22 GMT  
		Size: 29.7 MB (29653129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a057c520bd7a3264de619d98cb953fb2d172c0b7aea904b0b97aa130e5b12a31`  
		Last Modified: Wed, 20 Sep 2023 06:00:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfba7ead31b2aac27140ca57aa96b4c0c37731ebc4757a7a1266b8da684d13`  
		Last Modified: Wed, 20 Sep 2023 06:00:22 GMT  
		Size: 71.6 MB (71631627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e1fc5603884e36dafccd7be7c611ce804bc1f7a48f7cebccf662b64d887d4b`  
		Last Modified: Wed, 20 Sep 2023 06:00:12 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7a7acda4271f62e8855bb8a12789848d0eead9e96e22022e7ebf5e8b06704a`  
		Last Modified: Wed, 20 Sep 2023 06:00:35 GMT  
		Size: 19.1 MB (19077505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109a74993364fe1681f26da5aa6d00cc0b69c9be66656cc21b2f874aa5555128`  
		Last Modified: Wed, 20 Sep 2023 06:00:32 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e53251a566b8028f68bfa3dab63725647038865cff84949e92c27d0ef3159c5`  
		Last Modified: Wed, 20 Sep 2023 06:00:32 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd40bf6579d7f989f0e00feca286b07596eb3ca4fd4de346956800fbb778724`  
		Last Modified: Sat, 30 Sep 2023 06:37:22 GMT  
		Size: 12.4 MB (12386684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1a6514d3fdef047350225024b24924faa514dea77a087789a06786127c428be`  
		Last Modified: Sat, 30 Sep 2023 06:37:20 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97cbf2d242591068a5f98d08256008e782fc6963956aada52d34d0c4009b602`  
		Last Modified: Sat, 30 Sep 2023 06:37:23 GMT  
		Size: 10.5 MB (10486103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ccfe934a45f31f31b5608e0080ece810902d53ede559899aabfa33753e86b3`  
		Last Modified: Sat, 30 Sep 2023 06:37:20 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506aa2251b168a096d66e76feb25309c62895d8bf45ce384b8de497b6e246adf`  
		Last Modified: Sat, 30 Sep 2023 06:37:20 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f767a990deb6f9ea12f4297ac63859772bad3704d5c7f332580559afcdd63b`  
		Last Modified: Sat, 30 Sep 2023 06:37:20 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbdb75b1b2fd66572997c7e47449d6e620b181e4408509778e0fb76ac825168d`  
		Last Modified: Sat, 30 Sep 2023 08:46:10 GMT  
		Size: 1.7 MB (1737303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58f02e1744c2818135e05760de3c7aa3e6fa10b11667ddc9f0a8a9daf2dd589`  
		Last Modified: Sat, 30 Sep 2023 08:46:09 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068de5dc2b688d0d9bd0e2a1e17a21d05c7978aa920f89cd839a0db5318d8efb`  
		Last Modified: Tue, 10 Oct 2023 04:43:14 GMT  
		Size: 705.0 KB (705011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5055fbc53779c22e6d913a6a6285504db79bcab468d483fb537c50df5b383d`  
		Last Modified: Tue, 10 Oct 2023 04:43:14 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4292181c1b9af130a7f9d0341d8823f0d2f326cb4bca8f9e412e4eca685a1155`  
		Last Modified: Tue, 10 Oct 2023 04:43:18 GMT  
		Size: 18.5 MB (18542896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
