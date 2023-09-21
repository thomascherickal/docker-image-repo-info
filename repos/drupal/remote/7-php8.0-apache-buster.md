## `drupal:7-php8.0-apache-buster`

```console
$ docker pull drupal@sha256:69c7dce609ce11663ae014f60b850d56911b3fb52efe06eec8611d258da869d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:7-php8.0-apache-buster` - linux; amd64

```console
$ docker pull drupal@sha256:d8f993011d72bffa00252551e1242cda9d90edeedfb4e38653b948855a64b8a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150128978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2fb1e56e15da83aeeb2ebedfe6a74502b3cd9cd29867aec8ed5a71d6cef27fd`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 07 Sep 2023 00:21:35 GMT
ADD file:9c8b7c79fbbb19d308d151785d178e19bfa7b83257f38d03fa7f30cd41d58530 in / 
# Thu, 07 Sep 2023 00:21:35 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 07:04:41 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 07 Sep 2023 07:04:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 07 Sep 2023 07:05:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 07:05:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 07 Sep 2023 07:05:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 07 Sep 2023 07:08:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 07 Sep 2023 07:08:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 07 Sep 2023 07:08:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 07 Sep 2023 07:08:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 07 Sep 2023 07:08:30 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 07 Sep 2023 07:08:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 07:08:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 07:08:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 07 Sep 2023 07:08:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 07 Sep 2023 07:08:30 GMT
ENV PHP_VERSION=8.0.30
# Thu, 07 Sep 2023 07:08:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 07 Sep 2023 07:08:30 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 07 Sep 2023 07:08:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Sep 2023 07:08:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Sep 2023 07:11:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Sep 2023 07:11:38 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 07 Sep 2023 07:11:39 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Sep 2023 07:11:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Sep 2023 07:11:39 GMT
STOPSIGNAL SIGWINCH
# Thu, 07 Sep 2023 07:11:39 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 07 Sep 2023 07:11:39 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 07:11:39 GMT
EXPOSE 80
# Thu, 07 Sep 2023 07:11:40 GMT
CMD ["apache2-foreground"]
# Thu, 07 Sep 2023 23:46:38 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 23:46:39 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 07 Sep 2023 23:49:21 GMT
ENV DRUPAL_VERSION=7.98
# Thu, 07 Sep 2023 23:49:21 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Thu, 07 Sep 2023 23:49:22 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:91f01557fe0da558070d4f24631c94e91a80877a24621b52b8b13009b62d8d96`  
		Last Modified: Thu, 07 Sep 2023 00:26:44 GMT  
		Size: 27.2 MB (27187385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae13a49b7b1fa8948b97a72ec6e48151a5a7703df58f481e83bbb72ecd4526e1`  
		Last Modified: Thu, 07 Sep 2023 07:30:23 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1e9c09cf55454a744cb48ef46c9b0dca23fa800aab4d556edcbbe86dcfc582`  
		Last Modified: Thu, 07 Sep 2023 07:30:34 GMT  
		Size: 76.7 MB (76691058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89b4b1d57b71aee6b68bc9e2f31ca05d2c1903c9d0b84755265790dd5ff6681`  
		Last Modified: Thu, 07 Sep 2023 07:30:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8737f50d59bb08e591f1e6d49d41a7ea39c52599eb62c8e34073567acca8763d`  
		Last Modified: Thu, 07 Sep 2023 07:30:52 GMT  
		Size: 18.7 MB (18689994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ce4efb53360c4321be43bc627fb24e7fa670ad6c7cf7a2f23a8c4ec7d3f014`  
		Last Modified: Thu, 07 Sep 2023 07:30:50 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d94cf85b34b6196395367b8152949e9189571cf4a809b99a4f36e76719d53d9`  
		Last Modified: Thu, 07 Sep 2023 07:30:50 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bbbc0dc01e352587075894ecfde6b806ced33a6c6fa30429470b6d3a0a6387`  
		Last Modified: Thu, 07 Sep 2023 07:30:51 GMT  
		Size: 11.2 MB (11160913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3993f7e7c2208be37d92466844c15b3bc26c981e212ce1bc43e5e143192ce5`  
		Last Modified: Thu, 07 Sep 2023 07:30:48 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd44441ecda652546cd93b8875e2eb2027130cfe0102d38ac8caea78c5d36986`  
		Last Modified: Thu, 07 Sep 2023 07:30:49 GMT  
		Size: 10.7 MB (10734927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8994aec50cf75dc411fd7d21306f57e6e5bbaa45a8d53267b40bae3996a0831d`  
		Last Modified: Thu, 07 Sep 2023 07:30:48 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab5756a1796383f8bd9292da68f58064963197bfdbcc880fd68afebd538c297`  
		Last Modified: Thu, 07 Sep 2023 07:30:48 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d53cbf18ee40975076e74ef8563eec5d535996be08196d6efd0a0bbebc79c1`  
		Last Modified: Thu, 07 Sep 2023 07:30:48 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89828db1afd79036c336f0025afe88ee1e83b4bc3859efd237d19236948469d8`  
		Last Modified: Fri, 08 Sep 2023 00:06:15 GMT  
		Size: 2.2 MB (2248037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95bb15620431025872fd4c9c3d508bb74aecdad64eacc39658426457e36ff22`  
		Last Modified: Fri, 08 Sep 2023 00:06:15 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8663d7c4db8dfc68afbe0ec3da1da723661a7ac70505795397eb8f30746c0de`  
		Last Modified: Fri, 08 Sep 2023 00:09:14 GMT  
		Size: 3.4 MB (3410776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.0-apache-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:a38848a746cfa309dd40d2710b3d31e8059ef3e3262735f793d0161f6de889d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125290861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be2b1d29e44495b10ed1ee992bccdbf8429ad60bc915079cef0b93d5fc9a61ab`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 07 Sep 2023 00:58:32 GMT
ADD file:fa060a900723a2fce017a38b08be3eb2c27d4768d40c61cd1f6292a7f28a8bdc in / 
# Thu, 07 Sep 2023 00:58:33 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 18:38:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 07 Sep 2023 18:38:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 07 Sep 2023 18:39:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 18:39:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 07 Sep 2023 18:39:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 07 Sep 2023 18:42:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 07 Sep 2023 18:42:15 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 07 Sep 2023 18:42:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 07 Sep 2023 18:42:26 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 07 Sep 2023 18:42:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 07 Sep 2023 18:42:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 18:42:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 07 Sep 2023 18:42:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 07 Sep 2023 18:42:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 07 Sep 2023 18:42:27 GMT
ENV PHP_VERSION=8.0.30
# Thu, 07 Sep 2023 18:42:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 07 Sep 2023 18:42:28 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 07 Sep 2023 18:42:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Sep 2023 18:42:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Sep 2023 18:45:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Sep 2023 18:45:52 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 07 Sep 2023 18:45:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Sep 2023 18:45:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Sep 2023 18:45:52 GMT
STOPSIGNAL SIGWINCH
# Thu, 07 Sep 2023 18:45:52 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 07 Sep 2023 18:45:53 GMT
WORKDIR /var/www/html
# Thu, 07 Sep 2023 18:45:53 GMT
EXPOSE 80
# Thu, 07 Sep 2023 18:45:53 GMT
CMD ["apache2-foreground"]
# Fri, 08 Sep 2023 04:28:33 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Sep 2023 04:28:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 08 Sep 2023 04:31:21 GMT
ENV DRUPAL_VERSION=7.98
# Fri, 08 Sep 2023 04:31:21 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Fri, 08 Sep 2023 04:31:22 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:7e54f06c680feaf82a31a34e7453d765f332f671cfecacb622c3046561dcc572`  
		Last Modified: Thu, 07 Sep 2023 01:03:53 GMT  
		Size: 22.8 MB (22795752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed417f72a0d8c0020491eace2aef68fe5e017ce353baf87a7c0a0d523ff8384`  
		Last Modified: Thu, 07 Sep 2023 19:06:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31950e5c5fc44b2e387de59b3aac9a1a18544a5e070a1be579e612ed4e1741e6`  
		Last Modified: Thu, 07 Sep 2023 19:07:02 GMT  
		Size: 59.5 MB (59541512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df50a7162df832b2fadaa8a33cd31a2b5e2b34f8f6f9a342057e0bfe6652005`  
		Last Modified: Thu, 07 Sep 2023 19:06:45 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa6511487ceadf0761af50c6abb437923f064ece32b367f94f998265cdec496`  
		Last Modified: Thu, 07 Sep 2023 19:07:25 GMT  
		Size: 17.5 MB (17482085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1333ce19db02170b191755a3b246a3a77f1e94bae947817af0e9bd1268b278b5`  
		Last Modified: Thu, 07 Sep 2023 19:07:20 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc94e0889e8e799c61802ccf5e1934c6ba973f5cce1b1739a7af14d0d2b9165`  
		Last Modified: Thu, 07 Sep 2023 19:07:20 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86c7b5c3e62e9cbcf5f3b0746c996038f35c3487e07cc0db576e410d4c9284b`  
		Last Modified: Thu, 07 Sep 2023 19:07:22 GMT  
		Size: 11.2 MB (11158980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27597cdcfbc84fb6a8319b8fc1a80659d18eddc310c1df9b3bb4e9f0a280a0e1`  
		Last Modified: Thu, 07 Sep 2023 19:07:18 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644306849b14bf7e78325c97d002647bf2bb21a741468ff56cd0d69cdb50ce1c`  
		Last Modified: Thu, 07 Sep 2023 19:07:21 GMT  
		Size: 9.3 MB (9262457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e362bc575b85044dc9f7b01464be8955c4a87fb1a28fad79325a371061d368`  
		Last Modified: Thu, 07 Sep 2023 19:07:18 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcad625278377ff589060174bc64887c90ac166992e855c1094ceda290a2580a`  
		Last Modified: Thu, 07 Sep 2023 19:07:18 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f58890b640277b51789c693c143fb46bb1032d149bcb46018cbdd224988d04`  
		Last Modified: Thu, 07 Sep 2023 19:07:18 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143b250414bbaa420672e60fc922439ddc3050212ae7259a5c23989c1e28d419`  
		Last Modified: Fri, 08 Sep 2023 04:53:10 GMT  
		Size: 1.6 MB (1633410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17475b1343c0a3d7e1e331753a8d3fbc6428ed851ca60dccf8a55bf27773b6d3`  
		Last Modified: Fri, 08 Sep 2023 04:53:09 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276329315fd114335812c89a6eccdeea1b5b117aef042d2579ea6a63476ff6c9`  
		Last Modified: Fri, 08 Sep 2023 04:56:23 GMT  
		Size: 3.4 MB (3410781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.0-apache-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:e59d2f28b2b26465db8e262cb71b20366054fd917eecccf13550e578b18a8983
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.6 MB (141606343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7ee397011c38931a5d6c793d59e1ab85a2ada2cc88b02dd5ec7c971ee44621b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:42 GMT
ADD file:22373577ebc4a88322b8e7e5a349667740deade289df65952593aa5fa355e161 in / 
# Wed, 20 Sep 2023 02:44:42 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 05:47:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 05:47:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 05:47:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 05:47:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 05:47:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 05:50:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 05:50:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 05:50:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 05:50:14 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 05:50:14 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 05:50:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:50:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 05:50:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 05:50:14 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 05:50:15 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 05:50:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 05:50:15 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 05:50:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 05:50:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:52:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 05:52:21 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:52:21 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 05:52:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 05:52:21 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 05:52:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:52:21 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 05:52:22 GMT
EXPOSE 80
# Wed, 20 Sep 2023 05:52:22 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 18:43:41 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 18:43:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 20 Sep 2023 18:45:52 GMT
ENV DRUPAL_VERSION=7.98
# Wed, 20 Sep 2023 18:45:52 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Wed, 20 Sep 2023 18:45:53 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:a5329dc26fe29288aabb62184c71ef06987bd81c95d7c43a48e38a0dfaa54ff8`  
		Last Modified: Wed, 20 Sep 2023 02:48:50 GMT  
		Size: 26.0 MB (25967816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b246114d1c77fb2a14434449a34b0e8761eb8579db67ea844bcd3b8b2080f7b5`  
		Last Modified: Wed, 20 Sep 2023 06:16:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184f42380bd1e57d38a9a1bc857bece1bf51fe9157002f8e40e30f9edfd97dff`  
		Last Modified: Wed, 20 Sep 2023 06:16:42 GMT  
		Size: 70.4 MB (70362229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1529d01406312ce383fe74f2bc5676b908600571adc5a10ebc8c6f837ee38a`  
		Last Modified: Wed, 20 Sep 2023 06:16:35 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7f0c8a6b8b9a156c5e4e9d264025d931eb08280a9b24ee319b10a05c45b4f7`  
		Last Modified: Wed, 20 Sep 2023 06:16:59 GMT  
		Size: 18.6 MB (18587230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ee3333af32e62361fda70f2def3d4a6f18dc68a456a61b266e4c4037d3a3e5`  
		Last Modified: Wed, 20 Sep 2023 06:16:57 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15f2871fa4bccf4959dd71f8e835b6cbdd5ccea17bed21c1077ab153b60200a`  
		Last Modified: Wed, 20 Sep 2023 06:16:57 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805c6b2e69ad58b009a64ae933f0e824e42763890bf5f79376937c03494836c0`  
		Last Modified: Wed, 20 Sep 2023 06:16:58 GMT  
		Size: 11.2 MB (11159715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd9f79aa5006ab615a3497cecc1d010d8690b5acccb021b4096318369b97a80`  
		Last Modified: Wed, 20 Sep 2023 06:16:55 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33da982da9256759f78b23b06163fc46b73cbc7396712b5aa721dc2e6ecc11cc`  
		Last Modified: Wed, 20 Sep 2023 06:16:57 GMT  
		Size: 10.2 MB (10211993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd796c93b4f6b0a182ca4cfce2f2a52bc53ce47a876ef4aa2092a24a23868beb`  
		Last Modified: Wed, 20 Sep 2023 06:16:55 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b833ad835bb588e67c8abeacabd31087803621ef0bcf3e2892389beee7a9ae`  
		Last Modified: Wed, 20 Sep 2023 06:16:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a229a247c2b5ea09e897b7ebfceaca706265f5d74e489f8cc3c2af86643618`  
		Last Modified: Wed, 20 Sep 2023 06:16:55 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1952750e1218bccdf0bb1f8025b6bed9cff7aeac7f807e01cb43dcd6de0975c`  
		Last Modified: Wed, 20 Sep 2023 19:00:52 GMT  
		Size: 1.9 MB (1900704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5a4ac2c8d942998223b419da9f47839572bd2b666e818b5bee6c79fec1b2cd`  
		Last Modified: Wed, 20 Sep 2023 19:00:51 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5389bfedfa6b57360996900eb7c721fb9fdb7bf66f147d5b422575153f54c2`  
		Last Modified: Wed, 20 Sep 2023 19:03:50 GMT  
		Size: 3.4 MB (3410781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php8.0-apache-buster` - linux; 386

```console
$ docker pull drupal@sha256:87052d9b475dd57f60a982c936bdc1ad23a9a8cbbb47c9ff9b351fff7549f986
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (156037017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7673fb5443c3b69b017c8b2f4bfa6f3d9d0d18749db3b533a1df1800be7ec30`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:41 GMT
ADD file:fb989660816f4cd43e34acc142a953475b8c7002d0827f2bf3f52df3f7792cbf in / 
# Wed, 20 Sep 2023 00:42:41 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 06:30:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 06:30:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 06:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 06:30:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 06:30:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 06:36:29 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 06:36:29 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 06:36:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 06:36:45 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 06:36:45 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 06:36:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 06:36:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 06:36:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 06:36:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 06:36:46 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 06:36:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 06:36:46 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 06:37:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 06:37:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:41:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 06:41:58 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:41:58 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 06:41:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 06:41:59 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 06:41:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:41:59 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:41:59 GMT
EXPOSE 80
# Wed, 20 Sep 2023 06:41:59 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 03:09:37 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Sep 2023 03:09:38 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Sep 2023 03:12:24 GMT
ENV DRUPAL_VERSION=7.98
# Thu, 21 Sep 2023 03:12:25 GMT
ENV DRUPAL_MD5=4139f0feecb44a53645242194809b73a
# Thu, 21 Sep 2023 03:12:26 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:d2583a509dfdf283554f9e60a045ae6823d40ee59a6bb9892e15839171b30970`  
		Last Modified: Wed, 20 Sep 2023 00:48:22 GMT  
		Size: 27.8 MB (27846922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e957484b5cac85a6080e6d3c04e08504754aea75df923ea9e2443b28ce29f97`  
		Last Modified: Wed, 20 Sep 2023 07:15:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5282a2ff79ffe102d2983dbdc3aae753caccd756b0afa0b7e4f1920f43a41a9d`  
		Last Modified: Wed, 20 Sep 2023 07:16:00 GMT  
		Size: 81.2 MB (81235090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c03d8322b1297d6a7523f660b5817670c569707c2395a345be66ebe3b857b68`  
		Last Modified: Wed, 20 Sep 2023 07:15:41 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4946d99a5c60206eeef0155bc2b74e8dadadf83e89f6362e672c9c5e4f9f81`  
		Last Modified: Wed, 20 Sep 2023 07:16:21 GMT  
		Size: 19.1 MB (19117708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7a967757d50a09c4677705332f26859b5f99e4d609795ef11eb1117c746678`  
		Last Modified: Wed, 20 Sep 2023 07:16:17 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a656d3dd4526c0d778b74900a8f31ebe9cbf205e9bf13bd05754f798970dd176`  
		Last Modified: Wed, 20 Sep 2023 07:16:17 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4059e292440d8924678f71ac98d22579789e3e671d1d394668062c2d8e58c78e`  
		Last Modified: Wed, 20 Sep 2023 07:16:18 GMT  
		Size: 11.2 MB (11160238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89987bc673a48a6708d9652c50e336b7ab2d2505745b0b2fe3ff0a77eba53035`  
		Last Modified: Wed, 20 Sep 2023 07:16:15 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fc91d138317e9a55ff0429c3384d88d89174f159276b26b90d472ef2da6ee3`  
		Last Modified: Wed, 20 Sep 2023 07:16:19 GMT  
		Size: 10.9 MB (10943541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36073921823e443ac55fc43185bc9f06c731b3e58f6842fe0897b5037c0f1179`  
		Last Modified: Wed, 20 Sep 2023 07:16:15 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19585e01e416da59e61eaf6c4d6aab3e0a2aac75031fcb8c8632e544c5511d6d`  
		Last Modified: Wed, 20 Sep 2023 07:16:15 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5aa4acdddbb87be8064a12ddd28cb5a43e8732311d18d1c182138b9be812704`  
		Last Modified: Wed, 20 Sep 2023 07:16:15 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6594035876c1fb33245b20e3bdac767ffbd18c2064bb3aa9f2a2988b8bd63f6`  
		Last Modified: Thu, 21 Sep 2023 03:29:47 GMT  
		Size: 2.3 MB (2316852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0dcf8808bcb31a7d185ec4f004507134544a7e0eba349d943a32ee30331b5fe`  
		Last Modified: Thu, 21 Sep 2023 03:29:46 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbf8f62b9121cc86f99a32b58fbdcb089828ceab51f7b09815c3d6cd3b1ae4e`  
		Last Modified: Thu, 21 Sep 2023 03:32:55 GMT  
		Size: 3.4 MB (3410784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
