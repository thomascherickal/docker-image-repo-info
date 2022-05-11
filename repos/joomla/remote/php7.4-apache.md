## `joomla:php7.4-apache`

```console
$ docker pull joomla@sha256:8a4ceb4955725bc6b3311970e6eea8ad0fe28f3e0c04227360dcfc326f55496c
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

### `joomla:php7.4-apache` - linux; amd64

```console
$ docker pull joomla@sha256:934a37b995b2a18e654813c9f92ccb3be616dbb36bcbf2ffa0ab846a6e3fd135
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.6 MB (188645523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51cf854ca24b466273c73361831c81512e2241cf29944ddb8409c31f402bea9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:17:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Apr 2022 11:17:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Apr 2022 11:18:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:18:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Apr 2022 11:18:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 20 Apr 2022 11:21:28 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Apr 2022 11:21:28 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Apr 2022 11:21:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Apr 2022 11:21:37 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Apr 2022 11:21:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Apr 2022 11:21:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Apr 2022 11:21:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Apr 2022 11:21:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Apr 2022 12:12:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 20 Apr 2022 12:12:26 GMT
ENV PHP_VERSION=7.4.29
# Wed, 20 Apr 2022 12:12:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 20 Apr 2022 12:12:26 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 20 Apr 2022 12:12:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Apr 2022 12:12:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Apr 2022 12:14:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Apr 2022 12:14:26 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Apr 2022 12:14:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Apr 2022 12:14:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Apr 2022 12:14:27 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Apr 2022 12:14:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Apr 2022 12:14:27 GMT
WORKDIR /var/www/html
# Wed, 20 Apr 2022 12:14:27 GMT
EXPOSE 80
# Wed, 20 Apr 2022 12:14:27 GMT
CMD ["apache2-foreground"]
# Thu, 21 Apr 2022 10:00:40 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 21 Apr 2022 10:00:40 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 21 Apr 2022 10:00:41 GMT
RUN a2enmod rewrite
# Thu, 21 Apr 2022 10:02:13 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 10:02:13 GMT
VOLUME [/var/www/html]
# Thu, 21 Apr 2022 10:02:13 GMT
ENV JOOMLA_VERSION=4.1.2
# Thu, 21 Apr 2022 10:02:13 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Thu, 21 Apr 2022 10:02:19 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 21 Apr 2022 10:02:20 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Thu, 21 Apr 2022 10:02:20 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 21 Apr 2022 10:02:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Apr 2022 10:02:20 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:012a3732d045340a3dc134901bd26323e110832b987a23c9090004d618db2f8e`  
		Last Modified: Wed, 20 Apr 2022 12:31:34 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43092314d50ddcd60bd7952a240eed4ac448241b205a2dd92291219d977fb4d2`  
		Last Modified: Wed, 20 Apr 2022 12:31:48 GMT  
		Size: 91.6 MB (91602110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f615e42d863613d2afbf86fbbe2546444c6f983cfd2ba757a0533b3bc72b8dc`  
		Last Modified: Wed, 20 Apr 2022 12:31:34 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd39010a4efc82612859368c6702d1683701c5ceb15b024f087f7bd72c62ebda`  
		Last Modified: Wed, 20 Apr 2022 12:32:48 GMT  
		Size: 19.2 MB (19248616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d983c9ce24de82fa71d2579998d92374a39001e583a044a0c624fa9914d0f9ab`  
		Last Modified: Wed, 20 Apr 2022 12:32:46 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbdd59ae430584ee85ce938d09ad28f04c7308689f7adeeafed134c205492d1`  
		Last Modified: Wed, 20 Apr 2022 12:32:46 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d02b88c86184fb178b62074c3f76c885c1521cdf98541b49b641ccd241004f0`  
		Last Modified: Wed, 20 Apr 2022 12:40:34 GMT  
		Size: 10.8 MB (10758631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a246031d43e09937f7cbaba243d807b0a16c917d26c17a7a39e521250c1a1d`  
		Last Modified: Wed, 20 Apr 2022 12:40:30 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c0267e6c346f68cc7e514ba9b84716e7cc5542e5be22e1457edec0d5962764`  
		Last Modified: Wed, 20 Apr 2022 12:40:32 GMT  
		Size: 10.2 MB (10196814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787ca6348cef43213e0cc7654f2a18c6d91a6ffd3e84d26a938bb2926a7cc90c`  
		Last Modified: Wed, 20 Apr 2022 12:40:30 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8ad43595e2730d6c9054e0c8ecb6b1357597659a503e77331e4b824db638ac`  
		Last Modified: Wed, 20 Apr 2022 12:40:30 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e191f9e80e295f3e236722e2888e409fdd5886667c80fd7488469ae3807e240f`  
		Last Modified: Wed, 20 Apr 2022 12:40:30 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90b9d025ca701107aa9d8be441452f7c6832eaa321bdfb5f0aad0a74e24c9e`  
		Last Modified: Thu, 21 Apr 2022 10:16:03 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a72fcef5c6f0990df4e5852fa8bed98a1253392b2774faadc5663990586f8f8`  
		Last Modified: Thu, 21 Apr 2022 10:16:04 GMT  
		Size: 3.1 MB (3107385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73769e851c6145d06ae30ebda3ddf6c8bf4549aec5c53d0d8e8e67a4d7cd4532`  
		Last Modified: Thu, 21 Apr 2022 10:16:07 GMT  
		Size: 22.3 MB (22344661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad46999941e0eb70d887e2fac2ff60fe554557f8d5745b8a02c736ea3f887b16`  
		Last Modified: Thu, 21 Apr 2022 10:16:03 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1dce1e05968faa241643171474a67dc78c81ed45d96cd7cdde34d978888017`  
		Last Modified: Thu, 21 Apr 2022 10:16:03 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-apache` - linux; arm variant v5

```console
$ docker pull joomla@sha256:3fd2b284742044fed7232291cda7a48dabceb181eb88844791387c78f1f65970
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.7 MB (166742988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08bd0034fe9bb4de0df5b8031b4432d2c8350820dd38ebf69a90277c55c33292`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Apr 2022 07:16:42 GMT
ADD file:f20c57847025604e1ea1a848af3f090f71d78b5fc2eb2ac795822da94d6e6a0a in / 
# Wed, 20 Apr 2022 07:16:43 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 23:58:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Apr 2022 23:58:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Apr 2022 23:59:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 23:59:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Apr 2022 23:59:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 21 Apr 2022 00:06:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 21 Apr 2022 00:06:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 21 Apr 2022 00:07:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 21 Apr 2022 00:07:10 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 21 Apr 2022 00:07:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 21 Apr 2022 00:07:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 00:07:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 00:07:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 21 Apr 2022 01:35:52 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 21 Apr 2022 01:35:53 GMT
ENV PHP_VERSION=7.4.29
# Thu, 21 Apr 2022 01:35:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Thu, 21 Apr 2022 01:35:53 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Thu, 21 Apr 2022 01:36:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Apr 2022 01:36:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Apr 2022 01:40:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Apr 2022 01:40:18 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 21 Apr 2022 01:40:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Apr 2022 01:40:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Apr 2022 01:40:21 GMT
STOPSIGNAL SIGWINCH
# Thu, 21 Apr 2022 01:40:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 21 Apr 2022 01:40:22 GMT
WORKDIR /var/www/html
# Thu, 21 Apr 2022 01:40:22 GMT
EXPOSE 80
# Thu, 21 Apr 2022 01:40:23 GMT
CMD ["apache2-foreground"]
# Thu, 21 Apr 2022 17:48:46 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 21 Apr 2022 17:48:46 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 21 Apr 2022 17:48:48 GMT
RUN a2enmod rewrite
# Thu, 21 Apr 2022 17:53:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 17:53:47 GMT
VOLUME [/var/www/html]
# Thu, 21 Apr 2022 17:53:48 GMT
ENV JOOMLA_VERSION=4.1.2
# Thu, 21 Apr 2022 17:53:48 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Thu, 21 Apr 2022 17:54:06 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 21 Apr 2022 17:54:08 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Thu, 21 Apr 2022 17:54:08 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 21 Apr 2022 17:54:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Apr 2022 17:54:09 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3edd9d296fa023e00f76828c9d6fd6cc5b03e626341a6a045c40d2ea16c32d08`  
		Last Modified: Wed, 20 Apr 2022 07:32:27 GMT  
		Size: 28.9 MB (28921085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b3b92a382ea7fe97048f7942a8b716c9d41bca684f33190a1b6f222f9790be`  
		Last Modified: Thu, 21 Apr 2022 02:18:56 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e4cac9134496ebb2f101cb1e584faea40cd37a49f5e044337e02ef8d17d2b1`  
		Last Modified: Thu, 21 Apr 2022 02:19:46 GMT  
		Size: 73.7 MB (73683459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1a04c0b586dd8771be9ba83febdff607ee72bf05240eb26e7b97f725ca8aa0`  
		Last Modified: Thu, 21 Apr 2022 02:18:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f503b6ba6833c80c02ec36c57bbe468d3331434e911f838704942b90985b21`  
		Last Modified: Thu, 21 Apr 2022 02:21:10 GMT  
		Size: 18.5 MB (18545918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d01410e4543037acb7c208ada6834f2a2c52db6ef29a5176443be6badf3539`  
		Last Modified: Thu, 21 Apr 2022 02:20:59 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01fa16f28c21b7ba2705d4c32ae1ef73509d510e2b885cb4c868ee65765227ce`  
		Last Modified: Thu, 21 Apr 2022 02:20:59 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d215767f2956624c6085e1965de3d33d813c75ff4be5889c4d126add31b376`  
		Last Modified: Thu, 21 Apr 2022 02:32:24 GMT  
		Size: 10.8 MB (10757383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004520f947f672e97b60fe2ca7610567ac503615d35b39eaf5bc86a57f51808e`  
		Last Modified: Thu, 21 Apr 2022 02:32:19 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a1f660447361760daf550ad653076453683a456b3c5868da6010d6f50bdbb8`  
		Last Modified: Thu, 21 Apr 2022 02:32:26 GMT  
		Size: 9.6 MB (9573142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df61c6d4fdf63116f56ce0b998737ff4d66cc511f84382fc1451230c91dba8b4`  
		Last Modified: Thu, 21 Apr 2022 02:32:19 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9157969dd2f4f8f294b3affb834487ff6cfea78fa48266addf48c42fb2e20ff`  
		Last Modified: Thu, 21 Apr 2022 02:32:19 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7e9a41477b6046d7666535662847ec677b77da671d09ba498d08cfe1480fb1`  
		Last Modified: Thu, 21 Apr 2022 02:32:20 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e147a9a1d7756d95eebab1e48759b9d00413f329addc5a7fe532f6117163e76e`  
		Last Modified: Thu, 21 Apr 2022 18:36:14 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15da1d9aacb69a19a670a3f39120f7ab4be3f8e786a0cd176c1d439df72fc281`  
		Last Modified: Thu, 21 Apr 2022 18:36:16 GMT  
		Size: 2.9 MB (2909030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b114a695130d75a6b2afe28a42079d0730d9342ac90401baa5d27731fa918a3`  
		Last Modified: Thu, 21 Apr 2022 18:36:34 GMT  
		Size: 22.3 MB (22344642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e760b9fd3da0d0394f4bac0cbf229086defa9043ebd1ccaa2877851e09271f`  
		Last Modified: Thu, 21 Apr 2022 18:36:14 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d8ed230fbb3c66e519e9786bff7b3caee35fbf43cb21c805e931fca5abf80a`  
		Last Modified: Thu, 21 Apr 2022 18:36:14 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-apache` - linux; arm variant v7

```console
$ docker pull joomla@sha256:aad7023de9fc81cff151307b9d4854042fb31aa36601280ca36123ad8ddb3cbe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.9 MB (158879475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5dc1c03e50d6dbb15d1ee073be1ad3cecc1f7eecc148be1245c2fddf7a91db`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Apr 2022 13:27:18 GMT
ADD file:1a0e290eb32b3533f9d1684c683ad866b5003579790b25ad61b2044dc6c20bbb in / 
# Wed, 20 Apr 2022 13:27:18 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 14:16:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 21 Apr 2022 14:16:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 21 Apr 2022 14:17:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 14:17:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 21 Apr 2022 14:17:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 21 Apr 2022 14:22:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 21 Apr 2022 14:22:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 21 Apr 2022 14:23:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 21 Apr 2022 14:23:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 21 Apr 2022 14:23:11 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 21 Apr 2022 14:23:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 14:23:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 14:23:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 21 Apr 2022 15:46:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 21 Apr 2022 15:46:48 GMT
ENV PHP_VERSION=7.4.29
# Thu, 21 Apr 2022 15:46:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Thu, 21 Apr 2022 15:46:49 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Thu, 21 Apr 2022 15:47:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Apr 2022 15:47:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Apr 2022 15:50:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Apr 2022 15:50:42 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 21 Apr 2022 15:50:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Apr 2022 15:50:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Apr 2022 15:50:44 GMT
STOPSIGNAL SIGWINCH
# Thu, 21 Apr 2022 15:50:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 21 Apr 2022 15:50:45 GMT
WORKDIR /var/www/html
# Thu, 21 Apr 2022 15:50:46 GMT
EXPOSE 80
# Thu, 21 Apr 2022 15:50:46 GMT
CMD ["apache2-foreground"]
# Fri, 22 Apr 2022 16:13:22 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 22 Apr 2022 16:13:22 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 22 Apr 2022 16:13:24 GMT
RUN a2enmod rewrite
# Fri, 22 Apr 2022 16:18:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 16:18:10 GMT
VOLUME [/var/www/html]
# Fri, 22 Apr 2022 16:18:10 GMT
ENV JOOMLA_VERSION=4.1.2
# Fri, 22 Apr 2022 16:18:11 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Fri, 22 Apr 2022 16:18:28 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 22 Apr 2022 16:18:30 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 22 Apr 2022 16:18:30 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 22 Apr 2022 16:18:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Apr 2022 16:18:31 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a6b2963233cd14b47391f0e25f2a485bbeabb87e771a71b73e5cde7c013963da`  
		Last Modified: Wed, 20 Apr 2022 13:43:41 GMT  
		Size: 26.6 MB (26575758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b6b2706f2ab155a1aa75f913f2f6a946f438652f2588747c8457de78564ff2`  
		Last Modified: Thu, 21 Apr 2022 16:34:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d413824c0d6337c3b6aaea376d2d125d16991e18b1ee338d090a759467ae3b`  
		Last Modified: Thu, 21 Apr 2022 16:34:59 GMT  
		Size: 69.3 MB (69315918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311ab91865a3753968a48b7962ae371de7f1346692b824d03c5b550e6e4ed84d`  
		Last Modified: Thu, 21 Apr 2022 16:34:16 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee189dc14282eb2b4a9c40a4af6e3c095a570629c413ede3221c73b14fce0bd`  
		Last Modified: Thu, 21 Apr 2022 16:36:19 GMT  
		Size: 18.0 MB (17993448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2eff9fbb6ce9aedfc44728d4045a93526dc28a5e020a2ae3cfd3f5ecfb0555c`  
		Last Modified: Thu, 21 Apr 2022 16:36:10 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2198b0316ea5b8861d35ec0a988c202a4aba2aabef2193f88800bb3df2da83`  
		Last Modified: Thu, 21 Apr 2022 16:36:10 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a42f718672a9e3812588658b9b47f9cde927b6332231d9bebce8f0ad44ef53`  
		Last Modified: Thu, 21 Apr 2022 20:09:03 GMT  
		Size: 10.8 MB (10757350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d31c682cc69aea0c0981070060ee138886da32416752d0b42eb6c2c47a50a46`  
		Last Modified: Thu, 21 Apr 2022 20:08:59 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e74b47014b91396e1559c72303b2671d8e8d7b8f4c7a15ce3bc619f7242aaa`  
		Last Modified: Thu, 21 Apr 2022 20:09:05 GMT  
		Size: 9.1 MB (9088365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fb47e0053103c51ad67914147350ae59c5976abedde89768c22b8ddc1dea1f`  
		Last Modified: Thu, 21 Apr 2022 20:08:58 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0b51a69a00ff6df69b293816f1b8854562b5d27c83f9cb38bb7065ff179ecb`  
		Last Modified: Thu, 21 Apr 2022 20:08:59 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fe1f6de0a8449d0c7e5e1e586c45339c597966c912554ca5b29737faa4779e`  
		Last Modified: Thu, 21 Apr 2022 20:08:59 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335480d9bb9aacba4115cc60a80f95392d575f9ac68d6f446769891581d3391c`  
		Last Modified: Fri, 22 Apr 2022 17:00:42 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9cfddd1247f5b53ecdf5ac23438af3200282e0279c0bdca932f79fd3e524c8`  
		Last Modified: Fri, 22 Apr 2022 17:00:43 GMT  
		Size: 2.8 MB (2795637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68352b590847bd35339bb05a66c7ab37bd7b093d18f2b091ee56c7442d4265fc`  
		Last Modified: Fri, 22 Apr 2022 17:01:01 GMT  
		Size: 22.3 MB (22344657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7001615c48f4ad18c1cf297a825a706b712673993af7d5c15872401456ed552`  
		Last Modified: Fri, 22 Apr 2022 17:00:42 GMT  
		Size: 1.8 KB (1828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5121dd204f58ff2b7df70583f297e3d6ffda2b737c26f8bfbdbd0bd4edd6c5b0`  
		Last Modified: Fri, 22 Apr 2022 17:00:42 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-apache` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:d023a105dac635994543a9a76cd28285e9ce3b22372e3bd6a9ce989b2e103bea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.5 MB (181460966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98da78fe0d2e12144bc9ee700ef684880c96c30731cd58e3c7fc563bd89611ef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Apr 2022 04:29:10 GMT
ADD file:84523b5820128293b713ef35d8db618921162250da1e4c72bf9923f34ad7d87d in / 
# Wed, 20 Apr 2022 04:29:11 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 15:54:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Apr 2022 15:54:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Apr 2022 15:54:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 15:54:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Apr 2022 15:54:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 20 Apr 2022 15:59:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Apr 2022 15:59:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Apr 2022 15:59:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Apr 2022 15:59:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Apr 2022 15:59:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Apr 2022 15:59:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Apr 2022 15:59:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Apr 2022 15:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Apr 2022 16:55:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 20 Apr 2022 16:55:08 GMT
ENV PHP_VERSION=7.4.29
# Wed, 20 Apr 2022 16:55:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 20 Apr 2022 16:55:10 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 20 Apr 2022 16:55:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Apr 2022 16:55:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Apr 2022 16:57:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Apr 2022 16:57:13 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Apr 2022 16:57:13 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Apr 2022 16:57:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Apr 2022 16:57:15 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Apr 2022 16:57:17 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Apr 2022 16:57:17 GMT
WORKDIR /var/www/html
# Wed, 20 Apr 2022 16:57:18 GMT
EXPOSE 80
# Wed, 20 Apr 2022 16:57:19 GMT
CMD ["apache2-foreground"]
# Thu, 21 Apr 2022 11:45:12 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Thu, 21 Apr 2022 11:45:13 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 21 Apr 2022 11:45:14 GMT
RUN a2enmod rewrite
# Thu, 21 Apr 2022 11:46:58 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 11:46:58 GMT
VOLUME [/var/www/html]
# Thu, 21 Apr 2022 11:46:59 GMT
ENV JOOMLA_VERSION=4.1.2
# Thu, 21 Apr 2022 11:47:00 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Thu, 21 Apr 2022 11:47:08 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 21 Apr 2022 11:47:09 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Thu, 21 Apr 2022 11:47:10 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 21 Apr 2022 11:47:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Apr 2022 11:47:12 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6d4a449ac69c579312443ded09f57c4894e7adb42f7406abd364f95982fafc59`  
		Last Modified: Wed, 20 Apr 2022 04:35:49 GMT  
		Size: 30.1 MB (30065801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12d3b4aaab6372eb007a3b03d4e9a17823b75d804263acbc9a03b2f3d593bc6`  
		Last Modified: Wed, 20 Apr 2022 17:18:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c2be72a6916b19486404e4d330c2e0a38171287eba1738db1a7ea91e55df9e`  
		Last Modified: Wed, 20 Apr 2022 17:19:10 GMT  
		Size: 86.7 MB (86716247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98bf1b5854e24b3036bea49382784344c1d97960e743ddb2710a995c9b4cd14a`  
		Last Modified: Wed, 20 Apr 2022 17:18:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca77433480c40e1f7c7351c258795111dd1f49d6ab00cfb7a34e115163a14740`  
		Last Modified: Wed, 20 Apr 2022 17:20:12 GMT  
		Size: 18.9 MB (18943645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f570ffb0fe936ae55af1cde0ec66c434f04c00fa24e2eff370064cb8a166fb`  
		Last Modified: Wed, 20 Apr 2022 17:20:09 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8475ba7a33e1fc763e296130b7877f96e80fd8d31784985b453d40dbfcab48`  
		Last Modified: Wed, 20 Apr 2022 17:20:10 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065bd0243ba82813d8cbad9a49b7511d085f0c7f749e0836b541e3aaf4dbea5`  
		Last Modified: Wed, 20 Apr 2022 17:28:21 GMT  
		Size: 10.5 MB (10542824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2009452f3ca7cbec8d9dc393372338a59fc603f21e4466f18cf569ebb21492dd`  
		Last Modified: Wed, 20 Apr 2022 17:28:18 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57925945bf0fbc3eca05adbab5df3ab87f180c925b64533937b63c4e5834af6`  
		Last Modified: Wed, 20 Apr 2022 17:28:20 GMT  
		Size: 10.0 MB (9998957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bc9a42114f6e9af70a584f912bc446f9c691fc97835503b9ab9109d6a12106`  
		Last Modified: Wed, 20 Apr 2022 17:28:18 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33326e9876141e67b5c2484613a1e51eceb8ef30a08dba97340175aba4772377`  
		Last Modified: Wed, 20 Apr 2022 17:28:18 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd4f7b6fad555f7135ebc170ead80a57cf02d42e50b1d0be78e6bfc6900028a`  
		Last Modified: Wed, 20 Apr 2022 17:28:18 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7800b392843e99b587b68519577027a0ed0e67c31a592fdd8755b718041aeb10`  
		Last Modified: Thu, 21 Apr 2022 12:04:16 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b3b86463b9b2e5cd1989640db73674f54cbed6d2643a689550fbcee59717aa`  
		Last Modified: Thu, 21 Apr 2022 12:04:17 GMT  
		Size: 2.8 MB (2839743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2ba42fd0246cd6e2f2bfbc6a9f6d1d39a387380fa2fa86565043b5f9484707`  
		Last Modified: Thu, 21 Apr 2022 12:04:20 GMT  
		Size: 22.3 MB (22345535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def203713aaf2f2ca25eb08ddb64f05603b98b5a07923152331618428ee4b32e`  
		Last Modified: Thu, 21 Apr 2022 12:04:16 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd33e979811f3c0c65b789d4256a9f32127a22a46d7c1d5021cb52469d02f8a`  
		Last Modified: Thu, 21 Apr 2022 12:04:16 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-apache` - linux; 386

```console
$ docker pull joomla@sha256:64d028895a97868198073fbd8d4cb7c1ce898e90e5aa46b832ad3c1405172baf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.4 MB (190405534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29bc264306981a6d87e94e1db2e93666d5d79d08dc1f0994b1dd71c18a151384`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 07:12:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 07:12:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 07:12:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 07:12:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 07:12:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 07:15:52 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 07:15:53 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 07:16:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 07:16:05 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 07:16:06 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 07:16:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 07:16:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 07:16:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 08:57:00 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 11 May 2022 08:57:01 GMT
ENV PHP_VERSION=7.4.29
# Wed, 11 May 2022 08:57:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 11 May 2022 08:57:03 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 11 May 2022 08:57:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 08:57:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 08:58:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 08:58:59 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 May 2022 08:58:59 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 08:59:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 08:59:01 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 May 2022 08:59:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 May 2022 08:59:03 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 08:59:04 GMT
EXPOSE 80
# Wed, 11 May 2022 08:59:05 GMT
CMD ["apache2-foreground"]
# Wed, 11 May 2022 19:26:19 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 11 May 2022 19:26:20 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 11 May 2022 19:26:21 GMT
RUN a2enmod rewrite
# Wed, 11 May 2022 19:27:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 19:27:49 GMT
VOLUME [/var/www/html]
# Wed, 11 May 2022 21:38:46 GMT
ENV JOOMLA_VERSION=4.1.3
# Wed, 11 May 2022 21:38:46 GMT
ENV JOOMLA_SHA512=7937355529688adffe2d470bd49da89cddef1b10eca6e3ef20acfd2ebfb695fa3fa346352a68bc094787dd48fe9a2d06371038ce8894cf5ebb0197b3b6140bef
# Wed, 11 May 2022 21:38:55 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 11 May 2022 21:38:56 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Wed, 11 May 2022 21:38:57 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Wed, 11 May 2022 21:38:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 21:38:58 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7e0ab62bdf2006dcf0edb4bfd75f18ad278cc2688d9df909a02a0a68ef2d93`  
		Last Modified: Wed, 11 May 2022 09:24:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eaa23ffdeeb3c581979e596c004018640f1930f73b1ed2bf4edc782bfb5eb8`  
		Last Modified: Wed, 11 May 2022 09:24:15 GMT  
		Size: 92.5 MB (92510632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd517709db67f5f33db055442765cc831c277e3d797ce5def1cc069a78a5d93`  
		Last Modified: Wed, 11 May 2022 09:24:02 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5182b5d92746f4c930f66dde79c4f5544123a1b5cd5720bc1733f3c7a71761`  
		Last Modified: Wed, 11 May 2022 09:24:52 GMT  
		Size: 19.5 MB (19501916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20befabef06022876526393b1ac8e9d5a3d3e3822486e3ce6ce880b44c39112a`  
		Last Modified: Wed, 11 May 2022 09:24:48 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6417be0fc5e9629e325bb548147323a2984945a2ac094e57b1beb6c4698d4eb3`  
		Last Modified: Wed, 11 May 2022 09:24:49 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd9d82847f957093c0d922846e4da761b9eeb9bbd85fa5c0c1e9d4425c7cb46`  
		Last Modified: Wed, 11 May 2022 09:39:53 GMT  
		Size: 10.5 MB (10542869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68119a7a791687a526a66ace3decc107fed32a275afaaebca4b3020a80c90f6`  
		Last Modified: Wed, 11 May 2022 09:39:49 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1e557cec41f86150cd821c2d1bb8d83ba4650f7f83c10f44ec040fa543f67d`  
		Last Modified: Wed, 11 May 2022 09:39:51 GMT  
		Size: 10.4 MB (10442331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78d8579ac7cafbb37bab802143c3168d5163648500ca99fe864e07f613b592a`  
		Last Modified: Wed, 11 May 2022 09:39:49 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcbb45ddcb0b61e0eb231677fbc7a09fe0e1c38ccf229fe716a4517577449d4`  
		Last Modified: Wed, 11 May 2022 09:39:49 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129d70e5eefd0d51eb2bd1d67dd03f3e37e95c33d9a7c39ccb796484ccb9b99d`  
		Last Modified: Wed, 11 May 2022 09:39:49 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c963b547d74d767cf95f9bfe2161b8ec456a384f6f5d79d51b7c08f515e37374`  
		Last Modified: Wed, 11 May 2022 19:43:42 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3171947229025292ac0c90b3442522cbbeb6c93fbe7da13d02e78c5e39f12d16`  
		Last Modified: Wed, 11 May 2022 19:43:43 GMT  
		Size: 2.9 MB (2908135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6f958defeda9f575d9cb0aeed5aac9f4b6bc9f80e7fc92f3f77435da24f793`  
		Last Modified: Wed, 11 May 2022 21:44:33 GMT  
		Size: 22.1 MB (22101668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecfc414af9aad1e11fdce06791033fbc1252589ce6260159938ecfb4dbe844a`  
		Last Modified: Wed, 11 May 2022 21:44:29 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66796798059bee9d76738cb3d7069e3c8a0177e8c0b179101bf409663c1afb9b`  
		Last Modified: Wed, 11 May 2022 21:44:29 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-apache` - linux; mips64le

```console
$ docker pull joomla@sha256:41b2ff501f893c0b3db81790be13a7f2afc1d2db7c899b6f338ebd1b75791c50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.8 MB (165785457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3086bad3dcafa54e246be4e9d0814efc3e7ad5295b66b0ec8e55a0ee9c6d841e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Apr 2022 14:28:35 GMT
ADD file:11939fa9b6e0a3bde2ba32552130208df232ae0dd139b9244b80fa309690d57f in / 
# Wed, 20 Apr 2022 14:28:39 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 17:59:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 21 Apr 2022 17:59:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 21 Apr 2022 18:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 18:00:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 21 Apr 2022 18:00:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 21 Apr 2022 18:15:25 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 21 Apr 2022 18:15:29 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 21 Apr 2022 18:16:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 21 Apr 2022 18:16:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 21 Apr 2022 18:16:39 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 21 Apr 2022 18:16:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 18:16:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 18:16:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 21 Apr 2022 21:59:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 21 Apr 2022 21:59:13 GMT
ENV PHP_VERSION=7.4.29
# Thu, 21 Apr 2022 21:59:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Thu, 21 Apr 2022 21:59:20 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Thu, 21 Apr 2022 22:00:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Apr 2022 22:00:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Apr 2022 22:09:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Apr 2022 22:09:14 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 21 Apr 2022 22:09:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Apr 2022 22:09:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Apr 2022 22:09:28 GMT
STOPSIGNAL SIGWINCH
# Thu, 21 Apr 2022 22:09:31 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 21 Apr 2022 22:09:34 GMT
WORKDIR /var/www/html
# Thu, 21 Apr 2022 22:09:38 GMT
EXPOSE 80
# Thu, 21 Apr 2022 22:09:41 GMT
CMD ["apache2-foreground"]
# Fri, 22 Apr 2022 13:15:19 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 22 Apr 2022 13:15:23 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 22 Apr 2022 13:15:31 GMT
RUN a2enmod rewrite
# Fri, 22 Apr 2022 13:21:45 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 13:21:49 GMT
VOLUME [/var/www/html]
# Fri, 22 Apr 2022 13:21:53 GMT
ENV JOOMLA_VERSION=4.1.2
# Fri, 22 Apr 2022 13:21:57 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Fri, 22 Apr 2022 13:22:32 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 22 Apr 2022 13:22:39 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 22 Apr 2022 13:22:44 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 22 Apr 2022 13:22:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Apr 2022 13:22:57 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:211e565c951d5d12adf5ac13e34b5fdba747f88e6b462c2863538110b219144c`  
		Last Modified: Wed, 20 Apr 2022 14:39:17 GMT  
		Size: 29.6 MB (29641236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f739687e56cfb7a039de711643daf3c882b0f0040b289151a3f02e754bccd8fc`  
		Last Modified: Thu, 21 Apr 2022 23:16:58 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78f566aca9c129a58c56dc58d051b7ab1ec32112f2d923b0f2a3acfe23a867d`  
		Last Modified: Thu, 21 Apr 2022 23:17:50 GMT  
		Size: 71.8 MB (71809771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f5aa368f0ac8f0b25a917bc3a340bff52fbcc5d7c19d68996080dd575e7061`  
		Last Modified: Thu, 21 Apr 2022 23:16:57 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e12a00b02915534722ebef7593fece5bb4bc5b3f306fb8a5d249d4c710c35c`  
		Last Modified: Thu, 21 Apr 2022 23:19:00 GMT  
		Size: 18.9 MB (18933413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643862533faeeb728a54e3428a58486efa9c5af50d2bc03799a502c6a7aa194b`  
		Last Modified: Thu, 21 Apr 2022 23:18:47 GMT  
		Size: 441.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07785999b3a68cf18aaf8dbd96d07c3a88101c1921a50046d360e0dfdafd8db`  
		Last Modified: Thu, 21 Apr 2022 23:18:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f67d16c3e04aff757fcc2273441cce5a806f88e6e5d2944b34d93d844e78af`  
		Last Modified: Thu, 21 Apr 2022 23:28:56 GMT  
		Size: 10.5 MB (10541574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835efb1f3e8cd4d5496d6dac27d2518847a7b366d58c6eb586afa0f259befe0e`  
		Last Modified: Thu, 21 Apr 2022 23:28:52 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5363fbc9aa432dde8002a7f942e1a204aae317f483f3f901984381d720faa4d`  
		Last Modified: Thu, 21 Apr 2022 23:28:59 GMT  
		Size: 9.7 MB (9693332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b0885c1e114601bdd3e110edeb785d1e82e4ad53f0bcc3e7df10934658cb27`  
		Last Modified: Thu, 21 Apr 2022 23:28:51 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e65e50af184156967936f2264be6940d290af83ec459e179ce343c7d823f688`  
		Last Modified: Thu, 21 Apr 2022 23:28:51 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adaf70b872bc72cd99a153a58dd1ca80efceb29d5e4a259400c265ffb02e790`  
		Last Modified: Thu, 21 Apr 2022 23:28:51 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6182a220c3c46f3f7a8d09391587b903e1ada0902c384b374106f4fac1365c92`  
		Last Modified: Fri, 22 Apr 2022 14:15:15 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e131cabaf8d836f04a56ab305a03ad5f6861170c1bef62fb6d87e1d5f2eadb73`  
		Last Modified: Fri, 22 Apr 2022 14:15:18 GMT  
		Size: 2.8 MB (2812316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e942f1e18c8bef688c0ddda85384cde0b2fb97982278805c8dc63a96ab1b7aa9`  
		Last Modified: Fri, 22 Apr 2022 14:15:32 GMT  
		Size: 22.3 MB (22345571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a065af67324c865922c4cd219dbeb2b25153d4deb25178f3bc23db8c39c69d2`  
		Last Modified: Fri, 22 Apr 2022 14:15:15 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0529b0922c5e926419205ab03ec975c1fb0ad5299e8f628a3e884b998cd5bc37`  
		Last Modified: Fri, 22 Apr 2022 14:15:15 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-apache` - linux; ppc64le

```console
$ docker pull joomla@sha256:b42e374188b14e861ca21a39c2297cf568864da1dcca793305317b441f0f8109
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.7 MB (189685885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:937ea118611ef67db1e85d3e9e59a497faf237e19095350feca62c31a5c6e861`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Apr 2022 09:46:36 GMT
ADD file:8d406ebce4d9b0884d46ee25ec31fe7714726024b80aba9b408d81d39e2f6f8c in / 
# Wed, 20 Apr 2022 09:46:44 GMT
CMD ["bash"]
# Thu, 21 Apr 2022 00:57:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 21 Apr 2022 00:57:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 21 Apr 2022 00:59:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 00:59:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 21 Apr 2022 00:59:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 21 Apr 2022 01:05:33 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 21 Apr 2022 01:05:36 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 21 Apr 2022 01:06:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 21 Apr 2022 01:06:42 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 21 Apr 2022 01:06:47 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 21 Apr 2022 01:06:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 01:06:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 21 Apr 2022 01:06:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 21 Apr 2022 02:46:42 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 21 Apr 2022 02:46:45 GMT
ENV PHP_VERSION=7.4.29
# Thu, 21 Apr 2022 02:46:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Thu, 21 Apr 2022 02:46:48 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Thu, 21 Apr 2022 02:47:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Apr 2022 02:47:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Apr 2022 02:51:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Apr 2022 02:51:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 21 Apr 2022 02:51:29 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Apr 2022 02:51:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Apr 2022 02:51:32 GMT
STOPSIGNAL SIGWINCH
# Thu, 21 Apr 2022 02:51:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 21 Apr 2022 02:51:35 GMT
WORKDIR /var/www/html
# Thu, 21 Apr 2022 02:51:37 GMT
EXPOSE 80
# Thu, 21 Apr 2022 02:51:39 GMT
CMD ["apache2-foreground"]
# Fri, 22 Apr 2022 00:03:10 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Fri, 22 Apr 2022 00:03:12 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 22 Apr 2022 00:03:22 GMT
RUN a2enmod rewrite
# Fri, 22 Apr 2022 00:07:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 00:07:44 GMT
VOLUME [/var/www/html]
# Fri, 22 Apr 2022 00:07:47 GMT
ENV JOOMLA_VERSION=4.1.2
# Fri, 22 Apr 2022 00:07:50 GMT
ENV JOOMLA_SHA512=ae1cc556ef56415875a0c8aa4deb814acdc3efcc661bee32db4fd4b6017b800ae135d78e800226eaba11b687230b1ff6ed1793a64dda6da46907b163c5f2a666
# Fri, 22 Apr 2022 00:08:17 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 22 Apr 2022 00:08:25 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Fri, 22 Apr 2022 00:08:30 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 22 Apr 2022 00:08:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Apr 2022 00:08:40 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5e0d035960b14409a1ddb839de80aa08677b71addd5e94264ff9ee89a2523e5b`  
		Last Modified: Wed, 20 Apr 2022 09:56:59 GMT  
		Size: 35.3 MB (35285249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b3f143029a650945718f049f94d7fe10ce0282766d2ebfcf8287da753d20e1`  
		Last Modified: Thu, 21 Apr 2022 03:28:03 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b96b8b4cf170474b37586f15f5b7e9c2281d256e2284358baf9435ef970ab7f`  
		Last Modified: Thu, 21 Apr 2022 03:28:18 GMT  
		Size: 86.6 MB (86625757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e21cfe9b423c803158576f2d25107d8f04a7e4fdb55b44038e731f061a924ab`  
		Last Modified: Thu, 21 Apr 2022 03:28:00 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47fa6048915eff7cf8611ab2ce357648bdf3815b33ac18eee2e724a58f4df269`  
		Last Modified: Thu, 21 Apr 2022 03:29:33 GMT  
		Size: 20.5 MB (20453984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c791c79030cd731b4589ce6ca3aeccac513a02ef794c97a88bf63242d6226881`  
		Last Modified: Thu, 21 Apr 2022 03:29:30 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bf6968b23adb3f2926819839b0dd43ec594114eeb69952d51dcefc7618680d`  
		Last Modified: Thu, 21 Apr 2022 03:29:28 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2e74ceca61e004855bcb044c3ef8e4e7fbb0ba25c5d3ca45151074e8947d90`  
		Last Modified: Thu, 21 Apr 2022 03:39:00 GMT  
		Size: 10.8 MB (10758832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bcebd59a92906401d126c5435c3ea34b98c2a07c1cf52bb789a4b8f6ee65636`  
		Last Modified: Thu, 21 Apr 2022 03:38:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb7badda385b4741e1562628d9cbe1d0a43f9deceee53f470f8dc7a85395d7c`  
		Last Modified: Thu, 21 Apr 2022 03:38:59 GMT  
		Size: 10.9 MB (10893203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422cadaf79e6e1cafff58769ec812af8852f3e5e54dc7329988ec563c9848da5`  
		Last Modified: Thu, 21 Apr 2022 03:38:56 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5f6d9d4daf5f639e99bbbe2d06952fd7f1d3e1361d12a404cfa3c364c05326`  
		Last Modified: Thu, 21 Apr 2022 03:38:56 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7bed98d9903086019c35689a6826634c7ffed6c7dedcbd8e82d7e04c74b3b1`  
		Last Modified: Thu, 21 Apr 2022 03:38:56 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fc20e5755d7a12b32dafbc36c8a3628e218e1d765b6d770edca75e09ee58fe`  
		Last Modified: Fri, 22 Apr 2022 00:40:11 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108d959b127af870184b189b57a4892915692c429546b9ff5b7bcd3fffb84e9c`  
		Last Modified: Fri, 22 Apr 2022 00:40:12 GMT  
		Size: 3.3 MB (3315871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84da1d68905ccde44b44a338609e74b8b3b18ee8d06a1c1265c6db415c0669a9`  
		Last Modified: Fri, 22 Apr 2022 00:40:16 GMT  
		Size: 22.3 MB (22344652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d25ee61ab233e886570811a5ad64e77a2874a29c3b61092fcee975d57d14bc0`  
		Last Modified: Fri, 22 Apr 2022 00:40:11 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8adf7dab5771edb5d8f1c92d0f5f6a925a9f012ce2a839892228090d708bc052`  
		Last Modified: Fri, 22 Apr 2022 00:40:13 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-apache` - linux; s390x

```console
$ docker pull joomla@sha256:adf4cbd89da8a394e23fe847611a29d5883626d53f29dfbfc33d1914e789a71f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.9 MB (165946062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:339e4ab4b8dcc4a9b73fcfa6ab3ed1fc1d5850c6e5f33bb2b06d5848b209beb3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:44:17 GMT
ADD file:d93a1cf64a813d01774cd628dfd683c006e20159e2ab3464c2159c8d9897c725 in / 
# Wed, 11 May 2022 00:44:19 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:00:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 09:00:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 09:00:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:00:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 09:00:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 09:03:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 09:03:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 09:03:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 09:03:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 09:03:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 09:03:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:03:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:03:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 10:26:50 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 11 May 2022 10:26:51 GMT
ENV PHP_VERSION=7.4.29
# Wed, 11 May 2022 10:26:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 11 May 2022 10:26:51 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 11 May 2022 10:26:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 10:27:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 10:28:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 10:28:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 May 2022 10:28:46 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 10:28:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 10:28:47 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 May 2022 10:28:47 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 May 2022 10:28:47 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 10:28:47 GMT
EXPOSE 80
# Wed, 11 May 2022 10:28:47 GMT
CMD ["apache2-foreground"]
# Wed, 11 May 2022 18:38:57 GMT
LABEL maintainer=Llewellyn van der Merwe <llewellyn.van-der-merwe@community.joomla.org> (@Llewellynvdm), Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 11 May 2022 18:38:57 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 11 May 2022 18:38:58 GMT
RUN a2enmod rewrite
# Wed, 11 May 2022 18:40:17 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libicu-dev 		libjpeg-dev 		libldap2-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		intl 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install memcached-3.2.0; 	pecl install redis-5.3.7; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 18:40:18 GMT
VOLUME [/var/www/html]
# Wed, 11 May 2022 21:41:49 GMT
ENV JOOMLA_VERSION=4.1.3
# Wed, 11 May 2022 21:41:49 GMT
ENV JOOMLA_SHA512=7937355529688adffe2d470bd49da89cddef1b10eca6e3ef20acfd2ebfb695fa3fa346352a68bc094787dd48fe9a2d06371038ce8894cf5ebb0197b3b6140bef
# Wed, 11 May 2022 21:42:08 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Wed, 11 May 2022 21:42:15 GMT
COPY file:0606560d4086c1b747df5afb8b84de5e317d50368eb37b8af3407cb091e8cae8 in /entrypoint.sh 
# Wed, 11 May 2022 21:42:15 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Wed, 11 May 2022 21:42:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 11 May 2022 21:42:17 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9f3750f6094217808e26d471752341db88153c8d5b5f9bb11577b74671303bbc`  
		Last Modified: Wed, 11 May 2022 00:50:03 GMT  
		Size: 29.7 MB (29654739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f812b6b58048d2311eb80f0410cb37f884343218ec756d933b109a1a394791dc`  
		Last Modified: Wed, 11 May 2022 10:54:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d24614089fafa2f33fbfb92b70dc612b0203daeed642445bd142cf9cdee9212`  
		Last Modified: Wed, 11 May 2022 10:54:26 GMT  
		Size: 71.6 MB (71621628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eb678bab4e766e631c3f955141e51e923d3288e6ff9c307728a51d28d816c4`  
		Last Modified: Wed, 11 May 2022 10:54:16 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c777adeabf1143bdc6ab9b9dfdd11dc1292c8386fe5569d585e7c29f4a68fcea`  
		Last Modified: Wed, 11 May 2022 10:54:50 GMT  
		Size: 19.1 MB (19054546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e7ad25936861f6891e430256bd3719f6c5ec3da43957e64c08389533ed6d0e`  
		Last Modified: Wed, 11 May 2022 10:54:48 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42e3fdc4bde2ca8f906a25021d3b8e9f60d4ee9d0488c7bfeacce7c34fbef2f`  
		Last Modified: Wed, 11 May 2022 10:54:47 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4202df31103e3b84cb7f49e763f870929da9f747aec37542baa08cc1b22a8363`  
		Last Modified: Wed, 11 May 2022 11:05:06 GMT  
		Size: 10.8 MB (10757666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c9bca52a9da088a36ab87c3744b703d867d411ea02aece5b8a12741f6bf01e`  
		Last Modified: Wed, 11 May 2022 11:05:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b67fa9ad98d0ed44dd9c19536aad44df7a947176dee7ba2f833cab92eeba491`  
		Last Modified: Wed, 11 May 2022 11:05:06 GMT  
		Size: 9.7 MB (9688103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9488e981ee242ef513f051749ee9cf210ed87f92feb3ac2026588e084864df16`  
		Last Modified: Wed, 11 May 2022 11:05:04 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9b6dde6261d2bf1da84d67dfacfebeea9f0d819e4adb78921094b9de615485`  
		Last Modified: Wed, 11 May 2022 11:05:05 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae803f2dc644af1e81741b591f87ab27173ec6b59cdcd6a7b7f31349e365cb94`  
		Last Modified: Wed, 11 May 2022 11:05:04 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0267897fdaac536f4e6eefd93dee641e776ec4edd823857822f8119879370b61`  
		Last Modified: Wed, 11 May 2022 18:54:17 GMT  
		Size: 315.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c716e87119f74da509006bc7918f222a5ddbecd91149a69023865a95b605fb`  
		Last Modified: Wed, 11 May 2022 18:54:17 GMT  
		Size: 3.1 MB (3060512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9313827ff9c144c7baa415d1628556d65620571fd7176567898fe0667ff47c`  
		Last Modified: Wed, 11 May 2022 21:52:47 GMT  
		Size: 22.1 MB (22100538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34b096a6beecbaad7ee28edee1ac4985f32cbebdd5b56948495c6b8dd565d45`  
		Last Modified: Wed, 11 May 2022 21:52:44 GMT  
		Size: 1.8 KB (1827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9b1ad4002073a9bf45e0e12447b7cc11d232af2d5197ed96667ae474c3e4cf`  
		Last Modified: Wed, 11 May 2022 21:52:44 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
