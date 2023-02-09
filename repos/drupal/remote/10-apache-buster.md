## `drupal:10-apache-buster`

```console
$ docker pull drupal@sha256:ce2088d94b239badce19ec732cebd2a397577c73ec5fafe30be1af99390a29b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:10-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:21b1a556195d79db22b12e57f9df2a2c0cc67d95c88344b796e250f3c762a21b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166517568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5a315e3dbe79ebd37ce4d30fb51b605092b8ddf6a370d26c255329ee24fdb71`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:52:07 GMT
ADD file:4fbe1e3712cf37c85529cc81e0d03c82085203de00d64b0d669b5996e975925a in / 
# Sat, 04 Feb 2023 06:52:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:47:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 18:47:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 18:48:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:48:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 18:48:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 18:51:39 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 18:51:39 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 18:51:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 18:51:49 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 18:51:50 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 18:51:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 18:51:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 18:51:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 18:51:50 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 04 Feb 2023 18:51:50 GMT
ENV PHP_VERSION=8.2.2
# Sat, 04 Feb 2023 18:51:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.2.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.2.tar.xz.asc
# Sat, 04 Feb 2023 18:51:51 GMT
ENV PHP_SHA256=bdc4aa38e652bac86039601840bae01c0c3653972eaa6f9f93d5f71953a7ee33
# Sat, 04 Feb 2023 18:52:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 18:52:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 18:55:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 18:55:04 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 18:55:05 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 18:55:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 18:55:05 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 18:55:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 18:55:05 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 18:55:05 GMT
EXPOSE 80
# Sat, 04 Feb 2023 18:55:05 GMT
CMD ["apache2-foreground"]
# Sun, 05 Feb 2023 02:27:35 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 02:27:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 07 Feb 2023 01:43:17 GMT
COPY file:2c6e86189bae3d0f441696ba145d29f22860cb3f94dece0c5761829ffdb8cb91 in /usr/local/bin/ 
# Tue, 07 Feb 2023 01:43:17 GMT
ENV DRUPAL_VERSION=10.0.3
# Tue, 07 Feb 2023 01:43:17 GMT
WORKDIR /opt/drupal
# Tue, 07 Feb 2023 01:43:27 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 07 Feb 2023 01:43:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:0cf508b37688dca559387b506062329202aaf08b48be5f55f9278b2a818ad2c9`  
		Last Modified: Sat, 04 Feb 2023 06:56:58 GMT  
		Size: 27.1 MB (27140353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae08958ff1bd1856a03e2bfbae52b79c27be0d2f80bf155c8aa532f9ad46e220`  
		Last Modified: Sat, 04 Feb 2023 19:58:50 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db284214e0a94216b2a47f1bf6f9a9adf6209c7b73a59ea110027e2cb6e54469`  
		Last Modified: Sat, 04 Feb 2023 19:59:01 GMT  
		Size: 76.7 MB (76688297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881a1d9f7f864087aced46e16f6fb5f479692c06e9f75bc2b4b6f6af074a402d`  
		Last Modified: Sat, 04 Feb 2023 19:58:50 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551e93fcc836c645a28465dff51ca167571c0c7b2e51f53535a02b1f149e919c`  
		Last Modified: Sat, 04 Feb 2023 19:59:28 GMT  
		Size: 18.7 MB (18684933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2017a467471efaf04f51e06eb64ed8a4b6d76011d05fe8cd900d7b839a6f312c`  
		Last Modified: Sat, 04 Feb 2023 19:59:25 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd67da303719005dd7a8fc168c7c4e784f749d3099aa9b18d1dd3ca63d61cd8`  
		Last Modified: Sat, 04 Feb 2023 19:59:25 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d31375a2c05850f4e55c9059fae7aaea212be5f34887e69f697129f5b7c35ef`  
		Last Modified: Sat, 04 Feb 2023 19:59:26 GMT  
		Size: 12.3 MB (12276940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd54e12ecc50e996f813e313eea1187dbd39d6fd4376d4710cf0cb21c3988527`  
		Last Modified: Sat, 04 Feb 2023 19:59:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa80a855bece626107f1b4b3a747ddee340e16b007e5e1c60dc59865698e237`  
		Last Modified: Sat, 04 Feb 2023 19:59:26 GMT  
		Size: 11.3 MB (11275992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f63d80ae724c164533f764ade4dc061611d36139fee87d3b5f5d08c8bb1367`  
		Last Modified: Sat, 04 Feb 2023 19:59:23 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9af083a833d413fefb7216485f35a5ab575b70b0408e1de6abec96c7da5267`  
		Last Modified: Sat, 04 Feb 2023 19:59:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce88382d47b48e22c9c03b33329ebf925d7aa7f75bc4cc201bf42d23c752153`  
		Last Modified: Sat, 04 Feb 2023 19:59:23 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a46a916790a30ef20c638ce2ebbc79fb29a13b865ca528231f6e954ca312070`  
		Last Modified: Sun, 05 Feb 2023 02:49:08 GMT  
		Size: 2.1 MB (2090031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cd86312a08ffafa09e58e661fc3dfebb51704592452d1450fe77627f50a62`  
		Last Modified: Sun, 05 Feb 2023 02:49:08 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ebc79b6143a61a2df0c7fecd76fe123bd33c2cc4e1fd6c61f984ccebe72ee94`  
		Last Modified: Tue, 07 Feb 2023 01:59:26 GMT  
		Size: 697.1 KB (697097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69014ee61082c1040bdd6da1d868e17ee26b36de70a0a6333c7c349f172a173`  
		Last Modified: Tue, 07 Feb 2023 01:59:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a7061d295de7fcbc5f0b9f8101843f4580e0ef23fbe81763998a797e567e17`  
		Last Modified: Tue, 07 Feb 2023 01:59:30 GMT  
		Size: 17.7 MB (17657882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:e3f9360d2d5d6ff055d2a73e9743e32cf73b1e98fc97195cda6611afc7bf9799
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.7 MB (141658329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbff49b4c11153debcadfa1f30f5abc542b741904460bc4f9cbfbcd5227b6a3b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 10:00:07 GMT
ADD file:846a879e62f9818b9aa015fa10169114de528e64d1a704cdcd1e7ee2b0707dac in / 
# Sat, 04 Feb 2023 10:00:07 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:45:17 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 17:45:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 17:45:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:45:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 17:45:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 17:48:29 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 17:48:30 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 17:48:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 17:48:41 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 17:48:42 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 17:48:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 17:48:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 17:48:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 17:48:42 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 04 Feb 2023 17:48:42 GMT
ENV PHP_VERSION=8.2.2
# Sat, 04 Feb 2023 17:48:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.2.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.2.tar.xz.asc
# Sat, 04 Feb 2023 17:48:42 GMT
ENV PHP_SHA256=bdc4aa38e652bac86039601840bae01c0c3653972eaa6f9f93d5f71953a7ee33
# Sat, 04 Feb 2023 17:48:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 17:48:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:51:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 17:51:22 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:51:23 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 17:51:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 17:51:23 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 17:51:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 17:51:23 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 17:51:24 GMT
EXPOSE 80
# Sat, 04 Feb 2023 17:51:24 GMT
CMD ["apache2-foreground"]
# Sun, 05 Feb 2023 08:49:33 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 08:49:33 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 07 Feb 2023 02:18:54 GMT
COPY file:2c6e86189bae3d0f441696ba145d29f22860cb3f94dece0c5761829ffdb8cb91 in /usr/local/bin/ 
# Tue, 07 Feb 2023 02:18:54 GMT
ENV DRUPAL_VERSION=10.0.3
# Tue, 07 Feb 2023 02:18:54 GMT
WORKDIR /opt/drupal
# Tue, 07 Feb 2023 02:19:16 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 07 Feb 2023 02:19:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8f31db5a63e959a9d015a334241216fa6923a49f0bc031bde1bf336efc7a9614`  
		Last Modified: Sat, 04 Feb 2023 10:07:17 GMT  
		Size: 22.7 MB (22748916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd9c5e07ad6aabb7f2d5afcd2bd672f5ce044d8d8232c1d426c6ee304bd8089`  
		Last Modified: Sat, 04 Feb 2023 18:52:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376b0a5b355348b427e4584aa60883dc7f2c8028164154ecc5d6a971e08c2b63`  
		Last Modified: Sat, 04 Feb 2023 18:52:15 GMT  
		Size: 59.5 MB (59541437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535c3c3ca3201e7c8dd97d901114d29bfd620670e80e44af5595ad010f61f766`  
		Last Modified: Sat, 04 Feb 2023 18:52:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805381d26ffc289def52fb171e9b3a70eaf703d6ab627c8375f47a20b68079ee`  
		Last Modified: Sat, 04 Feb 2023 18:52:52 GMT  
		Size: 17.5 MB (17481422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f5cfbcbb17f5eb05e00a4ef56fbca1806ee26beeeb8b034b79780c44e7eb70`  
		Last Modified: Sat, 04 Feb 2023 18:52:49 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcbf6a55fce16e6f9531c8d3d16f32fac3fe39a6ce139ba3db7122d9d6a246e`  
		Last Modified: Sat, 04 Feb 2023 18:52:49 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f98522df50b80d28e94061b964b8706d42c9bd49dcf942b1affe4b6651c40e`  
		Last Modified: Sat, 04 Feb 2023 18:52:50 GMT  
		Size: 12.3 MB (12274956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db5b9f5f511ce9e2b921d00086672e7e9a9d093165ebc409317da8422ff8d7d`  
		Last Modified: Sat, 04 Feb 2023 18:52:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1330b12f1b2fb5bced8f02f2b75f0179ffc2f017f8bda112f08574a821890716`  
		Last Modified: Sat, 04 Feb 2023 18:52:49 GMT  
		Size: 9.8 MB (9760442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a149c7d00a8ac65e516b3aa3fa67aef7d0ca62ac7bce9e43f827f4d37ef4fb89`  
		Last Modified: Sat, 04 Feb 2023 18:52:47 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe1e9b70372083441e63c8ddb87cf613211c8773e4587d5b8795d04b727124b`  
		Last Modified: Sat, 04 Feb 2023 18:52:47 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51650831a2d11797a83c2d81a9d8cb6839869d2c119cd18d0281efccb610fbf`  
		Last Modified: Sat, 04 Feb 2023 18:52:47 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f497b2821a54a0cedaea88e86ac480495cfdb3234dc42b3275cace415b86b9a2`  
		Last Modified: Sun, 05 Feb 2023 09:22:34 GMT  
		Size: 1.5 MB (1490399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343a976be227070d47c04315e9e2a91d15587b65fafe5d6f7005d2041f23ae2f`  
		Last Modified: Sun, 05 Feb 2023 09:22:33 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05f10bbb6e09e1875c8cc6fe777716953d9d4688033711c3ad4a0801f0641042`  
		Last Modified: Tue, 07 Feb 2023 02:48:30 GMT  
		Size: 697.1 KB (697099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96f9489df9ede860486a74d68a1533259d6f5524b024df10f115434e5e4e066`  
		Last Modified: Tue, 07 Feb 2023 02:48:30 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7433ab4a203624ffc50b9761ca48a041e406bd5c05820badbc369f3b8f393c7c`  
		Last Modified: Tue, 07 Feb 2023 02:48:36 GMT  
		Size: 17.7 MB (17657768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:b9fa3570953f643f6b25f7524cef9b23458e4cd98483f349eef39e86be2c3b1c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.2 MB (159224013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2aebabe8a7e994ef6ee460acab2ea861ea50550442f736afa0e793119dc188f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:59 GMT
ADD file:442c85d39a4dbb97fb311e1f30e76f5d197339db3967532742e299fa73410f89 in / 
# Thu, 09 Feb 2023 03:58:59 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 05:39:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 05:39:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 05:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 05:40:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 05:40:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 05:43:05 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 09 Feb 2023 05:43:05 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 09 Feb 2023 05:43:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 09 Feb 2023 05:43:14 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 09 Feb 2023 05:43:14 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 09 Feb 2023 05:43:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:43:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:43:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 05:43:14 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 09 Feb 2023 05:43:14 GMT
ENV PHP_VERSION=8.2.2
# Thu, 09 Feb 2023 05:43:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.2.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.2.tar.xz.asc
# Thu, 09 Feb 2023 05:43:15 GMT
ENV PHP_SHA256=bdc4aa38e652bac86039601840bae01c0c3653972eaa6f9f93d5f71953a7ee33
# Thu, 09 Feb 2023 05:43:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 09 Feb 2023 05:43:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 09 Feb 2023 05:46:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 09 Feb 2023 05:46:13 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 09 Feb 2023 05:46:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 09 Feb 2023 05:46:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 09 Feb 2023 05:46:14 GMT
STOPSIGNAL SIGWINCH
# Thu, 09 Feb 2023 05:46:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 09 Feb 2023 05:46:14 GMT
WORKDIR /var/www/html
# Thu, 09 Feb 2023 05:46:14 GMT
EXPOSE 80
# Thu, 09 Feb 2023 05:46:14 GMT
CMD ["apache2-foreground"]
# Thu, 09 Feb 2023 14:24:24 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 14:24:25 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 09 Feb 2023 14:24:25 GMT
COPY file:2c6e86189bae3d0f441696ba145d29f22860cb3f94dece0c5761829ffdb8cb91 in /usr/local/bin/ 
# Thu, 09 Feb 2023 14:24:25 GMT
ENV DRUPAL_VERSION=10.0.3
# Thu, 09 Feb 2023 14:24:25 GMT
WORKDIR /opt/drupal
# Thu, 09 Feb 2023 14:24:48 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 09 Feb 2023 14:24:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:ebcd4e3db076a77234a526ba23bdac8b205f7d74fd052a936cfa190b42cf49aa`  
		Last Modified: Thu, 09 Feb 2023 04:03:14 GMT  
		Size: 25.9 MB (25922825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb59936b35f83df7e783b83adade014dde2600b8c66c7f156646724c0590c7a`  
		Last Modified: Thu, 09 Feb 2023 06:39:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483b7b021f35118cd09f08960f1af17be5a48449550af0f339bed3b0827a9baf`  
		Last Modified: Thu, 09 Feb 2023 06:39:44 GMT  
		Size: 70.4 MB (70362430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01c942918fd594cbfd67ad58a43f5f196e39ee36cd9395c7d0b3a87ebfb96e9`  
		Last Modified: Thu, 09 Feb 2023 06:39:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524358ce06edb34679f90c7960a1ae16533f51329eda372d0fef9d3e4b77970c`  
		Last Modified: Thu, 09 Feb 2023 06:40:11 GMT  
		Size: 18.6 MB (18583841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50b57b27c058d020a4257f4c0fc8b20fa0fc5d6ef54d70240156d936d24c797`  
		Last Modified: Thu, 09 Feb 2023 06:40:08 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fa49151627f6be68378b677fd0734801eea966b8fff3c12e2f042449b02133`  
		Last Modified: Thu, 09 Feb 2023 06:40:08 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab3b412ac9bf28ed11e7279033005326adab9cc44b785433a007f45fc20b8b6`  
		Last Modified: Thu, 09 Feb 2023 06:40:09 GMT  
		Size: 12.3 MB (12275734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8029c03147b5acaf8f286d8bfd04d3cb0dc09cfbc3a6d42291ba6bda0387ef07`  
		Last Modified: Thu, 09 Feb 2023 06:40:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab55288da371a81238c07857f387e7db1a3c63af2f441e62d72e201762ba2652`  
		Last Modified: Thu, 09 Feb 2023 06:40:08 GMT  
		Size: 11.4 MB (11360028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b0a350bde3187e19641081d92107fcfb47f1e8f5c92d46a7a55ddaf4cf37e2`  
		Last Modified: Thu, 09 Feb 2023 06:40:07 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d29619133dd0970dffe356445cc81cd2327ccdcfa776277f5376cb49b07aabf`  
		Last Modified: Thu, 09 Feb 2023 06:40:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ef5841bdd8b5b78085a15f9ce3be90446970db8f7ebdd49a894d4904881e38`  
		Last Modified: Thu, 09 Feb 2023 06:40:07 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d028deaff647e44ea949dc01f668bf2d4a2374b6385ab61ce351449ad030090`  
		Last Modified: Thu, 09 Feb 2023 14:47:03 GMT  
		Size: 2.4 MB (2358175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889ebd969f902605ba7271d5b3340d7fd0d5e7cb0d05cea0456b0bb82b8facb2`  
		Last Modified: Thu, 09 Feb 2023 14:47:02 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c6bc2832f35b229e6c73920322b5c616f88cab31913dd9eb38610958352578`  
		Last Modified: Thu, 09 Feb 2023 14:47:03 GMT  
		Size: 697.1 KB (697101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf3a355733b1c2be412078ea422401f442e3997451d3cbbea9d16e71ab503d6`  
		Last Modified: Thu, 09 Feb 2023 14:47:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389050158b4537765f0b02baa389e26fccd7f71844ef6ed07425adc17b643a0f`  
		Last Modified: Thu, 09 Feb 2023 14:47:06 GMT  
		Size: 17.7 MB (17657843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:041a2b39774a335d3508bc7ef3077b640d447edc7acd717822966a3d54747252
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.8 MB (171819375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8a3809042fbceb4fb9dbd1df7524e517e4a5ef406fed19662421390e1584fde`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:48 GMT
ADD file:060bbacc8df3d1b157ff409535b3ea29dd0b5667425e3dcf6e60556dcfa4e7f1 in / 
# Sat, 04 Feb 2023 07:49:48 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 14:30:07 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 14:30:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 14:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 14:30:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 14:30:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 14:33:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 14:33:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 14:34:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 14:34:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 14:34:04 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 14:34:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 14:34:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 14:34:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 14:34:07 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 04 Feb 2023 14:34:08 GMT
ENV PHP_VERSION=8.2.2
# Sat, 04 Feb 2023 14:34:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.2.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.2.tar.xz.asc
# Sat, 04 Feb 2023 14:34:10 GMT
ENV PHP_SHA256=bdc4aa38e652bac86039601840bae01c0c3653972eaa6f9f93d5f71953a7ee33
# Sat, 04 Feb 2023 14:34:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 14:34:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:37:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 14:37:06 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:37:07 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 14:37:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 14:37:08 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 14:37:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 14:37:10 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 14:37:11 GMT
EXPOSE 80
# Sat, 04 Feb 2023 14:37:12 GMT
CMD ["apache2-foreground"]
# Sat, 04 Feb 2023 23:30:11 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 23:30:12 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 04 Feb 2023 23:30:14 GMT
COPY file:e2da1c2113094da76d330eef39e0e1916af11394dff778e02af557c116266d7c in /usr/local/bin/ 
# Sat, 04 Feb 2023 23:30:14 GMT
ENV DRUPAL_VERSION=10.0.3
# Sat, 04 Feb 2023 23:30:15 GMT
WORKDIR /opt/drupal
# Sat, 04 Feb 2023 23:30:27 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Sat, 04 Feb 2023 23:30:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8e0d975bedf8c90406704c677df48435cd2d53449ac9ab15a876323ceb95ff8f`  
		Last Modified: Sat, 04 Feb 2023 07:55:52 GMT  
		Size: 27.8 MB (27798503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7530cf666fff6e57c2fd7b789b76bf7b9512b00c5d78ed4d83019d31c306e105`  
		Last Modified: Sat, 04 Feb 2023 15:42:40 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdb983fe81a5de6de33350ecbdd92cb52b3afb4f1d1d693c6384470024c6940`  
		Last Modified: Sat, 04 Feb 2023 15:42:51 GMT  
		Size: 81.2 MB (81235952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4035ed3a2e1d31e52d608036c5e463521bd61f242d5c91be4dd94cecd412b6d2`  
		Last Modified: Sat, 04 Feb 2023 15:42:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98abcc7f65763b73045c0d8135d34b1cb01fb29e49166288419c274222a2c80`  
		Last Modified: Sat, 04 Feb 2023 15:43:24 GMT  
		Size: 18.9 MB (18900914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:050e57b192e06f27e9d7c200c20e1993e9c8ebe059f008ec74709b1b399c9435`  
		Last Modified: Sat, 04 Feb 2023 15:43:21 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bc2168488272c2b60614ea16b164dfa7a80886809af6f6497eeb098a6a56b9d`  
		Last Modified: Sat, 04 Feb 2023 15:43:21 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300da7946c974e6a6ca61e63fdc9099a7e91b5198d0b6d6555a44b6aebd9227b`  
		Last Modified: Sat, 04 Feb 2023 15:43:23 GMT  
		Size: 12.1 MB (12061769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8dcf9a369555d99f52ba6fce799a9e9b43dbda3733c06c866780cd80fd2092`  
		Last Modified: Sat, 04 Feb 2023 15:43:19 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32e08e314975da2b9e74f1fe3c1eb43808219575224a0d5bf1d911e35ec7eb1`  
		Last Modified: Sat, 04 Feb 2023 15:43:21 GMT  
		Size: 11.5 MB (11515022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b820652b1e9ff30346e4dda1c0c9d99f6bae5bb5dcfa004b75759cc49c2fa8`  
		Last Modified: Sat, 04 Feb 2023 15:43:20 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943a64951e4a524fb7395cef0b7e8a7112110f92ea6b463c21f30a13a97e3a63`  
		Last Modified: Sat, 04 Feb 2023 15:43:19 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8a9dad6b091ef18fe824af2255ac29c193a002795e8e3d75f524981cfbdd07`  
		Last Modified: Sat, 04 Feb 2023 15:43:19 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb89b775dbe581a306d6e9e50b52c48f3acae38ea38a44fcf3ce59d0e73d373`  
		Last Modified: Sat, 04 Feb 2023 23:59:19 GMT  
		Size: 1.9 MB (1946507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7adc342de900580f40ea8f23686b7d49fea8d1faa57cc42a11ba65c2f57f5a4`  
		Last Modified: Sat, 04 Feb 2023 23:59:18 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d52cbbb4987f73bba984c102e67a6ae8f23423cce54e40f3ae1ed862232efe9`  
		Last Modified: Sat, 04 Feb 2023 23:59:19 GMT  
		Size: 695.2 KB (695204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1290cf2ce0bce172220fb88bc9fb81ee6e9a57bd7991ea20cd323d197d99e7`  
		Last Modified: Sat, 04 Feb 2023 23:59:18 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fa860710cb662d0733138a85e16159c7e82538374883df6c3f6eb23d61a945`  
		Last Modified: Sat, 04 Feb 2023 23:59:23 GMT  
		Size: 17.7 MB (17659611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
