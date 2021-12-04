## `joomla:4-php7.4-apache`

```console
$ docker pull joomla@sha256:b0f7b0572f3988231a4c6a1a7015cac405f6e655d436d32cb0c9b8b494fe415f
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

### `joomla:4-php7.4-apache` - linux; amd64

```console
$ docker pull joomla@sha256:cf79b8b3a5154bf2c9c3a97625296cc36de5a5e088023e0552af79eca1fb629d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.5 MB (191529375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83587cbd648af81abe645352fc15e8afa6850b5ff50cdf451262dfb8770db1e0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:20 GMT
ADD file:ece5ff85ca549f0b1e9139d29dcb43a52af672d0591c423e28180f6d8d700ad7 in / 
# Thu, 02 Dec 2021 02:48:21 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:03:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 12:03:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 12:04:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:04:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 12:04:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 12:13:22 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 12:13:22 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 12:13:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 12:13:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 12:13:37 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 12:13:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:13:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:13:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 14:22:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 02 Dec 2021 14:22:32 GMT
ENV PHP_VERSION=7.4.26
# Thu, 02 Dec 2021 14:22:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 02 Dec 2021 14:22:32 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 02 Dec 2021 14:22:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 02 Dec 2021 14:22:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:25:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 02 Dec 2021 14:25:51 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:25:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 02 Dec 2021 14:25:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Dec 2021 14:25:52 GMT
STOPSIGNAL SIGWINCH
# Thu, 02 Dec 2021 14:25:52 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 02 Dec 2021 14:25:53 GMT
WORKDIR /var/www/html
# Thu, 02 Dec 2021 14:25:53 GMT
EXPOSE 80
# Thu, 02 Dec 2021 14:25:53 GMT
CMD ["apache2-foreground"]
# Fri, 03 Dec 2021 19:32:36 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 03 Dec 2021 19:32:37 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 03 Dec 2021 19:32:37 GMT
RUN a2enmod rewrite
# Fri, 03 Dec 2021 19:34:18 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 19:34:19 GMT
VOLUME [/var/www/html]
# Fri, 03 Dec 2021 19:34:19 GMT
ENV JOOMLA_VERSION=4.0.4
# Fri, 03 Dec 2021 19:34:19 GMT
ENV JOOMLA_SHA512=56dc516fd4596c1f728cf3503d7427dfc755d4b23ad5c170e2ee11d2a1d9e38484b3fa5cb337f8ce9ad8b5108386644d915afda3d3eae0d418dae9bd1d774eb3
# Fri, 03 Dec 2021 19:34:26 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 03 Dec 2021 19:34:27 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Fri, 03 Dec 2021 19:34:27 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 03 Dec 2021 19:34:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 19:34:28 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e5ae68f740265288a4888db98d2999a638fdcb6d725f427678814538d253aa4d`  
		Last Modified: Thu, 02 Dec 2021 02:53:46 GMT  
		Size: 31.4 MB (31370221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c3c1c4d556eaf1a4d1ec1591b053c3a723104b3c998a9d44a66132b7ee3af8`  
		Last Modified: Thu, 02 Dec 2021 15:29:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c23b6beb07ab1b78af3929ff31a2ec34ece94ac611be50a32d54406e925b64f`  
		Last Modified: Thu, 02 Dec 2021 15:29:20 GMT  
		Size: 91.6 MB (91605023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9874148cff9ac18f61ee23d041488694c002bf082e32d004232055b99e2f705f`  
		Last Modified: Thu, 02 Dec 2021 15:29:03 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52defac986292394d78237bb5d79c9b45c18bcd31ba38ccf9a1c9fab6ee955b7`  
		Last Modified: Thu, 02 Dec 2021 15:30:15 GMT  
		Size: 19.2 MB (19235843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585eed6f53992820a6d18df110b45f7a75a2d8b94fc827978b09e444ee3985dd`  
		Last Modified: Thu, 02 Dec 2021 15:30:12 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa83ee0498fff0d0660501ab49e185d11ce4952ccd2f64a982e2909f21163bcd`  
		Last Modified: Thu, 02 Dec 2021 15:30:12 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356035aff0a02cd8f304e41fdd1d33bd0120a313335fbae58cdf22e1e24d5fb9`  
		Last Modified: Thu, 02 Dec 2021 15:37:33 GMT  
		Size: 10.8 MB (10760033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fcc4ec7a3593a968951b32a193d0074872c1388645ebe06e9756fbbeaf1554`  
		Last Modified: Thu, 02 Dec 2021 15:37:29 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0903fae56b0ec8b52e54ec42de00941386ddd4a9d790a7639c7f897908354dc`  
		Last Modified: Thu, 02 Dec 2021 15:37:33 GMT  
		Size: 13.9 MB (13907981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d2ad3b821d087b041151f36f3efce462c64091ae200f1d05103517a1bb1ff6`  
		Last Modified: Thu, 02 Dec 2021 15:37:29 GMT  
		Size: 2.3 KB (2311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bf4a72a8eb98eb63eb501424fe60463c452d1e76c43a84f047fe128376fc8f`  
		Last Modified: Thu, 02 Dec 2021 15:37:30 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5066fa6c34bb80697416ef53fab3b3d983f159e1f62bb5994899c781d1b8ffa0`  
		Last Modified: Thu, 02 Dec 2021 15:37:29 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666e697dc875ce32941c7c582be3eb1b9bbaf9470f45f1021bbc4c818db293c3`  
		Last Modified: Fri, 03 Dec 2021 19:48:32 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee8c6d994f50d2d5c59cfcd192a4924b7f6a89d71b4e6a1a561e06b89835a3c`  
		Last Modified: Fri, 03 Dec 2021 19:48:33 GMT  
		Size: 3.1 MB (3076214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dbd290cc596178167ca9bd9da01bc16326854d92dae10839a3b0b1490bb9ea`  
		Last Modified: Fri, 03 Dec 2021 19:48:36 GMT  
		Size: 21.6 MB (21566510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a67ef1cc0ad22fdaebb6d08174a0131fed04a621f55cec93d9f406fafe91a63`  
		Last Modified: Fri, 03 Dec 2021 19:48:32 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db897e8990f22252c7b83cc1ef422fe747f645a00334c22014e9c472af1c5a4`  
		Last Modified: Fri, 03 Dec 2021 19:48:32 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-apache` - linux; arm variant v5

```console
$ docker pull joomla@sha256:aefd94f5df2a9bca01ecdad152adab5036c79b92978bf741261f6f86e5e96c81
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169313618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f1d790a3f8c0d154e7ffefeb3a09beea6765d02e6a63a14d117590e6c10a91d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 02:50:37 GMT
ADD file:7debbdb237139cb08189976f79cfa64cfd71f5cc98dfb2f560b558acb5f7cec9 in / 
# Thu, 02 Dec 2021 02:50:38 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 01:13:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 01:13:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 01:14:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 01:14:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 01:14:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 01:20:28 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 03 Dec 2021 01:20:28 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 03 Dec 2021 01:20:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 03 Dec 2021 01:20:55 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 03 Dec 2021 01:20:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 03 Dec 2021 01:20:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:20:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:20:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 02:52:27 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 03 Dec 2021 02:52:27 GMT
ENV PHP_VERSION=7.4.26
# Fri, 03 Dec 2021 02:52:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Fri, 03 Dec 2021 02:52:28 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Fri, 03 Dec 2021 02:52:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Dec 2021 02:52:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Dec 2021 02:57:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Dec 2021 02:57:08 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 03 Dec 2021 02:57:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Dec 2021 02:57:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Dec 2021 02:57:10 GMT
STOPSIGNAL SIGWINCH
# Fri, 03 Dec 2021 02:57:11 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 03 Dec 2021 02:57:11 GMT
WORKDIR /var/www/html
# Fri, 03 Dec 2021 02:57:12 GMT
EXPOSE 80
# Fri, 03 Dec 2021 02:57:12 GMT
CMD ["apache2-foreground"]
# Fri, 03 Dec 2021 13:09:40 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 03 Dec 2021 13:09:41 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 03 Dec 2021 13:09:42 GMT
RUN a2enmod rewrite
# Fri, 03 Dec 2021 13:14:45 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 13:14:46 GMT
VOLUME [/var/www/html]
# Fri, 03 Dec 2021 13:14:46 GMT
ENV JOOMLA_VERSION=4.0.4
# Fri, 03 Dec 2021 13:14:47 GMT
ENV JOOMLA_SHA512=56dc516fd4596c1f728cf3503d7427dfc755d4b23ad5c170e2ee11d2a1d9e38484b3fa5cb337f8ce9ad8b5108386644d915afda3d3eae0d418dae9bd1d774eb3
# Fri, 03 Dec 2021 13:15:06 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 03 Dec 2021 13:15:08 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Fri, 03 Dec 2021 13:15:09 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 03 Dec 2021 13:15:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 13:15:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c5e429166894878430c39748965935f89ffa957667340c3c8bd872418dbce663`  
		Last Modified: Thu, 02 Dec 2021 03:09:28 GMT  
		Size: 28.9 MB (28910824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b027b55d12ad9ac869559247a51c3128131e902296b69d94ad0923affd65b49`  
		Last Modified: Fri, 03 Dec 2021 04:21:52 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f66ff2b781e02c0d613433e3c079cab11ef176f78cc3ef16fd441f40132e9f5`  
		Last Modified: Fri, 03 Dec 2021 04:22:42 GMT  
		Size: 73.7 MB (73684131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67de67500ee532057975d51ed0340f7d279a7a7cf82659d1b3965733f8b47937`  
		Last Modified: Fri, 03 Dec 2021 04:21:52 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed693c24ace943128a45d90db76c1b69f72c7781151918f8902c1f1e1ded526e`  
		Last Modified: Fri, 03 Dec 2021 04:24:07 GMT  
		Size: 18.5 MB (18525660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1893923c825009b10ff626f0f6bac8da8d7a76d7e7cc311a88748801abccbd23`  
		Last Modified: Fri, 03 Dec 2021 04:23:55 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5154e3266a52eebe5ae82ec9de7a72811614a96fe6164b550738ff98262a95d`  
		Last Modified: Fri, 03 Dec 2021 04:23:55 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b10b3bc2a1ce1d11eb6b623dde2eb778821e0b1b6bedb8e39a9b49b74a0388b`  
		Last Modified: Fri, 03 Dec 2021 04:35:51 GMT  
		Size: 10.8 MB (10758661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bc72b2f8556cecac99d7709d256e8e3774290134e9fa1a9d17fe938418df6f`  
		Last Modified: Fri, 03 Dec 2021 04:35:47 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02fc816429f7cd7e76d5100b8ceb792bda9146240d3be918df3be9bc582ced0c`  
		Last Modified: Fri, 03 Dec 2021 04:35:56 GMT  
		Size: 13.0 MB (12982319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb4bafb71b9a12617c05a51d0eda0769b9ffe37fd6af571471c5840b60817e7`  
		Last Modified: Fri, 03 Dec 2021 04:35:47 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60a4bee872ccabd3795d8fce47929684fb89d073c9568daaaa75b57853b17af`  
		Last Modified: Fri, 03 Dec 2021 04:35:47 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbf523e4a9b0ea205bd5ff21820dbbbf53bb3b2e070824250efaea6a33b38d5`  
		Last Modified: Fri, 03 Dec 2021 04:35:47 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622a6bdaac7b600e6af5bac55caa630340ca77dd34ff65fe0c7afb00300161b2`  
		Last Modified: Fri, 03 Dec 2021 13:56:22 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7298cbb4f3d9c3ae0e397261661e620f7d187a2a0e5a6c0ecf86816ee3813876`  
		Last Modified: Fri, 03 Dec 2021 13:56:24 GMT  
		Size: 2.9 MB (2878249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d106e685e72c093552c1821972be15adf7434e5783baa1cac47987231afe3c5`  
		Last Modified: Fri, 03 Dec 2021 13:56:41 GMT  
		Size: 21.6 MB (21566197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed99f1e47953342d9070f7667d57c66af801a0b1f0e7e8315c99d486990ef08e`  
		Last Modified: Fri, 03 Dec 2021 13:56:22 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610da35d5a4c30745a82a8ed40065ed93ac3efb0e08ef2b4580bc545cc4c5801`  
		Last Modified: Fri, 03 Dec 2021 13:56:22 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-apache` - linux; arm variant v7

```console
$ docker pull joomla@sha256:fafe03e290d4ac327e41cc7cce6a63ce4297b52dff5b45ff32f2dd74de4b957a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.3 MB (161255345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f538a37548aa621e6e499a2c33a469f2e0224f177f54e9ef894245fa9c76ee8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 09:05:17 GMT
ADD file:97ce5af9ff4fb4002733d5c402ddc01a13e765d31b85bb6525a7fa797b698e10 in / 
# Thu, 02 Dec 2021 09:05:17 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 23:36:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 23:36:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 23:37:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 23:37:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 23:37:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 23:42:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 23:42:45 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 23:43:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 23:43:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 23:43:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 23:43:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 23:43:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 23:43:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 01:07:43 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 03 Dec 2021 01:07:44 GMT
ENV PHP_VERSION=7.4.26
# Fri, 03 Dec 2021 01:07:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Fri, 03 Dec 2021 01:07:45 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Fri, 03 Dec 2021 01:08:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Dec 2021 01:08:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Dec 2021 01:11:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Dec 2021 01:12:00 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 03 Dec 2021 01:12:02 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Dec 2021 01:12:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Dec 2021 01:12:03 GMT
STOPSIGNAL SIGWINCH
# Fri, 03 Dec 2021 01:12:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 03 Dec 2021 01:12:04 GMT
WORKDIR /var/www/html
# Fri, 03 Dec 2021 01:12:04 GMT
EXPOSE 80
# Fri, 03 Dec 2021 01:12:05 GMT
CMD ["apache2-foreground"]
# Sat, 04 Dec 2021 08:09:23 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 04 Dec 2021 08:09:23 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 04 Dec 2021 08:09:25 GMT
RUN a2enmod rewrite
# Sat, 04 Dec 2021 08:14:10 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Dec 2021 08:14:10 GMT
VOLUME [/var/www/html]
# Sat, 04 Dec 2021 08:14:11 GMT
ENV JOOMLA_VERSION=4.0.4
# Sat, 04 Dec 2021 08:14:11 GMT
ENV JOOMLA_SHA512=56dc516fd4596c1f728cf3503d7427dfc755d4b23ad5c170e2ee11d2a1d9e38484b3fa5cb337f8ce9ad8b5108386644d915afda3d3eae0d418dae9bd1d774eb3
# Sat, 04 Dec 2021 08:14:30 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 04 Dec 2021 08:14:31 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Sat, 04 Dec 2021 08:14:32 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 04 Dec 2021 08:14:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Dec 2021 08:14:33 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ba82a1312e1efdcd1cc6eb31cd40358dcec180da31779dac399cba31bf3dc206`  
		Last Modified: Thu, 02 Dec 2021 09:21:03 GMT  
		Size: 26.6 MB (26573192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50ffdc47d6f068811ac71535715f43a36fe261bbb0c3e31f43186a2282c558b`  
		Last Modified: Fri, 03 Dec 2021 02:41:55 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8bef2d8d286eef83c2c19371d6f497a886c348995670857a897340992fbf33c`  
		Last Modified: Fri, 03 Dec 2021 02:42:37 GMT  
		Size: 69.3 MB (69315176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5d96c53a2bfbf975478318788fcea14a43e10e632584b962131667404f99ec`  
		Last Modified: Fri, 03 Dec 2021 02:41:55 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb01bfbc6c017e5e7dd887798fef991c95d712e811cd1c0b064e0c0b17dad74`  
		Last Modified: Fri, 03 Dec 2021 02:44:03 GMT  
		Size: 18.0 MB (17987524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec61b17b81613dca9ca8a067b75997e68017b241b4f2975e426b07993204659f`  
		Last Modified: Fri, 03 Dec 2021 02:43:51 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f239832ff9fd16e8718be405a5b8654e1e9849f4a5031089742a95c1d5b24`  
		Last Modified: Fri, 03 Dec 2021 02:43:51 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:858a7291927974e98887b1291d8c676121ae38ce62e74bc1fba6b953f9fa5862`  
		Last Modified: Fri, 03 Dec 2021 02:56:47 GMT  
		Size: 10.8 MB (10758695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef20edf79dd4efe66c171dab4765f5ac7df51b5f08e8ad4a1fe16f6ceea6c6cc`  
		Last Modified: Fri, 03 Dec 2021 02:56:42 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2f9c677321c08e1d078a79d20ea55db1ff4e6715543a87a9f4f57d7a2bc3f6`  
		Last Modified: Fri, 03 Dec 2021 02:56:51 GMT  
		Size: 12.3 MB (12278709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0db6a34516166162df2a28dc9052a5d87760a584d35e70a9d8252bbafbf9b0`  
		Last Modified: Fri, 03 Dec 2021 02:56:42 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e77a80713adcb0e7f4b921d0e9fbdc15a04678bfd9ba7eee4b5c212b9eb996`  
		Last Modified: Fri, 03 Dec 2021 02:56:42 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37404b00d335493f61374f272a7216702cf8388f9f82f8a047b4ab50f127587`  
		Last Modified: Fri, 03 Dec 2021 02:56:42 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ace04de9729299b9867b2d7eac0f10ebf62d08391a92de006f462a00cb097f5`  
		Last Modified: Sat, 04 Dec 2021 08:56:14 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a1b4d8cf0963098b4d059948764ef1623240bbd1851b9c7aed2632da8813c7`  
		Last Modified: Sat, 04 Dec 2021 08:56:16 GMT  
		Size: 2.8 MB (2767978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963a1cc19c6eec6ddc48f267cf0191d9f14db57acc15bc321d9776dd100fa74e`  
		Last Modified: Sat, 04 Dec 2021 08:56:33 GMT  
		Size: 21.6 MB (21566498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d488db00fc8088b9a655ec480fb18040eafe577f3c92daa96e076f97c13a0cfb`  
		Last Modified: Sat, 04 Dec 2021 08:56:14 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd5a530364fe8dea4690c2bbc0467e878a30ae6083a4a2de57e4172b112442e`  
		Last Modified: Sat, 04 Dec 2021 08:56:14 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-apache` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:8ae15977da2b583872f32de7e39722fbe6c1e5ce025a4346de680c5dbff9ec08
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.3 MB (184289534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a604c145ba050689b28afa379325c1d581dc20a9e176e51410a35a23ce76bfc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 08:08:09 GMT
ADD file:002f2f7c6dc806b24b6c365882acd59d2b3d3fcec46d8fd99130b07a4575c88c in / 
# Thu, 02 Dec 2021 08:08:10 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 11:59:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 11:59:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 11:59:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 11:59:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 11:59:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 12:04:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 12:04:12 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 12:04:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 12:04:23 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 12:04:24 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 12:04:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:04:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:04:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 13:01:12 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 02 Dec 2021 13:01:13 GMT
ENV PHP_VERSION=7.4.26
# Thu, 02 Dec 2021 13:01:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 02 Dec 2021 13:01:15 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 02 Dec 2021 13:01:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 02 Dec 2021 13:01:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:03:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 02 Dec 2021 13:03:27 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:03:28 GMT
RUN docker-php-ext-enable sodium
# Thu, 02 Dec 2021 13:03:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Dec 2021 13:03:29 GMT
STOPSIGNAL SIGWINCH
# Thu, 02 Dec 2021 13:03:31 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:03:31 GMT
WORKDIR /var/www/html
# Thu, 02 Dec 2021 13:03:32 GMT
EXPOSE 80
# Thu, 02 Dec 2021 13:03:33 GMT
CMD ["apache2-foreground"]
# Fri, 03 Dec 2021 13:20:00 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 03 Dec 2021 13:20:00 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 03 Dec 2021 13:20:01 GMT
RUN a2enmod rewrite
# Fri, 03 Dec 2021 13:21:43 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 13:21:44 GMT
VOLUME [/var/www/html]
# Fri, 03 Dec 2021 13:21:45 GMT
ENV JOOMLA_VERSION=4.0.4
# Fri, 03 Dec 2021 13:21:46 GMT
ENV JOOMLA_SHA512=56dc516fd4596c1f728cf3503d7427dfc755d4b23ad5c170e2ee11d2a1d9e38484b3fa5cb337f8ce9ad8b5108386644d915afda3d3eae0d418dae9bd1d774eb3
# Fri, 03 Dec 2021 13:21:54 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 03 Dec 2021 13:21:55 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Fri, 03 Dec 2021 13:21:56 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 03 Dec 2021 13:21:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 13:21:57 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:968621624b326084ed82349252b333e649eaab39f71866edb2b9a4f847283680`  
		Last Modified: Thu, 02 Dec 2021 08:40:45 GMT  
		Size: 30.1 MB (30056536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908fd1ac141117ff95101d5b08390302a6252e84d47119afbbbe003de9c20b77`  
		Last Modified: Thu, 02 Dec 2021 13:46:39 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1116953363ba7a140c5892cdee723aa4864f10c214e9a5f9fcdc5e43bc6f443f`  
		Last Modified: Thu, 02 Dec 2021 13:46:52 GMT  
		Size: 86.7 MB (86716561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7fa7c61c5bccc19737988eb57f742773cf8250a7c5bf668a489ef72699909e1`  
		Last Modified: Thu, 02 Dec 2021 13:46:39 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6199307de72dbca0947fa83256b339eacde31f10795b9f7ae7ec7807bb91ee9f`  
		Last Modified: Thu, 02 Dec 2021 13:47:55 GMT  
		Size: 18.9 MB (18939806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f08395deb5780095ab847148f33e7355d061e0db4b22f2c9bdde2be435f0d69`  
		Last Modified: Thu, 02 Dec 2021 13:47:52 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c56b2a5279a3303117dc0069ddad9832069c3a2c14d0f21439935267f08776c`  
		Last Modified: Thu, 02 Dec 2021 13:47:52 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27f8157d7a0fbc8e7d72abf9b9abf4564972e8cc7d495848a073694b3e3c88f`  
		Last Modified: Thu, 02 Dec 2021 13:55:54 GMT  
		Size: 10.5 MB (10544424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728c13c3fd0e921bdabc7d2e0a8b79480a0b3d79e3a13e1d080db74b544327c8`  
		Last Modified: Thu, 02 Dec 2021 13:55:50 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789c1836f59ff04326de4345937a46f0b72c0424419533d347241c424cbf2435`  
		Last Modified: Thu, 02 Dec 2021 13:55:53 GMT  
		Size: 13.6 MB (13649725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80326e90121d87d90b175ccb400c38aab6fd3def7a1818f17370a0a5013b996`  
		Last Modified: Thu, 02 Dec 2021 13:55:50 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9d41d4dffe2fe8c013da096c291cce0ec2c1cbce6c7b7b8971f70ac7413a10`  
		Last Modified: Thu, 02 Dec 2021 13:55:51 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ea42386502b194c584d71e1f88f69838db19da91b9267c10597425e0f5cb57`  
		Last Modified: Thu, 02 Dec 2021 13:55:50 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c9029560ee6e786cd02f827213ece346959cf606841c63bfd5a1f38ec14014`  
		Last Modified: Fri, 03 Dec 2021 13:38:23 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e744190d9b4c05576c793cd315513770e0a16392f96679f3c74e36a81fa3cc9`  
		Last Modified: Fri, 03 Dec 2021 13:38:24 GMT  
		Size: 2.8 MB (2808721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04855213c4e5ea5e4e64970f9dd5cca68d8f5ba510a55dcadcfbf896c967bc83`  
		Last Modified: Fri, 03 Dec 2021 13:38:27 GMT  
		Size: 21.6 MB (21566319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946af1762d4baf647afc1b6343adea65436a2cda4aa9a0163c662441b590bcb3`  
		Last Modified: Fri, 03 Dec 2021 13:38:23 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b566142d48b30d81bd4bf647b727303b03acc56614046b11beaeb946baec27`  
		Last Modified: Fri, 03 Dec 2021 13:38:23 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-apache` - linux; 386

```console
$ docker pull joomla@sha256:026a1b6fd39cf8142e14cfd31d111dd1a3b841521f7ca92aa0375a15f7e6a854
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.5 MB (194472665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7e54636f8be11280a11ed42306c113e6774ee093dee16af9a6e1763a7676a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 02:39:54 GMT
ADD file:0284c10b06ba22560408e1e14c1147887f4302c79dba143277ece2e333d6dcbc in / 
# Thu, 02 Dec 2021 02:39:55 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 15:34:51 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 15:34:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 15:35:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 15:35:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 15:35:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 15:41:30 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 15:41:30 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 15:41:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 15:41:42 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 15:41:43 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 15:41:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 15:41:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 15:41:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 17:40:18 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 02 Dec 2021 17:40:19 GMT
ENV PHP_VERSION=7.4.26
# Thu, 02 Dec 2021 17:40:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 02 Dec 2021 17:40:19 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 02 Dec 2021 17:40:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 02 Dec 2021 17:40:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:44:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 02 Dec 2021 17:44:09 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:44:10 GMT
RUN docker-php-ext-enable sodium
# Thu, 02 Dec 2021 17:44:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Dec 2021 17:44:11 GMT
STOPSIGNAL SIGWINCH
# Thu, 02 Dec 2021 17:44:11 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 02 Dec 2021 17:44:11 GMT
WORKDIR /var/www/html
# Thu, 02 Dec 2021 17:44:12 GMT
EXPOSE 80
# Thu, 02 Dec 2021 17:44:12 GMT
CMD ["apache2-foreground"]
# Fri, 03 Dec 2021 08:24:38 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 03 Dec 2021 08:24:38 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 03 Dec 2021 08:24:40 GMT
RUN a2enmod rewrite
# Fri, 03 Dec 2021 08:29:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 08:29:41 GMT
VOLUME [/var/www/html]
# Fri, 03 Dec 2021 08:29:41 GMT
ENV JOOMLA_VERSION=4.0.4
# Fri, 03 Dec 2021 08:29:42 GMT
ENV JOOMLA_SHA512=56dc516fd4596c1f728cf3503d7427dfc755d4b23ad5c170e2ee11d2a1d9e38484b3fa5cb337f8ce9ad8b5108386644d915afda3d3eae0d418dae9bd1d774eb3
# Fri, 03 Dec 2021 08:29:58 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 03 Dec 2021 08:29:59 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Fri, 03 Dec 2021 08:30:00 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 03 Dec 2021 08:30:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 08:30:01 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:2df7932f17d752876c686aa22054692a38e88e182dd7b6a5cca7ffce4ffe6f84`  
		Last Modified: Thu, 02 Dec 2021 02:47:59 GMT  
		Size: 32.4 MB (32380814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006beea53092d7c6fd5356ebb0b4bb1c22e305ea07d7cbd78c420befc8a3c9fe`  
		Last Modified: Thu, 02 Dec 2021 19:02:02 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef59490d4a3bd0c7383a92609286a83f9314e2ffdf7a53d6e060cc507bc9f6d3`  
		Last Modified: Thu, 02 Dec 2021 19:02:26 GMT  
		Size: 92.7 MB (92716335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0716a5cf8d0549d314324c1e362503d39682f1cf88eaf7cddf937b7d75a4f52`  
		Last Modified: Thu, 02 Dec 2021 19:02:01 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f906f03ba636f199744f65d5d1a24b0590bee9b8f7158fdfb59746c0af25e75`  
		Last Modified: Thu, 02 Dec 2021 19:03:39 GMT  
		Size: 19.7 MB (19713950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d2f58a7e697c46662966fac55bfb2f36765a073a078fcb9251a695584869f6`  
		Last Modified: Thu, 02 Dec 2021 19:03:34 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c76c91c58be847d65a50df901fab49b560d8c6f70ad5f3f86f09376f15d83df`  
		Last Modified: Thu, 02 Dec 2021 19:03:34 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a46078dc622606626128050e6f2dfaca35b37a3e6b5e17092bc30d47a053c2`  
		Last Modified: Thu, 02 Dec 2021 19:13:19 GMT  
		Size: 10.8 MB (10759341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4f38f37062d8d4a2a606197bf116d31251d91ede2d3b5a7e7e79d957762c42`  
		Last Modified: Thu, 02 Dec 2021 19:13:15 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb47c8f8c8537d9aaa08f1be4d5c204d6ed8dc1d89df9124941d474833bd045`  
		Last Modified: Thu, 02 Dec 2021 19:13:21 GMT  
		Size: 14.2 MB (14233621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d653211c117466deea74ef7aa5ffa925e722a0e023f2c8a2f394fbe42f9ac2bb`  
		Last Modified: Thu, 02 Dec 2021 19:13:15 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f362e91ec98bbb1f2025271052ab0acf92630576b765bce3be3563e113a8f4f3`  
		Last Modified: Thu, 02 Dec 2021 19:13:15 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba60d51d58ba398452d85888c43bf2dfb7ba533205f03682206e0010719e04cc`  
		Last Modified: Thu, 02 Dec 2021 19:13:15 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff3682f46edd9e0cf1b58fda86dfd674190bdd657b7372949c64c853a30eb66`  
		Last Modified: Fri, 03 Dec 2021 09:01:57 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcecda303df6edf741c9a0187ad0891bb9b9f7163636bb924cf8d7b4517bac3e`  
		Last Modified: Fri, 03 Dec 2021 09:01:59 GMT  
		Size: 3.1 MB (3094636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51f2554141e3cc9fc4b13e24f8b284bb0761227fe3a6856ccc668e25b472e88`  
		Last Modified: Fri, 03 Dec 2021 09:02:06 GMT  
		Size: 21.6 MB (21566408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d87ef8e641189fc2ad1324f607235ee46086ec43b93cc96a07c21e57ebee239`  
		Last Modified: Fri, 03 Dec 2021 09:01:56 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9ccbad6ebd17dd4ce8038487c4ba71a189a3064cb930272b80adaae84640c3`  
		Last Modified: Fri, 03 Dec 2021 09:01:57 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-apache` - linux; mips64le

```console
$ docker pull joomla@sha256:9414c4109c28c48a182be0cf55319eaf5543de1be0651c2ae30a11d30cc7f447
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.3 MB (169309244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9cb3f90084f674868de983a5f93d9395104de7bce5da779869d9ba3a5372969`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 03:09:10 GMT
ADD file:419aff162077eb16923c3ede6455ca86756a929a5a837bc6ac6b8dc67913503a in / 
# Thu, 02 Dec 2021 03:09:10 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 12:32:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 12:32:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 12:33:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 12:33:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 12:33:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 12:47:18 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 03 Dec 2021 12:47:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 03 Dec 2021 12:47:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 03 Dec 2021 12:47:48 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 03 Dec 2021 12:47:50 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 03 Dec 2021 12:47:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 12:47:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 12:47:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 16:12:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 03 Dec 2021 16:12:50 GMT
ENV PHP_VERSION=7.4.26
# Fri, 03 Dec 2021 16:12:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Fri, 03 Dec 2021 16:12:50 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Fri, 03 Dec 2021 16:13:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Dec 2021 16:13:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Dec 2021 16:21:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Dec 2021 16:21:04 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 03 Dec 2021 16:21:06 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Dec 2021 16:21:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Dec 2021 16:21:06 GMT
STOPSIGNAL SIGWINCH
# Fri, 03 Dec 2021 16:21:07 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 03 Dec 2021 16:21:07 GMT
WORKDIR /var/www/html
# Fri, 03 Dec 2021 16:21:08 GMT
EXPOSE 80
# Fri, 03 Dec 2021 16:21:08 GMT
CMD ["apache2-foreground"]
# Sat, 04 Dec 2021 06:08:26 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Sat, 04 Dec 2021 06:08:26 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Sat, 04 Dec 2021 06:08:28 GMT
RUN a2enmod rewrite
# Sat, 04 Dec 2021 06:14:07 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Dec 2021 06:14:07 GMT
VOLUME [/var/www/html]
# Sat, 04 Dec 2021 06:14:08 GMT
ENV JOOMLA_VERSION=4.0.4
# Sat, 04 Dec 2021 06:14:08 GMT
ENV JOOMLA_SHA512=56dc516fd4596c1f728cf3503d7427dfc755d4b23ad5c170e2ee11d2a1d9e38484b3fa5cb337f8ce9ad8b5108386644d915afda3d3eae0d418dae9bd1d774eb3
# Sat, 04 Dec 2021 06:14:30 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Sat, 04 Dec 2021 06:14:32 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Sat, 04 Dec 2021 06:14:32 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Sat, 04 Dec 2021 06:14:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 04 Dec 2021 06:14:33 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:df61fb15db6391af55d70bc3c0db3e9014438c81bf802619fb527221adf5e8a8`  
		Last Modified: Thu, 02 Dec 2021 03:17:58 GMT  
		Size: 29.6 MB (29630496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83c1e85b8a7d8f4eac1893af0c207b44ba6740c84b242afaf7d96af4a26120b`  
		Last Modified: Fri, 03 Dec 2021 18:41:46 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124389778aab42ee498bcb3c59b91b0d2d14f182fd993a4560f80bc5de07b749`  
		Last Modified: Fri, 03 Dec 2021 18:42:42 GMT  
		Size: 72.0 MB (72013733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf72b6001435333c90ef2102c1791b7223d8a3068ff8eaad536bd904a50a3fb5`  
		Last Modified: Fri, 03 Dec 2021 18:41:46 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40088846fba7a0ca24500a32740dc6ad8e0352613d9cb22815f6a240dcceef5`  
		Last Modified: Fri, 03 Dec 2021 18:43:50 GMT  
		Size: 19.1 MB (19143672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49778ac1045f587025ae6cc07c8bcd35ae378477a6c6fb776c95bf453f77f17b`  
		Last Modified: Fri, 03 Dec 2021 18:43:36 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d339f3447da8c4fc93394d91b9b71f7660c2bfcd128edb943f0d95a483794964`  
		Last Modified: Fri, 03 Dec 2021 18:43:35 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd44924406ba401bbfc8292f19444d09f6d238a76f86378c09e3368014d83e8`  
		Last Modified: Fri, 03 Dec 2021 18:55:16 GMT  
		Size: 10.8 MB (10757957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1cafbe683606124baa023120b8ed339bca9371260da1e843581099336598f4`  
		Last Modified: Fri, 03 Dec 2021 18:55:10 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bf5de038308208f205e5fa76d898a92b81387e9abb74e97f1075689a79d7b9`  
		Last Modified: Fri, 03 Dec 2021 18:55:21 GMT  
		Size: 13.2 MB (13195547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e3184de88d37a5540079593a23cb909a934ade0ad122e09939ab85f7d750ad`  
		Last Modified: Fri, 03 Dec 2021 18:55:11 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cf463eafd7629f967282fc37a45805feaea271328264bcb508b47191b130aa`  
		Last Modified: Fri, 03 Dec 2021 18:55:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb2134c2ff3d3e2e81039dee4c3a15fd84bc64fc1c15fda9114589726adaa73`  
		Last Modified: Fri, 03 Dec 2021 18:55:11 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d22c14bb4d95dbaafa9ea035de4ba3093fe8ce8890fc9773eb8e5a70b51cac`  
		Last Modified: Sat, 04 Dec 2021 06:55:15 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bfaa929d9dfdee90ecb45e8f242cd4354d8db8f262829792b9269244cd8e44`  
		Last Modified: Sat, 04 Dec 2021 06:55:18 GMT  
		Size: 3.0 MB (2994122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f61f4b513af6e556bed9d50a5187b27f48e1e44ce4b2bb28491ce18d4749ca`  
		Last Modified: Sat, 04 Dec 2021 06:55:32 GMT  
		Size: 21.6 MB (21566264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5968c6c0951d20a4eb78a60d5f571448162d43cb2c0d6975944a2631ee3f161d`  
		Last Modified: Sat, 04 Dec 2021 06:55:15 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0fcca2ce77ecc0cacf1fd88701f7220cfe9abeb40b2a3b57cda3d925451efc`  
		Last Modified: Sat, 04 Dec 2021 06:55:15 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-apache` - linux; ppc64le

```console
$ docker pull joomla@sha256:cd7fe26ba27cf401d65b08d87b4dc3ea2a80d91ab987a2bfb1b5b9c93c3d762b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.9 MB (192881635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f98a07c451227a73feb3c6ae2c23b7915e296acd84f6741f170755776fcbcc7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 07:21:21 GMT
ADD file:81a93de7f5dcdbb9397c05b9b6bb7dc5a4742119d46faf929b4c6277b02be7a5 in / 
# Thu, 02 Dec 2021 07:21:25 GMT
CMD ["bash"]
# Fri, 03 Dec 2021 01:26:51 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 03 Dec 2021 01:26:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 03 Dec 2021 01:28:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 01:28:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 03 Dec 2021 01:28:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 03 Dec 2021 01:34:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 03 Dec 2021 01:34:46 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 03 Dec 2021 01:35:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 03 Dec 2021 01:35:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 03 Dec 2021 01:35:51 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 03 Dec 2021 01:35:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:35:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 03 Dec 2021 01:35:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 03 Dec 2021 03:07:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 03 Dec 2021 03:07:40 GMT
ENV PHP_VERSION=7.4.26
# Fri, 03 Dec 2021 03:07:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Fri, 03 Dec 2021 03:07:49 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Fri, 03 Dec 2021 03:08:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Dec 2021 03:08:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Dec 2021 03:12:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Dec 2021 03:12:58 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 03 Dec 2021 03:13:02 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Dec 2021 03:13:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Dec 2021 03:13:06 GMT
STOPSIGNAL SIGWINCH
# Fri, 03 Dec 2021 03:13:07 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 03 Dec 2021 03:13:09 GMT
WORKDIR /var/www/html
# Fri, 03 Dec 2021 03:13:11 GMT
EXPOSE 80
# Fri, 03 Dec 2021 03:13:12 GMT
CMD ["apache2-foreground"]
# Fri, 03 Dec 2021 22:25:50 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 03 Dec 2021 22:26:01 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 03 Dec 2021 22:26:13 GMT
RUN a2enmod rewrite
# Fri, 03 Dec 2021 22:30:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Dec 2021 22:30:35 GMT
VOLUME [/var/www/html]
# Fri, 03 Dec 2021 22:30:38 GMT
ENV JOOMLA_VERSION=4.0.4
# Fri, 03 Dec 2021 22:30:41 GMT
ENV JOOMLA_SHA512=56dc516fd4596c1f728cf3503d7427dfc755d4b23ad5c170e2ee11d2a1d9e38484b3fa5cb337f8ce9ad8b5108386644d915afda3d3eae0d418dae9bd1d774eb3
# Fri, 03 Dec 2021 22:30:59 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 03 Dec 2021 22:31:10 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Fri, 03 Dec 2021 22:31:12 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 03 Dec 2021 22:31:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 03 Dec 2021 22:31:23 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8d46978b233ccedeaa1cbef7248b214991469fa922cc4fbf9916f9d0711d2d2e`  
		Last Modified: Thu, 02 Dec 2021 07:31:43 GMT  
		Size: 35.3 MB (35271379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6c286b4294c51bd0937f8e76dc2ab954a5979862c9d67047b7418b5c0c0216`  
		Last Modified: Fri, 03 Dec 2021 04:35:05 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ac0517ba1e5c6ce5c83aa70ead9ee84c78cd00ce5c00d48ab2571f5d2fee6d`  
		Last Modified: Fri, 03 Dec 2021 04:35:45 GMT  
		Size: 86.6 MB (86624644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2593e896803c19e6e62830e0e5445a9811ba89c9c949f6bc9e05bb0dfe769f45`  
		Last Modified: Fri, 03 Dec 2021 04:35:04 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740215b7c8505d1a8f2be9f6d2cc90aa2440a3c336c37775e6108d091f7cc1b4`  
		Last Modified: Fri, 03 Dec 2021 04:36:52 GMT  
		Size: 20.4 MB (20441229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ea4e2fbe7ca3edb06da17d6b4b837ad3995f9bfe993a29c426b443a13551a8a`  
		Last Modified: Fri, 03 Dec 2021 04:36:46 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5828f4ca2a293ab550a55ee804c736545b6b1c480797dbe54ed04eebd76f0b52`  
		Last Modified: Fri, 03 Dec 2021 04:36:46 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935a5cb18d7710124b9c5695849660d76e98408e6ba2a7f5fe2e939116344471`  
		Last Modified: Fri, 03 Dec 2021 04:46:07 GMT  
		Size: 10.8 MB (10760206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b57d84ef60c384868f8fe9ff22ea3db490265987f8b41f8a0f7b55a94b169`  
		Last Modified: Fri, 03 Dec 2021 04:46:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4599ede7fc5f2b786c5885f1a9a1a9db039277050e7cd2aea0068f09c9e491`  
		Last Modified: Fri, 03 Dec 2021 04:46:07 GMT  
		Size: 14.9 MB (14925154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02667b8378a4fe42f130c0736b6d7481194aa085c161ed5a64cdad558a12ea60`  
		Last Modified: Fri, 03 Dec 2021 04:46:04 GMT  
		Size: 2.3 KB (2310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622694d2aa660d6dc6d72e8753af5b79d73005f4ded3e877194d4801a163219d`  
		Last Modified: Fri, 03 Dec 2021 04:46:04 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38eb14484e3c34ad2ce29c6624c60ab246b02058dba005ee58c74035b8363eb`  
		Last Modified: Fri, 03 Dec 2021 04:46:04 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d13a5ad79570ad05eb8d33d2c8b6750678b83ee70f881ddac083f3ed7fdf3`  
		Last Modified: Fri, 03 Dec 2021 23:05:23 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40337ecfcf73e6ed0d5955bd8fac51f84c25dab59ac09c5ac3f4f4c848801a77`  
		Last Modified: Fri, 03 Dec 2021 23:05:24 GMT  
		Size: 3.3 MB (3285050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb265f7757d3b6c4b29c00fc87a32c56780330c5c430108949f8c5bbb65d1b9`  
		Last Modified: Fri, 03 Dec 2021 23:05:28 GMT  
		Size: 21.6 MB (21566409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84fab25985ab31b4c59a68475074f76c2853c5b94ec9fed97bc55b2fc2d96d43`  
		Last Modified: Fri, 03 Dec 2021 23:05:23 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c858ba56c2040c3d316473d424b4b88dd99a810bf07c736dcd04c14980de46b3`  
		Last Modified: Fri, 03 Dec 2021 23:05:23 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:4-php7.4-apache` - linux; s390x

```console
$ docker pull joomla@sha256:9c33599d93f4e8e809d7a61598149999cf903d9cdf6a5de3732fe8a0adf9b9f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **168.8 MB (168827177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e6ea244fd3b3bfeb2215583e36f9ca6ace2ce919b19fd487212c374fe621776`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:07 GMT
ADD file:9303def035f391c14bdca007751c5061f36fe929d5b3f4d725ce376e25f7dd36 in / 
# Thu, 02 Dec 2021 07:19:09 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 12:56:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 02 Dec 2021 12:56:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 02 Dec 2021 12:56:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 12:56:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 02 Dec 2021 12:56:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 02 Dec 2021 12:59:24 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 02 Dec 2021 12:59:25 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 02 Dec 2021 12:59:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 02 Dec 2021 12:59:33 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 02 Dec 2021 12:59:34 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 02 Dec 2021 12:59:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:59:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 02 Dec 2021 12:59:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 02 Dec 2021 13:37:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 02 Dec 2021 13:37:58 GMT
ENV PHP_VERSION=7.4.26
# Thu, 02 Dec 2021 13:37:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 02 Dec 2021 13:37:58 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 02 Dec 2021 13:38:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 02 Dec 2021 13:38:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:39:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 02 Dec 2021 13:39:30 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:39:31 GMT
RUN docker-php-ext-enable sodium
# Thu, 02 Dec 2021 13:39:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Dec 2021 13:39:31 GMT
STOPSIGNAL SIGWINCH
# Thu, 02 Dec 2021 13:39:31 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 02 Dec 2021 13:39:31 GMT
WORKDIR /var/www/html
# Thu, 02 Dec 2021 13:39:32 GMT
EXPOSE 80
# Thu, 02 Dec 2021 13:39:32 GMT
CMD ["apache2-foreground"]
# Thu, 02 Dec 2021 23:10:30 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 02 Dec 2021 23:10:30 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 02 Dec 2021 23:10:31 GMT
RUN a2enmod rewrite
# Thu, 02 Dec 2021 23:11:35 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.1.5; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Dec 2021 23:11:35 GMT
VOLUME [/var/www/html]
# Thu, 02 Dec 2021 23:11:35 GMT
ENV JOOMLA_VERSION=4.0.4
# Thu, 02 Dec 2021 23:11:35 GMT
ENV JOOMLA_SHA512=56dc516fd4596c1f728cf3503d7427dfc755d4b23ad5c170e2ee11d2a1d9e38484b3fa5cb337f8ce9ad8b5108386644d915afda3d3eae0d418dae9bd1d774eb3
# Thu, 02 Dec 2021 23:11:41 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 02 Dec 2021 23:11:43 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 02 Dec 2021 23:11:43 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 02 Dec 2021 23:11:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Dec 2021 23:11:44 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bf2c280d82ca10801fb58bfc3f73029eef17592cbe00e94875cb189bdbac0c5f`  
		Last Modified: Thu, 02 Dec 2021 07:25:12 GMT  
		Size: 29.7 MB (29650954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae19b0f8c96c26b9c7447079b0bf62b84c7f445da800c4d545ed5ed81c44475`  
		Last Modified: Thu, 02 Dec 2021 14:16:10 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74df6370c0af1794838fd1e4579f84cb3c4a3b9e54ae16f2da44d6723c3f3a6`  
		Last Modified: Thu, 02 Dec 2021 14:16:20 GMT  
		Size: 71.6 MB (71617963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c73983b46e5745f144dd89c2613c09f786e736d97f66a5378e2eadd93abb727`  
		Last Modified: Thu, 02 Dec 2021 14:16:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c553899b5d172b0d7a2e657a9322613ad329ab8b0d7154ae56fa58ffcdd9cb`  
		Last Modified: Thu, 02 Dec 2021 14:17:00 GMT  
		Size: 19.1 MB (19052149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05ec9d3bc7cffd2071f8271ccfde370cc722513c89c8fe66579b6d85aa73191`  
		Last Modified: Thu, 02 Dec 2021 14:16:58 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c320fa0b3b7c851180e1f014391ba674c49de9811330f3392a3079f4ca15a1a7`  
		Last Modified: Thu, 02 Dec 2021 14:16:58 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0053d368557bcf8feb86b49160e34949092d2e07f5d8b6587ccf5d3e4949fae`  
		Last Modified: Thu, 02 Dec 2021 14:22:55 GMT  
		Size: 10.8 MB (10758952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198c60d5aafad7742340aff23c1fdd340758c0a935f7a43389b57db29883d9f7`  
		Last Modified: Thu, 02 Dec 2021 14:22:53 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca32b5a96b0cba571b064626dfd2a07fbc9cc50eee53142dd2f7b84b500aa2a`  
		Last Modified: Thu, 02 Dec 2021 14:22:56 GMT  
		Size: 13.1 MB (13144336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1045cfd7a7c6a51e2e8d4796f17d2918fe0d5ab711dbce7e5acaf9a21eaee46`  
		Last Modified: Thu, 02 Dec 2021 14:22:54 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cfc1d25f93abda88738a1c58ebfe6554723e482ece795a182857f516d2220d`  
		Last Modified: Thu, 02 Dec 2021 14:22:53 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07d056be03f143db7b9d2f9c7f842c07bc63676be8f6717688c106f20d14ebb`  
		Last Modified: Thu, 02 Dec 2021 14:22:54 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc3391c30d6037d5d2a331095c99ea25325508a942738ea52c703cdbef0a63b`  
		Last Modified: Thu, 02 Dec 2021 23:23:15 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9b9ba8831011a96897896539455f788c31c215d2f11ea77256fe1e01786ae7`  
		Last Modified: Thu, 02 Dec 2021 23:23:15 GMT  
		Size: 3.0 MB (3028886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad4cc380d811c9ebfe2b3d1e338ee62956c5220dd06c0f034f71a383e57e7f7`  
		Last Modified: Thu, 02 Dec 2021 23:23:18 GMT  
		Size: 21.6 MB (21566385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5958725c1ac772960fa54366c863c725376dc6cb02ec80129238f8d702cd3244`  
		Last Modified: Thu, 02 Dec 2021 23:23:15 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637dad5ad21115fe3d2a9272840abd062238fa42172f9d7f91511f0534e23f46`  
		Last Modified: Thu, 02 Dec 2021 23:23:15 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
