## `drupal:7-apache`

```console
$ docker pull drupal@sha256:a9f2153bb93a041e9d4378ec54539dee6f3d0daacb0c57e24189eecfa71045a0
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

### `drupal:7-apache` - linux; amd64

```console
$ docker pull drupal@sha256:f4053f0aaabc47eb9015c190fc544709cd176bf451daa83de137d7e0ea61b49e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.6 MB (168584596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb64f2abc9b26d603fca548b6e89538dc8b1ed6016788bd807e1934619b566b0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 09:45:07 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 09:45:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 09:45:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 09:45:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 09:45:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 09:48:45 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 09:48:45 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 09:48:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 09:48:54 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 09:48:54 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 09:48:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:48:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:48:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 11:07:02 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 13 Sep 2022 11:07:02 GMT
ENV PHP_VERSION=7.4.30
# Tue, 13 Sep 2022 11:07:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 13 Sep 2022 11:07:02 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 13 Sep 2022 11:07:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 11:07:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:09:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 11:09:18 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:09:19 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 11:09:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 11:09:19 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 11:09:19 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:09:19 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 11:09:19 GMT
EXPOSE 80
# Tue, 13 Sep 2022 11:09:19 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 18:39:48 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 18:39:48 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 18:47:11 GMT
ENV DRUPAL_VERSION=7.92
# Tue, 13 Sep 2022 18:47:11 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Tue, 13 Sep 2022 18:47:13 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad30ef427bea3618f38ae67475db13c5b65eb0614aba841828d870d674b95371`  
		Last Modified: Tue, 13 Sep 2022 11:28:23 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deeb65fd0ffbe39e5bf2df35ff8531c9c9f3cbea72ee32f2513282eb1279268a`  
		Last Modified: Tue, 13 Sep 2022 11:28:36 GMT  
		Size: 91.6 MB (91633603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136a0d294b5e7cad81e1688610e721299e60d71c66a47e440884e77b30e62841`  
		Last Modified: Tue, 13 Sep 2022 11:28:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d44545310ede55d8b331f7fd70d6cd719e94994cd0439ad6d3aa2168b781cb`  
		Last Modified: Tue, 13 Sep 2022 11:29:09 GMT  
		Size: 19.2 MB (19244950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d7b00e32064640e29f1045945f831902a8a7adff90fdf891bae602738a5f53`  
		Last Modified: Tue, 13 Sep 2022 11:29:07 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:294cc749e981bf3c408329b165b5e5bc613b43287386ca6728b1451b782056ef`  
		Last Modified: Tue, 13 Sep 2022 11:29:07 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff4a4a9529ce8a137de0713d25a6f69457b89985805b6d54f148f1ba435bbf0`  
		Last Modified: Tue, 13 Sep 2022 11:40:30 GMT  
		Size: 10.8 MB (10758924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c181669adae49d6c6f98cbeeaae5b67c59309af2e2cd2c3fcc76e747be9067de`  
		Last Modified: Tue, 13 Sep 2022 11:40:27 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcb4eb3e9c0b34654c865c6c1587a73ba6c2cdd032d635f57e7062d44b943be`  
		Last Modified: Tue, 13 Sep 2022 11:40:28 GMT  
		Size: 10.2 MB (10197032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca42b58ec080ac0793ca4d506f1e42f82c382bcf6131c284a5729fa67c5aa20c`  
		Last Modified: Tue, 13 Sep 2022 11:40:26 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff2a009e44cb4255bd3eb27259d1dafe47fccc9b7874581a273857b98231181`  
		Last Modified: Tue, 13 Sep 2022 11:40:26 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7fca748a1a828d7612a9c2aea7c576c3d3f41f761f626b0792c63ef07d5eb4`  
		Last Modified: Tue, 13 Sep 2022 11:40:26 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519791d04dc7c8a46e56fc2ef7dad0e26ac43e0cf344fe35a3181871be8f1d99`  
		Last Modified: Tue, 13 Sep 2022 19:02:01 GMT  
		Size: 1.9 MB (1943231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6139cbc4c84c4bf8655ecd7380a3d6d62ac490e7945760523a355df3ac5fe301`  
		Last Modified: Tue, 13 Sep 2022 19:02:01 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af34a11399f0875d1127c241317ed07a08eb0cd28d5caf9e492edc2e9c27cf73`  
		Last Modified: Tue, 13 Sep 2022 19:10:37 GMT  
		Size: 3.4 MB (3396839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache` - linux; arm variant v5

```console
$ docker pull drupal@sha256:2eabb747a6fd3d2078b80fdbca6d5abcb3c0c4e48d322771f362aac9dcd1d5a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146652874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3a08b274992bbeb639d65a45e5dc61b2c640b6bc23c2729dd71343bafbb891b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 00:53:30 GMT
ADD file:539e23f1c3a625a612a5a59b3939e9692c86c3cfa4956d30f4802c9f34ffa29c in / 
# Tue, 13 Sep 2022 00:53:31 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:31:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 07:31:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 07:31:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:31:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 07:31:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 07:39:18 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 07:39:18 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 07:39:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 07:39:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 07:39:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 07:39:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 07:39:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 07:39:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 09:29:53 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 13 Sep 2022 09:29:54 GMT
ENV PHP_VERSION=7.4.30
# Tue, 13 Sep 2022 09:29:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 13 Sep 2022 09:29:54 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 13 Sep 2022 09:30:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 09:30:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 09:35:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 09:35:40 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 09:35:40 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 09:35:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 09:35:41 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 09:35:41 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 09:35:41 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 09:35:41 GMT
EXPOSE 80
# Tue, 13 Sep 2022 09:35:41 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 17:37:02 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 17:37:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 17:37:03 GMT
ENV DRUPAL_VERSION=7.92
# Tue, 13 Sep 2022 17:37:03 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Tue, 13 Sep 2022 17:37:05 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:705abbab4fcb3a8dfe046a2ae6c450328aa11d93911abce66d3bba8bc693cbd4`  
		Last Modified: Tue, 13 Sep 2022 01:01:07 GMT  
		Size: 28.9 MB (28905288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99efe79d5c9446f0a5c0af85ea81891a7846fc47b18565a7ed579dfd03d22466`  
		Last Modified: Tue, 13 Sep 2022 09:55:29 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fe2b2c56e09d8fbfa17cf0d926221cfaaa384710b41971a8932c042d4e09bd`  
		Last Modified: Tue, 13 Sep 2022 09:55:51 GMT  
		Size: 73.7 MB (73686919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7764660ce43a68f00f900f7533e4f6a75f794d603904d830851fc9729f194a`  
		Last Modified: Tue, 13 Sep 2022 09:55:29 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9d561f60baa0d2e7d517f71be03ef4cd45082da12157c6bbf3538303881bfb`  
		Last Modified: Tue, 13 Sep 2022 09:56:36 GMT  
		Size: 18.6 MB (18553933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db79cca54a31526037c1348137c9b31f00aa0dd695a276cbc3d79c7112b128f2`  
		Last Modified: Tue, 13 Sep 2022 09:56:31 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5f65d52d96eff36632d37197a65abb455e660162bc7ff1f379f1f138c7d66d`  
		Last Modified: Tue, 13 Sep 2022 09:56:31 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f16713637395093219e4ca338c57fd81f78b7e97407874767fe938193c782e1`  
		Last Modified: Tue, 13 Sep 2022 10:04:39 GMT  
		Size: 10.8 MB (10757404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f215ab8a4df505c118050d83bd2be3cfb6bf632f636e7c9536b3c8c3e7ceff9`  
		Last Modified: Tue, 13 Sep 2022 10:04:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b131867b0df02ca0d7382e91f1481ef3d365fc312d8cf98b0eff843c73a83791`  
		Last Modified: Tue, 13 Sep 2022 10:04:39 GMT  
		Size: 9.6 MB (9572916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5877e8edd4d60b0b771f128af396639195648feee21acd7a6f4da9bc65a87996`  
		Last Modified: Tue, 13 Sep 2022 10:04:35 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be72df30b0695ba8688681cb80d19ff0d2ce4ee06fac9052c8a62bd84c152cc8`  
		Last Modified: Tue, 13 Sep 2022 10:04:35 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884db09a4dda38db5bf1eefc7e05c6032ef1002981fd1c2d2e553ae31ac979fa`  
		Last Modified: Tue, 13 Sep 2022 10:04:35 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eb0142b93febae1b66fef8aee1dafb4e75fc96d1d0113540d18d6c64123412`  
		Last Modified: Tue, 13 Sep 2022 17:41:07 GMT  
		Size: 1.8 MB (1773684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62aaebef338c2b52240873770ee54df642826375a6de2a0d27fa71cdc6f11e5c`  
		Last Modified: Tue, 13 Sep 2022 17:41:06 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed6351e82fb0a9683e79b3d70ad4f03a0f8fed581129a7e6b1eaf0bbee42927`  
		Last Modified: Tue, 13 Sep 2022 17:41:08 GMT  
		Size: 3.4 MB (3396829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache` - linux; arm variant v7

```console
$ docker pull drupal@sha256:8f9621fcf42be75e439ad7ca24552cabb3bc55b1e4d3b2ceff76ef0557508a8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.8 MB (138779414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ee296f71275e1a3a75d1a0db651aff1ba6a0d095ff63a8ede0e3bfcdafb54e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 03:42:37 GMT
ADD file:04b0c48a2d326e2ac4255df4a6165508f0d29d8a32147fb8df6bf9504b8f6b09 in / 
# Tue, 13 Sep 2022 03:42:37 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 19:13:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 19:13:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 19:14:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 19:14:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 19:14:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 19:21:45 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 19:21:45 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 19:21:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 19:21:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 19:21:59 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 19:21:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 19:21:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 19:21:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 23:02:35 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 13 Sep 2022 23:02:35 GMT
ENV PHP_VERSION=7.4.30
# Tue, 13 Sep 2022 23:02:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 13 Sep 2022 23:02:35 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 13 Sep 2022 23:02:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 23:02:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 23:08:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 23:08:14 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 23:08:15 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 23:08:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 23:08:15 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 23:08:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 23:08:15 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 23:08:15 GMT
EXPOSE 80
# Tue, 13 Sep 2022 23:08:16 GMT
CMD ["apache2-foreground"]
# Thu, 15 Sep 2022 00:03:12 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 15 Sep 2022 00:03:13 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Sep 2022 00:16:04 GMT
ENV DRUPAL_VERSION=7.92
# Thu, 15 Sep 2022 00:16:04 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Thu, 15 Sep 2022 00:16:05 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:43caeee1782255456dd3403ae8e6ba191802c3deb004ca68ce0420b30368995d`  
		Last Modified: Tue, 13 Sep 2022 03:49:46 GMT  
		Size: 26.6 MB (26567059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52628763237e3b562ec4c9ca1588341c32a5b17d78c89bb7c0f319887ed2770b`  
		Last Modified: Wed, 14 Sep 2022 00:04:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5a1b10616371cbe99bfb9ca7199a1ed9fea4e6999376a9e770edea1a316415`  
		Last Modified: Wed, 14 Sep 2022 00:04:51 GMT  
		Size: 69.3 MB (69320254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ffb320db3fed1509d190e30ef29ff6d6770441b99e1645c16934c386e8dc89`  
		Last Modified: Wed, 14 Sep 2022 00:04:31 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456bb04520bf4cb2dcb047307f740751a1b0baf82e31156ab0b7914ea4669ab9`  
		Last Modified: Wed, 14 Sep 2022 00:05:37 GMT  
		Size: 18.0 MB (17998119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc3c76556abb0fc34d414ffdc6bd159244aa83e8b204c0ab84e936a72c6d920`  
		Last Modified: Wed, 14 Sep 2022 00:05:32 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e42b556031c60530e6be320e3b7ac03254debdaae944c84f628d38e03870ca0`  
		Last Modified: Wed, 14 Sep 2022 00:05:32 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfecd24178903f0cbdbfe2f86fc28b5ac2e20a688ec5230962afe98f9531d41`  
		Last Modified: Wed, 14 Sep 2022 00:20:18 GMT  
		Size: 10.8 MB (10757446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08274eb1ff055b49a5f8e89240bf11de0f61de2f45b760b42433f35e83216dab`  
		Last Modified: Wed, 14 Sep 2022 00:20:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb5990fbcf2f2c30ad95dc0bdd6f0cd696141b02eceb8d31e9bdd0971782ff9`  
		Last Modified: Wed, 14 Sep 2022 00:20:17 GMT  
		Size: 9.1 MB (9088192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d965a3be5447fc6b324b028bc8be37ea0faab713e0882b829fe7760e83e820a`  
		Last Modified: Wed, 14 Sep 2022 00:20:14 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f569c2a2177ab7685b46fa1fa0a16111f2b38ca39aac9f5dc50f6b182dee55a`  
		Last Modified: Wed, 14 Sep 2022 00:20:14 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ca2e4348726cdfa695bd4b157c7dff79aa87fc69f47dcd4c53d8c16a9e6013`  
		Last Modified: Wed, 14 Sep 2022 00:20:14 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c256578145d1d5e4a228d223f34aa572cb753167a817dd86f028d847b6ea8ca`  
		Last Modified: Thu, 15 Sep 2022 00:42:22 GMT  
		Size: 1.6 MB (1645601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae29ba5331ddc2eb78513943e94afecf0ed56c77d3c190f42393d2d4d2eebcf0`  
		Last Modified: Thu, 15 Sep 2022 00:42:22 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b61339865356aa9d0ff0642f9f1390d35ba873e1d7990247c194d75885f06b`  
		Last Modified: Thu, 15 Sep 2022 00:54:53 GMT  
		Size: 3.4 MB (3396849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:c4066116ea29bc2dcb28e2785e1e53aceb2d5bba844e249f61121a2f2bfbc157
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.6 MB (161577214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b267b27e174ade0575ed3ba3e3a14de928b89a557047fbbb6827cc4c96cd22f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 09:53:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 09:53:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 09:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 09:53:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 09:53:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 09:58:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 09:58:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 09:58:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 09:58:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 09:58:18 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 09:58:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:58:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:58:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 11:27:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 13 Sep 2022 11:27:48 GMT
ENV PHP_VERSION=7.4.30
# Tue, 13 Sep 2022 11:27:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 13 Sep 2022 11:27:50 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 13 Sep 2022 11:28:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 11:28:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:29:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 11:29:53 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:29:53 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 11:29:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 11:29:55 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 11:29:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:29:57 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 11:29:58 GMT
EXPOSE 80
# Tue, 13 Sep 2022 11:29:59 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 20:06:08 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 20:06:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 20:18:20 GMT
ENV DRUPAL_VERSION=7.92
# Tue, 13 Sep 2022 20:18:21 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Tue, 13 Sep 2022 20:18:23 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fd9a4eb0be0c31ebe8b629af97161c7aeb7ba560b02ecb344ed96dc24794f7`  
		Last Modified: Tue, 13 Sep 2022 11:53:45 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa6592a3fc821840b04f25b635ae6239707e725a6cc5e7f4b8ed7cca15bc21a`  
		Last Modified: Tue, 13 Sep 2022 11:53:57 GMT  
		Size: 86.9 MB (86925053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c316363f6ab23bd46440cf834debf44919ab7a0deb4f86a4f57d7530744101a0`  
		Last Modified: Tue, 13 Sep 2022 11:53:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4c1923eb753ecfd4a7c9271ae20e3219b5f835c5a627811dcc7eefa651618a`  
		Last Modified: Tue, 13 Sep 2022 11:54:32 GMT  
		Size: 19.0 MB (18950417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527169df94894a18a2ad0bea7141c5f25627c02cafce5814316ad2fb8a998c48`  
		Last Modified: Tue, 13 Sep 2022 11:54:30 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1151c54f17a6b0e2f49acff5ea5f2f3ba358eeee930cfdf47eff12c9b4b9f6a1`  
		Last Modified: Tue, 13 Sep 2022 11:54:30 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269fd8a860a37b6f4474a19becb74791f214f75eab40eadac048b4862be39109`  
		Last Modified: Tue, 13 Sep 2022 12:06:02 GMT  
		Size: 10.5 MB (10543215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9a74a58ef50b57d33588213b05b0cacc01224a112ed8cf2d902384ed2ef740`  
		Last Modified: Tue, 13 Sep 2022 12:05:59 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11034d7a2e3d7b29edfda11acff4aee360802badc99b2ef075a2404723919ee`  
		Last Modified: Tue, 13 Sep 2022 12:06:02 GMT  
		Size: 10.0 MB (9998909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b004258dd36a7b5b393a8c4649d3947c6a7cbacb1b668d9addcc48319bb572`  
		Last Modified: Tue, 13 Sep 2022 12:05:59 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6480b54bf732e6002edecf9a1257f2101816279b8806dc878e9904577a0fbcce`  
		Last Modified: Tue, 13 Sep 2022 12:05:59 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d922b3376c359da854f9399b7d6a8372a29b65765620a77af56852910c6ec0`  
		Last Modified: Tue, 13 Sep 2022 12:05:59 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b44f302559d6a1e5fbc20582e44a28a5b8f66c22f0d43c58ed87480faa14dd5`  
		Last Modified: Tue, 13 Sep 2022 20:39:30 GMT  
		Size: 1.7 MB (1703041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7dff1de35c95130659afc975705e5719b1812be19f2988c3e8d257e5839e50`  
		Last Modified: Tue, 13 Sep 2022 20:39:29 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a934f4158a99f06870cf581598824686f6c69416b2f1a8ea7bf56f9a2e642f0`  
		Last Modified: Tue, 13 Sep 2022 20:48:54 GMT  
		Size: 3.4 MB (3396560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache` - linux; 386

```console
$ docker pull drupal@sha256:354965608a7c813ae68c65b756cd6348069b5628e19264b3807bda7b5dcd2f12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.8 MB (170818754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d29c4f3fa7230acfd36cd9694ea77d53a97cb9e8ac113795a8062255bb62cc0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 01:39:44 GMT
ADD file:414dad8d6231b19eca031ae43d450f7b700460907f7319c029b542ab528c5f9b in / 
# Tue, 13 Sep 2022 01:39:45 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:00:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 10:01:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 10:01:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 10:01:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 10:01:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 10:04:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 10:04:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 10:04:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 10:04:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 10:04:54 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 10:04:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 10:04:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 10:04:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 11:21:11 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 13 Sep 2022 11:21:11 GMT
ENV PHP_VERSION=7.4.30
# Tue, 13 Sep 2022 11:21:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 13 Sep 2022 11:21:13 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 13 Sep 2022 11:21:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 11:21:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:23:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 11:23:08 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:23:08 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 11:23:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 11:23:10 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 11:23:12 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 11:23:12 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 11:23:13 GMT
EXPOSE 80
# Tue, 13 Sep 2022 11:23:14 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 18:21:20 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 18:21:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 18:31:21 GMT
ENV DRUPAL_VERSION=7.92
# Tue, 13 Sep 2022 18:31:21 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Tue, 13 Sep 2022 18:31:23 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:221c5dcdb82ed8982a21341b5c0cadf79cc338347a649dc99854a5697661d7aa`  
		Last Modified: Tue, 13 Sep 2022 01:45:21 GMT  
		Size: 32.4 MB (32383788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d1e34bd845edb47943a1881d00a75a80a41e489593e95fc7c0b8443d9f815e`  
		Last Modified: Tue, 13 Sep 2022 11:46:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6a71ef2453ac6b8c43691f9f7de7823b722a65644b3504bf29d97aac5ed480`  
		Last Modified: Tue, 13 Sep 2022 11:46:49 GMT  
		Size: 92.7 MB (92716566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e0024de959dd3b0a0fffdc3828a6b1ee777b6a4bb9bd420d03bf927300063e`  
		Last Modified: Tue, 13 Sep 2022 11:46:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d8a9e50329b2b3ab8e7035fb56b3e9b128ff6aef01d9e13cb8ca4465735489`  
		Last Modified: Tue, 13 Sep 2022 11:47:25 GMT  
		Size: 19.5 MB (19515749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd16c1634a57c531a76d5102cbcf5ed317c2d124df0a25155838ec3be00597e7`  
		Last Modified: Tue, 13 Sep 2022 11:47:22 GMT  
		Size: 428.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64397695a1376f7a914ef27bd6a14ddd3480c3ab5c7032dae80fab1fad681f8`  
		Last Modified: Tue, 13 Sep 2022 11:47:22 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50bdbaeeabaa3195e76f009eaad75fc4bc81d1f2a955f49f2605affb5929a9b7`  
		Last Modified: Tue, 13 Sep 2022 11:59:15 GMT  
		Size: 10.5 MB (10543204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c546bc7817abbf6432e7bc0d3ea25b08be4a1bf84eda0fb5eafbad90a6fad3d8`  
		Last Modified: Tue, 13 Sep 2022 11:59:11 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed36a0f6f2c717477b946c1a0d6e2330d8c554c3d4261fe63352d93890c34633`  
		Last Modified: Tue, 13 Sep 2022 11:59:13 GMT  
		Size: 10.4 MB (10442034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539513ace5f71d142b4d848c847b87cbb0044380952fcc3b4fc781cc796eee02`  
		Last Modified: Tue, 13 Sep 2022 11:59:11 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4836658e12e145a85979e75919966d2ec68fb52e985c99e797c7071a6ccbc538`  
		Last Modified: Tue, 13 Sep 2022 11:59:11 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6de10b59d6a43c4c0c59584f66eeeb64e18798c6f289a8a675909c7ded92e4`  
		Last Modified: Tue, 13 Sep 2022 11:59:12 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca8c6bca1226eaf50a50f1357fa96c50e3883fd1f0b03888b47b56b055e1e29`  
		Last Modified: Tue, 13 Sep 2022 18:55:09 GMT  
		Size: 1.8 MB (1815072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291fc25327a380dc8c0753081da07ca92727c9eee9374d89c33c55c69bc1f117`  
		Last Modified: Tue, 13 Sep 2022 18:55:09 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c08120e00e2b918fdfbbef5ef7910d41f4b070a0ea0440eb73640f48510acb`  
		Last Modified: Tue, 13 Sep 2022 19:04:55 GMT  
		Size: 3.4 MB (3396563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache` - linux; mips64le

```console
$ docker pull drupal@sha256:b09a7b5b6d36477d708b954ca20c22f4edb5d265848f38f2ad9eea8b87ad9f26
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.9 MB (145891371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a1b3cdbb9eb5e64ee549a41c4028cad9a17ca14e77f875d22bbefe050ad2666`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 01:10:58 GMT
ADD file:91a8d8627a614ff3741d68216da46f13b393e52a70377b97ef317e4a00a3cac6 in / 
# Tue, 13 Sep 2022 01:11:02 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 10:56:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 10:56:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 10:58:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 10:58:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 10:58:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 11:13:03 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 11:13:06 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 11:13:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 11:14:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 11:14:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 11:14:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 11:14:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 11:14:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 13:57:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 13 Sep 2022 13:58:01 GMT
ENV PHP_VERSION=7.4.30
# Tue, 13 Sep 2022 13:58:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 13 Sep 2022 13:58:08 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 13 Sep 2022 13:58:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 13:58:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 14:07:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 14:07:35 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 14:07:41 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 14:07:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 14:07:49 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 14:07:52 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 14:07:55 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 14:07:59 GMT
EXPOSE 80
# Tue, 13 Sep 2022 14:08:02 GMT
CMD ["apache2-foreground"]
# Wed, 14 Sep 2022 01:03:41 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Sep 2022 01:03:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 14 Sep 2022 01:03:50 GMT
ENV DRUPAL_VERSION=7.92
# Wed, 14 Sep 2022 01:03:54 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Wed, 14 Sep 2022 01:04:03 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:98abeb1446d0e9df6f48d5f72a70b36598cfc1091c9a5ca82690bedcf320e2b3`  
		Last Modified: Tue, 13 Sep 2022 01:18:50 GMT  
		Size: 29.6 MB (29627659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d398b60506f9fff4beffdf2d731ecd850964f1262a37053f0489b99010db3f4`  
		Last Modified: Tue, 13 Sep 2022 14:31:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d716b9e19bf21605eb5a455ab1250fb711828d598d59cf031eac8b30cb1cc0c`  
		Last Modified: Tue, 13 Sep 2022 14:32:18 GMT  
		Size: 72.0 MB (72017341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3647849c5afe980618f8524555066ff7281a4922837e738bedbbfbb9535122e1`  
		Last Modified: Tue, 13 Sep 2022 14:31:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8762fb9639df84c726ced66c2dd5acf3bf12c70155e09c56c7481ac7ba1d34a4`  
		Last Modified: Tue, 13 Sep 2022 14:33:00 GMT  
		Size: 18.9 MB (18940067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd113daae99ef3edb53b60ba436e136109d384741177c04f92c6d681841af7e`  
		Last Modified: Tue, 13 Sep 2022 14:32:47 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2322960eb4a16dbc5d77cf70fc2d2dc36964c39649e20a7d59a2b57432cb64a`  
		Last Modified: Tue, 13 Sep 2022 14:32:48 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ce0ce0ab6bca245fea23dbb01dbf77d6cd82fcb4b67f599b1ab0cc1be7c358`  
		Last Modified: Tue, 13 Sep 2022 14:41:12 GMT  
		Size: 10.5 MB (10541953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b3d9c196f4500477a13c150949ec7313d05b8087e170e0cec5fcfe0c9097eb`  
		Last Modified: Tue, 13 Sep 2022 14:41:07 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c267c1f00c8135e4d2480399207548d63145d6b870d25d08dad87e9f676d752`  
		Last Modified: Tue, 13 Sep 2022 14:41:15 GMT  
		Size: 9.7 MB (9693343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4803a9d6cf2c7704cd3ce0c00bc4a19429ab072760f741ef73f7183b80938d2`  
		Last Modified: Tue, 13 Sep 2022 14:41:07 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0175899ee9ffc756686084aac590984805d341f8c1f75ec36940666930e5af`  
		Last Modified: Tue, 13 Sep 2022 14:41:07 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97592f02c5d02f8f54302dfc52ba9cf3356172481ed39def8462fa3efff27c59`  
		Last Modified: Tue, 13 Sep 2022 14:41:07 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ab598fad000c2b2cd17ac24733cb91cb2cfa32a24b83e694e55fcc2adab682`  
		Last Modified: Wed, 14 Sep 2022 01:08:49 GMT  
		Size: 1.7 MB (1668644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543660c3a7c52c8f2b836929fa35e7327abf2fd719312e88933f1ee895110a39`  
		Last Modified: Wed, 14 Sep 2022 01:08:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da0cd03acef87adf16820b85fbf69bac479f9522dd9ea7488f4626140476bed`  
		Last Modified: Wed, 14 Sep 2022 01:08:51 GMT  
		Size: 3.4 MB (3396560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache` - linux; ppc64le

```console
$ docker pull drupal@sha256:9538f5ad99c8c1b62e2c2f64f08784b5cfba7fcb2ff73a7e60dc84225bef674b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.6 MB (169603365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af786837d12e23f363fddb2a45965b3e79e6468eb903c98dbd30aee91c36ea99`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 02:07:56 GMT
ADD file:8b05dcf5f16a2ae9169b27aa848b812e07cd30414e51e4d53df9a5f01cd4c1a4 in / 
# Tue, 13 Sep 2022 02:07:58 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 08:57:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 08:57:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 08:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 08:58:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 08:58:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 09:03:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 09:03:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 09:03:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 09:03:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 09:03:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 09:03:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:03:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 09:03:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 09:54:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 13 Sep 2022 09:54:29 GMT
ENV PHP_VERSION=7.4.30
# Tue, 13 Sep 2022 09:54:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 13 Sep 2022 09:54:29 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 13 Sep 2022 09:54:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 09:54:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 09:57:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 09:57:37 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 09:57:39 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 09:57:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 09:57:39 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 09:57:39 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 09:57:40 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 09:57:40 GMT
EXPOSE 80
# Tue, 13 Sep 2022 09:57:40 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 17:56:53 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 17:56:54 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 18:04:13 GMT
ENV DRUPAL_VERSION=7.92
# Tue, 13 Sep 2022 18:04:13 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Tue, 13 Sep 2022 18:04:15 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:9716ed411387b5ba1ec8278e9fb108a44d8a09ffbbbfd1639f06c63f20364b45`  
		Last Modified: Tue, 13 Sep 2022 02:13:40 GMT  
		Size: 35.3 MB (35277392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91209fccba8355253d327410153436e6f68c9c4042604ce50f89c317278629f`  
		Last Modified: Tue, 13 Sep 2022 10:13:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c5ea8d2fe0355e70ac32fb3ed54088813398979340abf844b3a26512d23af3`  
		Last Modified: Tue, 13 Sep 2022 10:13:40 GMT  
		Size: 86.6 MB (86630630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a5879ca995ecd125c33859087ac27956f59f3083e972e286ebaa8cd70213b1`  
		Last Modified: Tue, 13 Sep 2022 10:13:15 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00be9890085732ccef9092ac3c66cf33f8b2713b3111df6ae39b33697f017d2`  
		Last Modified: Tue, 13 Sep 2022 10:14:24 GMT  
		Size: 20.5 MB (20464728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482854eea10defaf6bda6d1e7fa2c44d9112925552530ec32ed1c5c4402a6d15`  
		Last Modified: Tue, 13 Sep 2022 10:14:19 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecdde92afb2ac7e5f1b7964ee3952d0d8149d604722c408ecd36709e5bc1642a`  
		Last Modified: Tue, 13 Sep 2022 10:14:18 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1669bffad5f0cf5646030f3141298d7ed5098268841e8f0f4ce8bbf3607721a7`  
		Last Modified: Tue, 13 Sep 2022 10:23:18 GMT  
		Size: 10.8 MB (10758752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5c6a13fe05644fa9ea1ae1cbd270c97690edf36a4a01450b28cba4a731bbd`  
		Last Modified: Tue, 13 Sep 2022 10:23:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a648e63bb556cb13e4be30a71d03c50f9e0b851e20fc7bd2758ba6ffd52d94`  
		Last Modified: Tue, 13 Sep 2022 10:23:18 GMT  
		Size: 10.9 MB (10893004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0f34379441acd63133e822e616b238df98b1970688e4603af4171e1484fc09`  
		Last Modified: Tue, 13 Sep 2022 10:23:14 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60b1d08c817ead8e67c1397aacb724cab6b94e650fdaf5312d6352aea037250`  
		Last Modified: Tue, 13 Sep 2022 10:23:14 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcab3a0d7a90b00041858a5bfaeeb5a944cef2f10902eb05f8b1f551bebbe0cd`  
		Last Modified: Tue, 13 Sep 2022 10:23:14 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a9e343cdf489a3499505320fb4513ec7b50b3c4ed64dd6ca73502a39151eb4`  
		Last Modified: Tue, 13 Sep 2022 18:23:20 GMT  
		Size: 2.2 MB (2176105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c993606819e8ccb0819f0fa8cfbd78412fa5d22ebbaa261a40affcab9551af58`  
		Last Modified: Tue, 13 Sep 2022 18:23:19 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b9d32f9e40cddda1b604fbdd9acacc2c217eb8b124068b3917a3b6da61b828`  
		Last Modified: Tue, 13 Sep 2022 18:30:48 GMT  
		Size: 3.4 MB (3396849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-apache` - linux; s390x

```console
$ docker pull drupal@sha256:0a240bb06a9c84c69f2e7b721d0b0fe77ee351da649fdf46257e31a0396a8107
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.1 MB (146071103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f7b36c741329279a83e1a1e5f70294ee63a790da2be9e7ef2a8a9d49b674c27`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:37:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 13 Sep 2022 03:37:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 13 Sep 2022 03:37:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:37:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 13 Sep 2022 03:37:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 13 Sep 2022 03:40:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 13 Sep 2022 03:40:49 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 13 Sep 2022 03:40:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 13 Sep 2022 03:40:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 13 Sep 2022 03:40:59 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 13 Sep 2022 03:40:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 03:40:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 13 Sep 2022 03:40:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 13 Sep 2022 04:11:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 13 Sep 2022 04:11:31 GMT
ENV PHP_VERSION=7.4.30
# Tue, 13 Sep 2022 04:11:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 13 Sep 2022 04:11:31 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 13 Sep 2022 04:11:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 04:11:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:13:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 13 Sep 2022 04:13:04 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:13:04 GMT
RUN docker-php-ext-enable sodium
# Tue, 13 Sep 2022 04:13:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 13 Sep 2022 04:13:04 GMT
STOPSIGNAL SIGWINCH
# Tue, 13 Sep 2022 04:13:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 13 Sep 2022 04:13:05 GMT
WORKDIR /var/www/html
# Tue, 13 Sep 2022 04:13:05 GMT
EXPOSE 80
# Tue, 13 Sep 2022 04:13:05 GMT
CMD ["apache2-foreground"]
# Tue, 13 Sep 2022 12:55:09 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:55:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 13 Sep 2022 13:00:49 GMT
ENV DRUPAL_VERSION=7.92
# Tue, 13 Sep 2022 13:00:49 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Tue, 13 Sep 2022 13:00:50 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7b0f5d9f946c903b232120cd9ba651b9c49152b60e0cc030015c6d46b9ecad`  
		Last Modified: Tue, 13 Sep 2022 04:26:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384bdf7038d2518202b377df8a6d9ed8ea70e2e03017059118a215c6720afe19`  
		Last Modified: Tue, 13 Sep 2022 04:26:09 GMT  
		Size: 71.6 MB (71625709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00dfe3f880fd64eff9f2b5b67139c8b88ce9109de9802b7b3bb411ef2f5bb531`  
		Last Modified: Tue, 13 Sep 2022 04:26:00 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35aa7e122e3d514f58b34e887f925e575dcae5fd0d5ee1052dd5501269e2dda4`  
		Last Modified: Tue, 13 Sep 2022 04:26:34 GMT  
		Size: 19.1 MB (19070968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214c10017a0450a7c2e32da584d50a2f8725d7d868279c592d4e50fbca349669`  
		Last Modified: Tue, 13 Sep 2022 04:26:31 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695c86d2e601886bd430282ce8ee48996bf23e7642c07efa5b5590bb362a0592`  
		Last Modified: Tue, 13 Sep 2022 04:26:31 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d074a374bc6d098160eaf7b005fa34df2c399b0978b130e7d1b67afd8bb07dc5`  
		Last Modified: Tue, 13 Sep 2022 04:32:04 GMT  
		Size: 10.8 MB (10757890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d78f9cdb6a15c93c62fc897ee85424db221d79969e42a6e28a1336d824a2577`  
		Last Modified: Tue, 13 Sep 2022 04:32:02 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e694032f18671a6f60e7da768ca69b13096e0ba5f64fcad3faedffdf67a005`  
		Last Modified: Tue, 13 Sep 2022 04:32:04 GMT  
		Size: 9.7 MB (9687975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e2544ae3cda8f0f3861a9417d0661b7e6acf92df29c7f084f4061ae24e815d`  
		Last Modified: Tue, 13 Sep 2022 04:32:02 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941fca5fdddb517537a6b7b4c78f17bfbe87b9e816f9055480ab59b226f606d5`  
		Last Modified: Tue, 13 Sep 2022 04:32:02 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72554cec59efa02a02427987b7649987a374b23bca2516dad985a734acebd9c`  
		Last Modified: Tue, 13 Sep 2022 04:32:02 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb7d9ebd5396371f9b0708e72fdadc998c3176ec253c62cba8e2edf8c5ffeb5`  
		Last Modified: Tue, 13 Sep 2022 13:14:30 GMT  
		Size: 1.9 MB (1890736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f5b793a347749422d87ecc9f3bbbbd26c486332d54a9e1b0b2540b7fe830c`  
		Last Modified: Tue, 13 Sep 2022 13:14:30 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d193805fb3eb8c5dcc3ab605188eecd2abac2ad3ab6be87c6627d6e3981412`  
		Last Modified: Tue, 13 Sep 2022 13:18:55 GMT  
		Size: 3.4 MB (3396852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
