## `joomla:php7.4`

```console
$ docker pull joomla@sha256:42e2a6d2e8dadccda582fdb85adabf4e63264c6b9756e8cdae51433bbacd42e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `joomla:php7.4` - linux; amd64

```console
$ docker pull joomla@sha256:728049aac7652bcd92865b3b0b52114922c420271a37cdf8c82d73e33f56b7ea
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.2 MB (160151215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f65f0dee7058c814d34a990c4a5ee7b8c56d2c86bdf11414fcae385c2e654e47`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Feb 2021 02:20:55 GMT
ADD file:d5c41bfaf15180481d8606f50799297e3f49b8a258c7c2cd988ab2bf0013272d in / 
# Tue, 09 Feb 2021 02:20:56 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 18:55:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 18:55:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 18:55:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 18:55:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 18:55:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 19:05:05 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Feb 2021 19:05:05 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Feb 2021 19:05:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Feb 2021 19:05:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Feb 2021 19:05:18 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Feb 2021 19:05:18 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Feb 2021 19:05:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Feb 2021 19:05:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 19:05:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 19:05:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 19:37:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 19:37:23 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 19:37:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 19:37:24 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 19:37:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 19:37:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 19:42:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 19:42:21 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 09 Feb 2021 19:42:22 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 19:42:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 19:42:23 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Feb 2021 19:42:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Feb 2021 19:42:23 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 19:42:24 GMT
EXPOSE 80
# Tue, 09 Feb 2021 19:42:24 GMT
CMD ["apache2-foreground"]
# Wed, 10 Feb 2021 10:30:09 GMT
LABEL maintainer=Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 10 Feb 2021 10:30:09 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 10 Feb 2021 10:30:10 GMT
RUN a2enmod rewrite
# Wed, 10 Feb 2021 10:31:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 10 Feb 2021 10:31:40 GMT
VOLUME [/var/www/html]
# Thu, 04 Mar 2021 02:20:26 GMT
ENV JOOMLA_VERSION=3.9.25
# Thu, 04 Mar 2021 02:20:27 GMT
ENV JOOMLA_SHA512=83fc90cb09d710e30dc8e8f50c4e6074ab74fb6a431a851b2567e30273e2a27686d9702cc0cdbae7dc2db09efa0081f8418064b691de43fee1af15f7a195fa25
# Thu, 04 Mar 2021 02:20:31 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 04 Mar 2021 02:20:32 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 04 Mar 2021 02:20:32 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 04 Mar 2021 02:20:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 Mar 2021 02:20:32 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:45b42c59be334ecda0daaa139b2f7d310e45c564c5f12263b1b8e68ec9e810ed`  
		Last Modified: Tue, 09 Feb 2021 02:26:39 GMT  
		Size: 27.1 MB (27095142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48991d6909cf720506106468cbe52f0eec8e1c809d7684429ffca6503fcebf1`  
		Last Modified: Tue, 09 Feb 2021 20:43:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935e2abd2c2c402808fff904dbd8a4a40328ef5be78063cae8fa3b780383e266`  
		Last Modified: Tue, 09 Feb 2021 20:43:27 GMT  
		Size: 76.7 MB (76677231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ccf45ccdb967c3157f2b65cb4fd4f821bb329dc5cbb0192423518ab73ceae6`  
		Last Modified: Tue, 09 Feb 2021 20:43:09 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b5ac70765b0ba0da437148053d9bd9d8a80652a3a1368a29e9e13263dceba9`  
		Last Modified: Tue, 09 Feb 2021 20:43:54 GMT  
		Size: 18.7 MB (18678374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5638b69045baa7e8884e7f730a9f8d86b1aabac740267d7bf09aabb9c9dec62b`  
		Last Modified: Tue, 09 Feb 2021 20:43:49 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdaed064166ffd6ba57f62591ec2164b9112834089a51167836cd8352861bf3`  
		Last Modified: Tue, 09 Feb 2021 20:43:48 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e932cec09cedb1f3ec15654a6b4d4194238a3102f073562fc64e728e47b37e7f`  
		Last Modified: Tue, 09 Feb 2021 20:45:16 GMT  
		Size: 10.7 MB (10670402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe190145b1c3b548117b4244ea41e229db54e22073525a49af2200761288d0f`  
		Last Modified: Tue, 09 Feb 2021 20:45:14 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f747612094ef8fb6a36f88b37c72bd35ac5aa129e8ae9e9e6746e829d8fd3a79`  
		Last Modified: Tue, 09 Feb 2021 20:45:17 GMT  
		Size: 13.8 MB (13832137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300f68c220b15f099e6a4985b80e0320a7e7607ad3e70d245fb79aab0e2dd673`  
		Last Modified: Tue, 09 Feb 2021 20:45:14 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd583fc4f80c3fde1444d83dd503f8a8a0442bafbed760a2bbdb0272ac7f977`  
		Last Modified: Tue, 09 Feb 2021 20:45:13 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011e53c9540e645c8f8b8f7120158dd3f9fcb60eb41b1da86797b8834292f205`  
		Last Modified: Tue, 09 Feb 2021 20:45:14 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0477a016e85e07c71779fb0aa8eb9860406e7472bd586d6549d6e68cc5b0fc07`  
		Last Modified: Wed, 10 Feb 2021 10:35:03 GMT  
		Size: 316.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdeff45d51843426a4ca9a8fe109970b56117378ae87402dff6de62b5118480`  
		Last Modified: Wed, 10 Feb 2021 10:35:03 GMT  
		Size: 3.5 MB (3477809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f01ef45cd852b122c256fdfdb900a54f24cc9321e38d12d4283c411b1b2da7f`  
		Last Modified: Thu, 04 Mar 2021 02:22:19 GMT  
		Size: 9.7 MB (9712726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14328cad08e7cfb87f2b59f11644690cf9db60c846aa8c22da5cf25a8b0de68f`  
		Last Modified: Thu, 04 Mar 2021 02:22:16 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef05ec512defb176b20682bf8f1ffa18a89e8078abf5b36d32e59fd521fd45b8`  
		Last Modified: Thu, 04 Mar 2021 02:22:17 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4` - linux; arm variant v5

```console
$ docker pull joomla@sha256:a3b653d88d81b5cd562164f393f2a1461ffdec5db49d9dafe6b54edc413bcba3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138296709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68d1fff89ae7efab67ba63d982794de873738dfa22e018c507379bf2a40f0085`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Feb 2021 02:50:10 GMT
ADD file:fbd00ef7871dc27d7ed5fa8c238cdc80652bd87b8033be7de9e54a799bbf10a4 in / 
# Tue, 09 Feb 2021 02:50:11 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 09:40:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 09:40:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 09:41:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 09:41:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 09:41:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 09:45:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Feb 2021 09:45:52 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Feb 2021 09:46:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Feb 2021 09:46:18 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Feb 2021 09:46:20 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Feb 2021 09:46:21 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Feb 2021 09:46:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Feb 2021 09:46:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 09:46:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 09:46:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 10:02:18 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 10:02:19 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 10:02:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 10:02:20 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 10:02:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 10:02:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 10:05:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 10:05:33 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 09 Feb 2021 10:05:35 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 10:05:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 10:05:36 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Feb 2021 10:05:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Feb 2021 10:05:37 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 10:05:38 GMT
EXPOSE 80
# Tue, 09 Feb 2021 10:05:38 GMT
CMD ["apache2-foreground"]
# Tue, 09 Feb 2021 16:45:46 GMT
LABEL maintainer=Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 09 Feb 2021 16:45:47 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 09 Feb 2021 16:45:49 GMT
RUN a2enmod rewrite
# Tue, 09 Feb 2021 16:48:34 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 16:48:35 GMT
VOLUME [/var/www/html]
# Thu, 04 Mar 2021 02:49:46 GMT
ENV JOOMLA_VERSION=3.9.25
# Thu, 04 Mar 2021 02:49:48 GMT
ENV JOOMLA_SHA512=83fc90cb09d710e30dc8e8f50c4e6074ab74fb6a431a851b2567e30273e2a27686d9702cc0cdbae7dc2db09efa0081f8418064b691de43fee1af15f7a195fa25
# Thu, 04 Mar 2021 02:50:02 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 04 Mar 2021 02:50:04 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 04 Mar 2021 02:50:05 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 04 Mar 2021 02:50:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 Mar 2021 02:50:08 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8e683fcc73f4da7d69ce1d5f4e1d77510aa459490068f38db2d8663698b391a0`  
		Last Modified: Tue, 09 Feb 2021 02:59:07 GMT  
		Size: 24.8 MB (24839297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479d20320ef94e865807f24ef2b2ed4435c3b8f9a45286e13b963422bb31030e`  
		Last Modified: Tue, 09 Feb 2021 10:48:55 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f378ecd0ed69d12360ccc0800e83b3d3d66ca888dacb74bb21b13599b0c51903`  
		Last Modified: Tue, 09 Feb 2021 10:49:14 GMT  
		Size: 58.8 MB (58814766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fba887c8789cfa67533944f9e7d2e966cf5d283331b7a74d9c4a4ba2b0fe83`  
		Last Modified: Tue, 09 Feb 2021 10:48:55 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24250d2772eb056e6c3c1c8e3fd2d365d0253ed0ea589a22108c0daa243edc03`  
		Last Modified: Tue, 09 Feb 2021 10:49:47 GMT  
		Size: 18.0 MB (18026256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fbeb13befaccae1c25574d64fd63ec33c6ae0aea76ad6050272748257c11c53`  
		Last Modified: Tue, 09 Feb 2021 10:49:42 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a6e6366d4ef0a148501b6adfaa5a812d48aabc304090a81e9e750c27384179`  
		Last Modified: Tue, 09 Feb 2021 10:49:42 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a80599d5bdeda2dc3222d24d9c575e0f622a83e0ff5694a8cd3258ebc83a8c`  
		Last Modified: Tue, 09 Feb 2021 10:51:28 GMT  
		Size: 10.7 MB (10668608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e685868644d7d029423a245355186f0583cabcc64fa4b922d4c432228993a6`  
		Last Modified: Tue, 09 Feb 2021 10:51:26 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ff04d5cbab967f2a68087e6acec26a1b1125593a1be50e31e624d32aea70fc`  
		Last Modified: Tue, 09 Feb 2021 10:51:30 GMT  
		Size: 12.9 MB (12919185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5c6d2206fdc81a8305de871f7db5766fdf73c93545cfb9483411ab0246dd3c`  
		Last Modified: Tue, 09 Feb 2021 10:51:25 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1784eca452a5ddda5489854c16644144bca80b611ab407d61cdfdce15ba7ccef`  
		Last Modified: Tue, 09 Feb 2021 10:51:26 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624a4eea2db5fe273c5e8b656e5f2e58453fc148c8b2aa4883fcdf0d68a933c1`  
		Last Modified: Tue, 09 Feb 2021 10:51:25 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c0a83f7e9fbdcc31a094afedebc51ec9bdff59c20acd7808af004e00833281`  
		Last Modified: Tue, 09 Feb 2021 16:54:08 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3255f8b9a166a11bc3ff1cdce18ec61fd23acdc1903f915a165bfc663d1306b0`  
		Last Modified: Tue, 09 Feb 2021 16:54:09 GMT  
		Size: 3.3 MB (3308273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5b83975b0b8d4d56afd02021ba106eeaa9acdabb79ed2c46dcf8bd74cfab0a`  
		Last Modified: Thu, 04 Mar 2021 02:52:18 GMT  
		Size: 9.7 MB (9712803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6e7cca257afdc0080c06a79e7295a865a65fe19c517b46c773a3dec16f5445`  
		Last Modified: Thu, 04 Mar 2021 02:52:13 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0a711e5d70d4641c0749b434b1a0715718c665a011886139f2333e29f1b9c2`  
		Last Modified: Thu, 04 Mar 2021 02:52:12 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4` - linux; arm variant v7

```console
$ docker pull joomla@sha256:44457a6bcb935bd68c5866aca2df8a500e8ad8a129dc1a138ec1c9438eb09d7e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135516363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27dfe24fdcb2142ce405c2e8faef99660e6805ed7dac54816e247249659c7aa1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:57 GMT
ADD file:e675d50366bde57173a75f9a29367d765e7da2b7254c5254b64e777cf6870502 in / 
# Tue, 09 Feb 2021 03:01:00 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 11:54:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 11:54:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 11:55:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 11:55:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 11:55:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 11:58:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Feb 2021 11:58:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Feb 2021 11:59:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Feb 2021 11:59:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Feb 2021 11:59:11 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Feb 2021 11:59:13 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Feb 2021 11:59:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Feb 2021 11:59:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 11:59:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 11:59:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 12:13:43 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 12:13:43 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 12:13:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 12:13:45 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 12:14:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 12:14:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 12:16:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 12:16:37 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 09 Feb 2021 12:16:40 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 12:16:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 12:16:42 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Feb 2021 12:16:43 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Feb 2021 12:16:43 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 12:16:44 GMT
EXPOSE 80
# Tue, 09 Feb 2021 12:16:45 GMT
CMD ["apache2-foreground"]
# Wed, 10 Feb 2021 02:52:38 GMT
LABEL maintainer=Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 10 Feb 2021 02:52:39 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 10 Feb 2021 02:52:42 GMT
RUN a2enmod rewrite
# Wed, 10 Feb 2021 02:55:18 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 10 Feb 2021 02:55:19 GMT
VOLUME [/var/www/html]
# Thu, 04 Mar 2021 03:01:09 GMT
ENV JOOMLA_VERSION=3.9.25
# Thu, 04 Mar 2021 03:01:09 GMT
ENV JOOMLA_SHA512=83fc90cb09d710e30dc8e8f50c4e6074ab74fb6a431a851b2567e30273e2a27686d9702cc0cdbae7dc2db09efa0081f8418064b691de43fee1af15f7a195fa25
# Thu, 04 Mar 2021 03:01:25 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 04 Mar 2021 03:01:28 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 04 Mar 2021 03:01:29 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 04 Mar 2021 03:01:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 Mar 2021 03:01:30 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:db574d82360c3b60abadbef4f3daf8dee01f24741fc6ab3692aa543558d8b624`  
		Last Modified: Tue, 09 Feb 2021 03:09:46 GMT  
		Size: 22.7 MB (22703384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4e7c5500d514905861de5fd68ba2321eb5866e64f8b6689c3ea8129a68b4a2`  
		Last Modified: Tue, 09 Feb 2021 13:00:44 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30745314a6fe3cad64125db918cc09eadf8b13a570ca225f34f3e36e9fb6110`  
		Last Modified: Tue, 09 Feb 2021 13:01:01 GMT  
		Size: 59.5 MB (59513280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0061ef8da45b5a1732d5c93658be4ee8d9088db791f661832ceabe441b54544b`  
		Last Modified: Tue, 09 Feb 2021 13:00:44 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226dc87e52cfe2aa84256e6c7b9d91fd5b7141333352d9d6fb8741e15918d65d`  
		Last Modified: Tue, 09 Feb 2021 13:01:34 GMT  
		Size: 17.5 MB (17481726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b759469265947391c3878a45262001e6d3e2ed0dd26c43d1804cbca8d9dfb04`  
		Last Modified: Tue, 09 Feb 2021 13:01:29 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7cd574b5f7f1b94cabe3a9ad3dc6928da8f35126b1e3cbce55a02e8ed7e8dd`  
		Last Modified: Tue, 09 Feb 2021 13:01:29 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56893060319f8e1242de64474c1a6f72dc1e77faf5e04cf2d34cdca0ec508e5`  
		Last Modified: Tue, 09 Feb 2021 13:03:25 GMT  
		Size: 10.7 MB (10668627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e630469897caaef2812e94d6ccbbe45f5a67d2afe84fd053c3cb81a80b21366c`  
		Last Modified: Tue, 09 Feb 2021 13:03:22 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43fe4400f99060865152637b305bf318ba1b75d5197968f73c48df486359f4f`  
		Last Modified: Tue, 09 Feb 2021 13:03:26 GMT  
		Size: 12.2 MB (12213098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e463c3140f3a68687a892afc3935375353e4824f45ce9434afb585a490fe25b`  
		Last Modified: Tue, 09 Feb 2021 13:03:22 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601892f37b2111185beec53734dc72ea41e5702531b015dd35e051d32a8d962c`  
		Last Modified: Tue, 09 Feb 2021 13:03:22 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:989b27926beaff01e5349ce568aecc6ce89e35686995183a99853e4d8d3300b9`  
		Last Modified: Tue, 09 Feb 2021 13:03:22 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e67edc5caa3defb3dc966ef28523778798ea87a19e14b9c400ac2aa9dc131b9`  
		Last Modified: Wed, 10 Feb 2021 03:00:52 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbf45f7216fb12df577e075fda24c2e753724ecf8b568b891dcd558a0d44b4c`  
		Last Modified: Wed, 10 Feb 2021 03:00:54 GMT  
		Size: 3.2 MB (3215941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05564b05060826657ce6838555a420aeedff8b677009d91229d9558b91e008e`  
		Last Modified: Thu, 04 Mar 2021 03:04:49 GMT  
		Size: 9.7 MB (9712795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1788a8e6a1327dc558f953ef2a71f2befb3a49e0c28d6846ae5bc18001093cb7`  
		Last Modified: Thu, 04 Mar 2021 03:04:44 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cb6fc4e24ba4da36493da172e8e38cb3344477b47bf3435e21de06273ed6e1`  
		Last Modified: Thu, 04 Mar 2021 03:04:43 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:c488293f7ab564c7e9c0f8eed3a910fc4bfc2947d71adecfb91e4c69aa092823
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.2 MB (152217359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f6b3f84c37ef03b1f27aa1466fcaa5266fd738e68315fffbe57ec00ec90d9ab`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Feb 2021 02:41:10 GMT
ADD file:d906dedaf14d8e3874b46787f7a1dbf268bc124c4e1dd32f13f3079e12f22238 in / 
# Tue, 09 Feb 2021 02:41:13 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 13:24:06 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 13:24:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 13:24:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 13:24:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 13:24:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 13:29:29 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Feb 2021 13:29:30 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Feb 2021 13:29:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Feb 2021 13:29:49 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Feb 2021 13:29:51 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Feb 2021 13:29:52 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Feb 2021 13:29:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Feb 2021 13:29:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 13:29:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 13:29:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 13:46:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 13:46:10 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 13:46:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 13:46:14 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 13:46:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 13:46:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 13:49:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 13:49:20 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 09 Feb 2021 13:49:23 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 13:49:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 13:49:25 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Feb 2021 13:49:26 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Feb 2021 13:49:27 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 13:49:29 GMT
EXPOSE 80
# Tue, 09 Feb 2021 13:49:31 GMT
CMD ["apache2-foreground"]
# Wed, 10 Feb 2021 05:18:30 GMT
LABEL maintainer=Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 10 Feb 2021 05:18:30 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 10 Feb 2021 05:18:32 GMT
RUN a2enmod rewrite
# Wed, 10 Feb 2021 05:20:56 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 10 Feb 2021 05:20:57 GMT
VOLUME [/var/www/html]
# Thu, 04 Mar 2021 02:40:53 GMT
ENV JOOMLA_VERSION=3.9.25
# Thu, 04 Mar 2021 02:40:54 GMT
ENV JOOMLA_SHA512=83fc90cb09d710e30dc8e8f50c4e6074ab74fb6a431a851b2567e30273e2a27686d9702cc0cdbae7dc2db09efa0081f8418064b691de43fee1af15f7a195fa25
# Thu, 04 Mar 2021 02:41:02 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 04 Mar 2021 02:41:04 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 04 Mar 2021 02:41:05 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 04 Mar 2021 02:41:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 Mar 2021 02:41:06 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:83c5cfdaa5385ea6fc4d31e724fd4dc5d74de847a7bdd968555b8f2c558dac0e`  
		Last Modified: Tue, 09 Feb 2021 02:47:27 GMT  
		Size: 25.9 MB (25851449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7445693bd43e8246a8c166233392b33143f7f5e396c480f74538e5738fb6bd6e`  
		Last Modified: Tue, 09 Feb 2021 14:35:20 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb0363d084b9a838de3a1ef92a69c34131d0be020cc0474098ea80a07e16b6d`  
		Last Modified: Tue, 09 Feb 2021 14:35:38 GMT  
		Size: 70.4 MB (70355003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87c2495950546c2e82fc496d7c39837a517f3f3095fb87598d1731d0529f907`  
		Last Modified: Tue, 09 Feb 2021 14:35:20 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1c5d697df1ad5b06b1191622869ff679a88a60b478a1d7f2dc94b38c249efa`  
		Last Modified: Tue, 09 Feb 2021 14:36:30 GMT  
		Size: 18.6 MB (18579948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361e2a373dc16cf325162b9be8d28ae695eaddb93f477dbad81713d17c4eb823`  
		Last Modified: Tue, 09 Feb 2021 14:36:15 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df605982341375d14e7a1c2767d248fe8e85a467ac502562d36f73b352f654e9`  
		Last Modified: Tue, 09 Feb 2021 14:36:15 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282e62e4b1359ca753d92fec39694a2a08e69de2aa7248450167150e43f33f01`  
		Last Modified: Tue, 09 Feb 2021 14:38:18 GMT  
		Size: 10.7 MB (10669291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbec33b64b9ffea1c2898793fa8352db3a53c3934f193f255d149ef1c726ed8`  
		Last Modified: Tue, 09 Feb 2021 14:38:16 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7643dc96f9971d79c7a4948d938008c5ace5ca68ca372f321508950d4500711`  
		Last Modified: Tue, 09 Feb 2021 14:38:20 GMT  
		Size: 13.6 MB (13610678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113254d1e77acb1ced4e82ccde2e3f41506bf27a1f80fce35212c5f4b5a1133b`  
		Last Modified: Tue, 09 Feb 2021 14:38:16 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6b49bef0eb0129716605e6ce6a2dca5dc82a91adef36536612091fd5233379`  
		Last Modified: Tue, 09 Feb 2021 14:38:16 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572473fc3433ce7d8ef286f74425711cce7cd1992dc04910b3a65fe5e10c491`  
		Last Modified: Tue, 09 Feb 2021 14:38:16 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe8cfa92acd043f9d38b4c597424bc544524a6ba48dc35cab4b296455ce1b5c`  
		Last Modified: Wed, 10 Feb 2021 05:25:55 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6cd20def262447451b02167aa4626acfed0849e4fd22647b77a5d817a2e1da2`  
		Last Modified: Wed, 10 Feb 2021 05:25:56 GMT  
		Size: 3.4 MB (3430677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497af90e360702dfb16d12ddf83bf888610320bcd6cfa6296f8bf2249b61c01`  
		Last Modified: Thu, 04 Mar 2021 02:43:52 GMT  
		Size: 9.7 MB (9712802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61aedb98608e4d4521e63cead1ec8a678a27680cb2b69c9d7455936e1cb2bf73`  
		Last Modified: Thu, 04 Mar 2021 02:43:49 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4f48197dbad17244d63ba45c19271532b35427ff22f0133fa650295047f9be`  
		Last Modified: Thu, 04 Mar 2021 02:43:50 GMT  
		Size: 612.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4` - linux; 386

```console
$ docker pull joomla@sha256:4abfc1c42d751d797373db8d4c64746e108037e775cb389f412c72c9280fbfc0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166130162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc2bcf4f77dd418bf0ed01f541febc7fe983087cbfa6ae526cea4d7c36d5a363`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Feb 2021 02:39:47 GMT
ADD file:61c31b1037672781ed0ecbc080ee3d49c83af49f5578b011544513fa9625698d in / 
# Tue, 09 Feb 2021 02:39:47 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 12:55:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 12:55:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 12:55:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 12:55:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 12:55:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 13:04:35 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Feb 2021 13:04:35 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Feb 2021 13:04:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Feb 2021 13:04:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Feb 2021 13:04:54 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Feb 2021 13:04:54 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Feb 2021 13:04:54 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Feb 2021 13:04:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 13:04:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 13:04:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 13:37:28 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 13:37:28 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 13:37:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 13:37:29 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 13:37:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 13:37:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 13:42:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 13:42:33 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 09 Feb 2021 13:42:34 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 13:42:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 13:42:34 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Feb 2021 13:42:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Feb 2021 13:42:34 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 13:42:35 GMT
EXPOSE 80
# Tue, 09 Feb 2021 13:42:35 GMT
CMD ["apache2-foreground"]
# Tue, 09 Feb 2021 21:35:26 GMT
LABEL maintainer=Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 09 Feb 2021 21:35:26 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 09 Feb 2021 21:35:30 GMT
RUN a2enmod rewrite
# Tue, 09 Feb 2021 21:37:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 21:37:24 GMT
VOLUME [/var/www/html]
# Thu, 04 Mar 2021 02:42:08 GMT
ENV JOOMLA_VERSION=3.9.25
# Thu, 04 Mar 2021 02:42:08 GMT
ENV JOOMLA_SHA512=83fc90cb09d710e30dc8e8f50c4e6074ab74fb6a431a851b2567e30273e2a27686d9702cc0cdbae7dc2db09efa0081f8418064b691de43fee1af15f7a195fa25
# Thu, 04 Mar 2021 02:42:13 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 04 Mar 2021 02:42:14 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 04 Mar 2021 02:42:14 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 04 Mar 2021 02:42:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 Mar 2021 02:42:14 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:27cbb00346a16ea900c1049a2e5b47942c586c377179e098382c8ca1c8e87966`  
		Last Modified: Tue, 09 Feb 2021 02:45:51 GMT  
		Size: 27.8 MB (27752731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e273ebd73efe18fbe0a9fb3fa3727a6f72bd5edef4eec32f0cdfd91723b6c877`  
		Last Modified: Tue, 09 Feb 2021 15:05:40 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07347a055a7dbbfecfcbf26edf69115228d399f8c70e5ce9fe2575ac94c9b0c`  
		Last Modified: Tue, 09 Feb 2021 15:06:30 GMT  
		Size: 81.2 MB (81216990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71658904aa5572b07669df7ce20edd1cdbad61f48cd009aff53e9dd64cc748b3`  
		Last Modified: Tue, 09 Feb 2021 15:05:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dccafaa5063e93f83f919bc8f6161244d6508266d216744e6829243dd507ede`  
		Last Modified: Tue, 09 Feb 2021 15:06:57 GMT  
		Size: 19.1 MB (19113687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9c76baf959785aaa0a744ad8d17d6692364ca9e4a891c48250de6eeca08d61`  
		Last Modified: Tue, 09 Feb 2021 15:06:49 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86fe53cd56aa76bf4a093d5adad30627fc1794ff921c6a089787c37866f9001`  
		Last Modified: Tue, 09 Feb 2021 15:06:49 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5985c33a32dc94e828ce31c5807e5db9cf9aa04e1154d4ee554f81b44b8d3ed`  
		Last Modified: Tue, 09 Feb 2021 15:09:06 GMT  
		Size: 10.7 MB (10669758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866cd2248799604e549bad6c8ad535943248142ff55668681088948fba815b74`  
		Last Modified: Tue, 09 Feb 2021 15:09:02 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69027d977749c6e3fdd47447c116731f2de1a6563ee96fd8532d5d9e1d85b98`  
		Last Modified: Tue, 09 Feb 2021 15:09:10 GMT  
		Size: 14.2 MB (14167002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0596ac9c8182bb6fc207dac8da9af60472b126211a400b9c26602574bccb44f`  
		Last Modified: Tue, 09 Feb 2021 15:09:02 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f314bb5294d4340799e9023297a80dea3b59e3a72597fba317a5af48a3797a7f`  
		Last Modified: Tue, 09 Feb 2021 15:09:02 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62234f9ff20856627afd2c02b9a54a37f5daa9331c193cf16048c38ed8277bd`  
		Last Modified: Tue, 09 Feb 2021 15:09:02 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69daa3e0b7a80c63914378f64793f83805b1da46a7fe81919c9b3d75fe722ee2`  
		Last Modified: Tue, 09 Feb 2021 21:41:41 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10798175d541a57a38d05e798e4755bac804812a88767d0c6d2d72fdfa1adaf3`  
		Last Modified: Tue, 09 Feb 2021 21:41:43 GMT  
		Size: 3.5 MB (3489879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d12ed306379e8cd8ff419d9720aa1500b40f08f755d6d5a74b6b0f8af29a69`  
		Last Modified: Thu, 04 Mar 2021 02:43:22 GMT  
		Size: 9.7 MB (9712727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac201bd480d022decb3176359f465af0393c9b91781bdb96f85a002ab38a231e`  
		Last Modified: Thu, 04 Mar 2021 02:43:18 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b1059b908d7cd7e9571244b2d6abbdc2839742521791c6c9c1af749836b38c`  
		Last Modified: Thu, 04 Mar 2021 02:43:18 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4` - linux; mips64le

```console
$ docker pull joomla@sha256:fb79e3aeb8b2f306a499d74b2648bd1c5b282e0d96fba0d173ea1569fe511986
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.7 MB (142728786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98978900500bbdb2532fa296555f63ff81589602093a7e3ad2b5f1113dfe96f4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Feb 2021 03:09:26 GMT
ADD file:0222a151f4e5033d9eae98ce2b703a63f52d049dd72ac40bdd0dc2dafe619f0a in / 
# Tue, 09 Feb 2021 03:09:27 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:38:23 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 04:38:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 04:39:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:39:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 04:39:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 04:52:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Feb 2021 04:52:07 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Feb 2021 04:52:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Feb 2021 04:52:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Feb 2021 04:52:37 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Feb 2021 04:52:37 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Feb 2021 04:52:37 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Feb 2021 04:52:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 04:52:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 04:52:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 05:40:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 05:40:21 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 05:40:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 05:40:22 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 05:40:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 05:40:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 05:48:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 05:48:31 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 09 Feb 2021 05:48:33 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 05:48:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 05:48:33 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Feb 2021 05:48:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Feb 2021 05:48:34 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 05:48:34 GMT
EXPOSE 80
# Tue, 09 Feb 2021 05:48:35 GMT
CMD ["apache2-foreground"]
# Tue, 09 Feb 2021 18:47:06 GMT
LABEL maintainer=Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 09 Feb 2021 18:47:06 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 09 Feb 2021 18:47:08 GMT
RUN a2enmod rewrite
# Tue, 09 Feb 2021 18:51:56 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 18:51:57 GMT
VOLUME [/var/www/html]
# Thu, 04 Mar 2021 02:08:08 GMT
ENV JOOMLA_VERSION=3.9.25
# Thu, 04 Mar 2021 02:08:08 GMT
ENV JOOMLA_SHA512=83fc90cb09d710e30dc8e8f50c4e6074ab74fb6a431a851b2567e30273e2a27686d9702cc0cdbae7dc2db09efa0081f8418064b691de43fee1af15f7a195fa25
# Thu, 04 Mar 2021 02:08:21 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 04 Mar 2021 02:08:23 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 04 Mar 2021 02:08:23 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 04 Mar 2021 02:08:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 Mar 2021 02:08:24 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:dfb81134097d874e01b495d1fba82e384056d0a3a45f01a69a2e86ae82af1e96`  
		Last Modified: Tue, 09 Feb 2021 03:15:55 GMT  
		Size: 25.8 MB (25764640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ea2980e9d1424f17765223b637d6e3f527c0ab3e3b3c293e4ab6d46df86bb6`  
		Last Modified: Tue, 09 Feb 2021 07:01:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04fd49341687ab8ff8e018c1339c00f4b14d980dcff74a90982425c92fb4d468`  
		Last Modified: Tue, 09 Feb 2021 07:02:38 GMT  
		Size: 61.4 MB (61402881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6385772c6452fb0c29341d9195703f25fc85945134be55c6dfe8b39f7825c9cf`  
		Last Modified: Tue, 09 Feb 2021 07:01:48 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622135c380b7e1c06242732be8917d872646053d815a5519070528d722fb33f0`  
		Last Modified: Tue, 09 Feb 2021 07:03:49 GMT  
		Size: 18.6 MB (18611659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc4bbff0885d0ebb94156291ec625b0730ad351928cb8d4fd0056a84ab39066`  
		Last Modified: Tue, 09 Feb 2021 07:03:35 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c7ea375acdfbe784ce7f0076182b2b0c8f1df7b669987f47c8d7b15ddf3f4e`  
		Last Modified: Tue, 09 Feb 2021 07:03:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6685ae441dbc95b51b5e17f21388746de1a6489dca0c8600e1ef423f3da3318`  
		Last Modified: Tue, 09 Feb 2021 07:07:05 GMT  
		Size: 10.7 MB (10667801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c2d7b1d0b8b535248b513283e0f3a6e63c3ae0d5ea5dc74c60b1c46d62d4d4`  
		Last Modified: Tue, 09 Feb 2021 07:06:59 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a38a3421c5be441a0b463dc4460b5df41efe9d139be0aefaeef8dcaa1f0ed37`  
		Last Modified: Tue, 09 Feb 2021 07:07:11 GMT  
		Size: 13.1 MB (13143491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10d1bb6682016ff08f4c56de2d0fbf7b95da977a43e136b840320b939452e98`  
		Last Modified: Tue, 09 Feb 2021 07:07:00 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed8d99dbb90af8a230447d68b454d6f77ff720784d3a5ff83c18ae476b6aee7`  
		Last Modified: Tue, 09 Feb 2021 07:06:59 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b8c398f58cbcaa581cc01b8ee1292389485dcfb9c6b5e77bd7af12c4692a86`  
		Last Modified: Tue, 09 Feb 2021 07:06:59 GMT  
		Size: 889.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc5295e920831fc3d5ccab545d03889dba3d175183c7bb1fb56c1ef09e3570a`  
		Last Modified: Tue, 09 Feb 2021 18:59:53 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b50bfb581f28af09aad37591b134381bbe14653f9385db3bf9ec9fe65f54459`  
		Last Modified: Tue, 09 Feb 2021 18:59:57 GMT  
		Size: 3.4 MB (3418182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8540da7426a822984f8debbc01b95df0f215cc9dd4081f7ddbb05d37036d97cd`  
		Last Modified: Thu, 04 Mar 2021 02:11:28 GMT  
		Size: 9.7 MB (9712731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b4d13e789d85bb7dedbe9308739a2062cbcebdcf87f0e80dc31910c8b2784f`  
		Last Modified: Thu, 04 Mar 2021 02:11:18 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fab727e19e089dcc96dec00158eaf989917e0d40ec277ebee07ca0d45b8395`  
		Last Modified: Thu, 04 Mar 2021 02:11:18 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4` - linux; ppc64le

```console
$ docker pull joomla@sha256:432402c1a27995d94baae9dc977111d68cf3ec022136a5fbb2870b6fcbad2079
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.6 MB (171571428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e03850a0133e25a833a90c49035cf73ee538b330b005da66f561700351d6fa0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Feb 2021 02:19:19 GMT
ADD file:9a8cfdf0eab394a693b5cde0700ad47b6e8506ef0b79fabb8a07874b96e6c394 in / 
# Tue, 09 Feb 2021 02:19:34 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 15:49:06 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 15:49:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 15:54:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 15:54:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 15:54:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 16:05:12 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Feb 2021 16:05:15 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Feb 2021 16:07:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Feb 2021 16:07:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Feb 2021 16:07:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Feb 2021 16:08:02 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Feb 2021 16:08:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Feb 2021 16:08:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 16:08:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 16:08:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 16:40:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 16:40:16 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 16:40:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 16:40:29 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 16:42:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 16:42:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 16:50:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 16:50:14 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 09 Feb 2021 16:50:33 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 16:50:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 16:50:41 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Feb 2021 16:50:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Feb 2021 16:50:51 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 16:50:57 GMT
EXPOSE 80
# Tue, 09 Feb 2021 16:51:03 GMT
CMD ["apache2-foreground"]
# Wed, 10 Feb 2021 10:22:05 GMT
LABEL maintainer=Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Wed, 10 Feb 2021 10:22:17 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Wed, 10 Feb 2021 10:22:40 GMT
RUN a2enmod rewrite
# Wed, 10 Feb 2021 10:27:53 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 10 Feb 2021 10:28:02 GMT
VOLUME [/var/www/html]
# Thu, 04 Mar 2021 02:24:03 GMT
ENV JOOMLA_VERSION=3.9.25
# Thu, 04 Mar 2021 02:24:08 GMT
ENV JOOMLA_SHA512=83fc90cb09d710e30dc8e8f50c4e6074ab74fb6a431a851b2567e30273e2a27686d9702cc0cdbae7dc2db09efa0081f8418064b691de43fee1af15f7a195fa25
# Thu, 04 Mar 2021 02:24:32 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 04 Mar 2021 02:24:41 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 04 Mar 2021 02:24:46 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 04 Mar 2021 02:24:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 Mar 2021 02:25:07 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9996b4fb6bc1c50f95ba30f8988c9c89526556fa320d3fda59d3d8359f7810d6`  
		Last Modified: Tue, 09 Feb 2021 02:27:59 GMT  
		Size: 30.5 MB (30519509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08ed6cfbd4e7b8f4f2d892c01b1976ced072938787d146fc0a55690e9883a74`  
		Last Modified: Tue, 09 Feb 2021 17:52:52 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cc4083d6613c902035d3b0dd1bb317f5bb699313bcd6e687ec17347192cdaa`  
		Last Modified: Tue, 09 Feb 2021 17:53:19 GMT  
		Size: 82.3 MB (82290490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d61a25f1b4f9da6f8c429b980f08dd7c19f7c6353704da136afc7e59343620`  
		Last Modified: Tue, 09 Feb 2021 17:52:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b1f6476e9275a2b18cd7fd1272d6dda57c23b2553c61e8498701ec7e37a54d`  
		Last Modified: Tue, 09 Feb 2021 17:54:20 GMT  
		Size: 19.8 MB (19818441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b84cb0491f75c5f31ddeb649efdc5c1b5105987ed26041d96b7415b17384dd`  
		Last Modified: Tue, 09 Feb 2021 17:54:15 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139cd3ca812b53dbae139a43e087189c11bfcbb27f2dba64e6defc1d5dd151ee`  
		Last Modified: Tue, 09 Feb 2021 17:54:15 GMT  
		Size: 521.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef658a6dbbe181080de3290985ed470a35894b2f4acace6a047faf6d3d269e0c`  
		Last Modified: Tue, 09 Feb 2021 17:57:19 GMT  
		Size: 10.7 MB (10670688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae104ab3d2b4d4f6b7711515a776c9e7b81805c3d806d0c74d4570e275d016c7`  
		Last Modified: Tue, 09 Feb 2021 17:57:14 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13639e6a360fadb166983634bf15b7bd22e89781500a7ecb9bbc5789a681b78`  
		Last Modified: Tue, 09 Feb 2021 17:57:17 GMT  
		Size: 14.9 MB (14874811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d7130823ef1d803c27dfeffbb8eded0d29394e02296342ee9a89e792dd161f`  
		Last Modified: Tue, 09 Feb 2021 17:57:13 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b84889b8e30c3274b9773333eab0d2f35ca74bab373c83673c501e8456dc63`  
		Last Modified: Tue, 09 Feb 2021 17:57:13 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540e1840fb7317308659b7805d240b4ce050179c0fbe22caf5c517579895dc5d`  
		Last Modified: Tue, 09 Feb 2021 17:57:13 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9179b26dca3bfa7d1205b2a9e9c380a908c4e4d4d6824c58d2ef35ff26c5d188`  
		Last Modified: Wed, 10 Feb 2021 10:39:03 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f79ae64958748e46b5c5236b5b26d779cc377d7b872a6fe23aa0305afc680e`  
		Last Modified: Wed, 10 Feb 2021 10:39:03 GMT  
		Size: 3.7 MB (3677163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0881394bc48885f4d6fa5b90535ed95a456b0e9114c5bc7dd9d923140ab6373c`  
		Last Modified: Thu, 04 Mar 2021 02:32:49 GMT  
		Size: 9.7 MB (9712805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38913bc74efc0b8e5d154a9234b7c024842e1fa14fdc3016406b496c4c1769b`  
		Last Modified: Thu, 04 Mar 2021 02:32:46 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fe95bfd014651b31fd1477e8bb94a3c3eacdcba5f1fecc638e93c40dcf294c`  
		Last Modified: Thu, 04 Mar 2021 02:32:46 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4` - linux; s390x

```console
$ docker pull joomla@sha256:fbf35213d0bceca6a1841d528f159d70b2414582c0bea478a16ef654bec27965
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.8 MB (145812163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f76a3c766a0b6cef31ef5a6385df00327ab033b7843ef941467ab53d4fa6742`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 09 Feb 2021 02:42:10 GMT
ADD file:0edb2de05df54191a141bd125f59d7e14eef0cc4576927a247b8dd7d6f255d04 in / 
# Tue, 09 Feb 2021 02:42:12 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 05:49:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 09 Feb 2021 05:49:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 09 Feb 2021 05:49:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 05:49:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Feb 2021 05:49:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Feb 2021 05:52:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 09 Feb 2021 05:52:06 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 09 Feb 2021 05:52:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 09 Feb 2021 05:52:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 09 Feb 2021 05:52:15 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 09 Feb 2021 05:52:15 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 09 Feb 2021 05:52:16 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 09 Feb 2021 05:52:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 05:52:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Feb 2021 05:52:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Feb 2021 06:05:44 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 09 Feb 2021 06:05:44 GMT
ENV PHP_VERSION=7.4.15
# Tue, 09 Feb 2021 06:05:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Tue, 09 Feb 2021 06:05:45 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Tue, 09 Feb 2021 06:05:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 09 Feb 2021 06:05:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:08:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 09 Feb 2021 06:09:00 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:09:01 GMT
RUN docker-php-ext-enable sodium
# Tue, 09 Feb 2021 06:09:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 09 Feb 2021 06:09:02 GMT
STOPSIGNAL SIGWINCH
# Tue, 09 Feb 2021 06:09:02 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 09 Feb 2021 06:09:03 GMT
WORKDIR /var/www/html
# Tue, 09 Feb 2021 06:09:03 GMT
EXPOSE 80
# Tue, 09 Feb 2021 06:09:04 GMT
CMD ["apache2-foreground"]
# Tue, 09 Feb 2021 12:23:18 GMT
LABEL maintainer=Harald Leithner <harald.leithner@community.joomla.org> (@HLeithner)
# Tue, 09 Feb 2021 12:23:18 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Tue, 09 Feb 2021 12:23:19 GMT
RUN a2enmod rewrite
# Tue, 09 Feb 2021 12:24:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libbz2-dev 		libgmp-dev 		libjpeg-dev 		libldap2-dev 		libmcrypt-dev 		libmemcached-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		gmp 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 12:24:28 GMT
VOLUME [/var/www/html]
# Thu, 04 Mar 2021 02:42:18 GMT
ENV JOOMLA_VERSION=3.9.25
# Thu, 04 Mar 2021 02:42:18 GMT
ENV JOOMLA_SHA512=83fc90cb09d710e30dc8e8f50c4e6074ab74fb6a431a851b2567e30273e2a27686d9702cc0cdbae7dc2db09efa0081f8418064b691de43fee1af15f7a195fa25
# Thu, 04 Mar 2021 02:42:26 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 04 Mar 2021 02:42:27 GMT
COPY file:f6b7a1c96cc89593a2b9ce4c68af350ae02f2e0c654cd5e842ff6c03641d470e in /entrypoint.sh 
# Thu, 04 Mar 2021 02:42:28 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 04 Mar 2021 02:42:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 Mar 2021 02:42:28 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:032413a44cf56b097e48b8221bf475ca1bec26e7a27f35fe61d699366a335b79`  
		Last Modified: Tue, 09 Feb 2021 02:45:31 GMT  
		Size: 25.7 MB (25710021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5de5518f7317a13d96a78cb6a69d8a40c528b4f9f5cb8ec38cc29d96e0d3a8`  
		Last Modified: Tue, 09 Feb 2021 06:28:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4631238e5cca78ca96ac7a1e842104ab9c3ebc4b79becc0737d434640363dd04`  
		Last Modified: Tue, 09 Feb 2021 06:29:02 GMT  
		Size: 64.7 MB (64709263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8411cec4a9e17ed0143fe56c907dc88654d788140303c7f805c87d03077642f7`  
		Last Modified: Tue, 09 Feb 2021 06:28:52 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c0653069ff052183ade3fc00c49df68f5c61a45f824621b497dbecbe167d57`  
		Last Modified: Tue, 09 Feb 2021 06:29:31 GMT  
		Size: 18.5 MB (18524892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd3181ee2169b6b7dee05c06019a90ecd69cde9e7aa9f267e73c2020a765533`  
		Last Modified: Tue, 09 Feb 2021 06:29:29 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7c1a1be3b9b8377d35ebe47341808e9121230ea351144eff6fdae3c5978893`  
		Last Modified: Tue, 09 Feb 2021 06:29:28 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946822ee1c0b618e9a3a7a49b289a0543710f98b2dc3ccfc3e749b13eeb274dc`  
		Last Modified: Tue, 09 Feb 2021 06:31:17 GMT  
		Size: 10.7 MB (10668867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d7a7793e11e68ddcb11c610d8eed8040f859e5873a8ccfb13783322e0cdab0`  
		Last Modified: Tue, 09 Feb 2021 06:31:15 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4bf56636d509980efd5021b200a981def56d72016b2b8b71f3017567af00fb`  
		Last Modified: Tue, 09 Feb 2021 06:31:17 GMT  
		Size: 13.0 MB (13047566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cb0aa83faffe2c1e6761014333d6c67d759a4dd015689802df7c4e046f070e`  
		Last Modified: Tue, 09 Feb 2021 06:31:15 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7b424fc06113afad70f611d409ae8b18883c84b5f7f0b218eed8b58d4c7163`  
		Last Modified: Tue, 09 Feb 2021 06:31:15 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb1be752ed6ae3556fad53c70355e5674482a6dc5464beaff6818b4652679d1`  
		Last Modified: Tue, 09 Feb 2021 06:31:15 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19cb05227f413f6fb71f4bb73273f0477dec9c24006173c6b546eaa8240776d`  
		Last Modified: Tue, 09 Feb 2021 12:27:48 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e200ad0144185aeb9dd36a0fd6c3b1a51fc91de10677561d1fec9ca9d3740e`  
		Last Modified: Tue, 09 Feb 2021 12:27:48 GMT  
		Size: 3.4 MB (3431248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78851d9b8357c169c552ba77160fc90fdd10315671c0458cede1d348ea22978e`  
		Last Modified: Thu, 04 Mar 2021 02:44:49 GMT  
		Size: 9.7 MB (9712806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ddec4d1c3658c778a7ad1bab20c79e668ddd300c6931cacab416635a725668`  
		Last Modified: Thu, 04 Mar 2021 02:44:48 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c6fa8cbf9de5c8ad7df5cf59ef4359ee0b477f8f9b2861b7366871211b1de6`  
		Last Modified: Thu, 04 Mar 2021 02:44:48 GMT  
		Size: 613.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
