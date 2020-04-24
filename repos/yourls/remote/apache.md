## `yourls:apache`

```console
$ docker pull yourls@sha256:13c283788cb90cbf61fe37fa34e34198bf4dfb04e51956f5a81e7d1c787eeea6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `yourls:apache` - linux; amd64

```console
$ docker pull yourls@sha256:a5c73e5cfa57180856a847609994daf86b57940ea01c70eac6f7c884ae8fe00c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.7 MB (151654064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae1e5f6b1b795f03ce59593d123bba633fdb02aa6bde1471e10df57018c7280b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 15:16:13 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 16 Apr 2020 15:16:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 16 Apr 2020 15:16:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 15:16:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 16 Apr 2020 15:16:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 16 Apr 2020 15:23:34 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 16 Apr 2020 15:23:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 16 Apr 2020 15:23:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 16 Apr 2020 15:23:45 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 16 Apr 2020 15:23:46 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 16 Apr 2020 15:23:46 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 16 Apr 2020 15:23:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 16 Apr 2020 15:23:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 16 Apr 2020 15:23:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 11:30:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 14:05:04 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 17 Apr 2020 21:44:27 GMT
ENV PHP_VERSION=7.2.30
# Fri, 17 Apr 2020 21:44:27 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 21:44:27 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Fri, 17 Apr 2020 21:44:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 17 Apr 2020 21:44:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 21:49:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 21:49:34 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 17 Apr 2020 21:49:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 21:49:37 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 17 Apr 2020 21:49:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 21:49:38 GMT
STOPSIGNAL SIGWINCH
# Fri, 17 Apr 2020 21:49:38 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 17 Apr 2020 21:49:38 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 21:49:39 GMT
EXPOSE 80
# Fri, 17 Apr 2020 21:49:39 GMT
CMD ["apache2-foreground"]
# Sat, 18 Apr 2020 00:14:07 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Sat, 18 Apr 2020 00:14:08 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 18 Apr 2020 00:14:09 GMT
RUN a2enmod rewrite expires
# Wed, 22 Apr 2020 20:55:43 GMT
ENV YOURLS_VERSION=1.7.9
# Wed, 22 Apr 2020 20:55:43 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Wed, 22 Apr 2020 20:55:44 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 22 Apr 2020 20:55:44 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Wed, 22 Apr 2020 20:55:44 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Wed, 22 Apr 2020 20:55:45 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 22 Apr 2020 20:55:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Apr 2020 20:55:45 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7092974b7b31e1df4eea2a0dc16c923935c66865089738215d9d47c711045598`  
		Last Modified: Thu, 16 Apr 2020 17:30:22 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9112462bf4d40d5e33366d3124145a039c0f557d0a0269e614af8c1edec0b0f`  
		Last Modified: Thu, 16 Apr 2020 17:30:37 GMT  
		Size: 76.7 MB (76652064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9079bbeda63926320822bad70d04785361bd7d7246c0bcd9d8cce726f613aa59`  
		Last Modified: Thu, 16 Apr 2020 17:30:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ed61c235e6569a5569f403461b4febce1760cdbf888df7f510fde2f3b0918f`  
		Last Modified: Thu, 16 Apr 2020 17:30:57 GMT  
		Size: 18.7 MB (18675947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d7916f03ec1ba4bdae345f9197a428dce014f04652e652e22404a01cf2c82a`  
		Last Modified: Thu, 16 Apr 2020 17:30:52 GMT  
		Size: 442.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d60c7b08513aebc50bd1c0002f099c8bb1da134ca54cbde8c3e953a2d6628ae`  
		Last Modified: Thu, 16 Apr 2020 17:30:52 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29362d24be463a120a3acc2b488d677ef70a9035ba9bbdf6054e37e4a7b69775`  
		Last Modified: Fri, 17 Apr 2020 23:35:47 GMT  
		Size: 12.6 MB (12621665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff34b6a8cee0587e19aa1f50ac249e665b4bd9e7244472d52a7b9211d1b44f3c`  
		Last Modified: Fri, 17 Apr 2020 23:35:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bb8cf3dce29ff3466d2ce67afe5b36e4d6e248c563bf68bb7c4faef30ecf23`  
		Last Modified: Fri, 17 Apr 2020 23:35:48 GMT  
		Size: 13.8 MB (13820484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519e2ddee8a89a33c94a40e151fbdd583b022c9973de273d016109ef708fd739`  
		Last Modified: Fri, 17 Apr 2020 23:35:44 GMT  
		Size: 2.2 KB (2231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bedcf0e38242d31766dd7afc804355698b56027e716065df24b031e5eb8218`  
		Last Modified: Fri, 17 Apr 2020 23:35:44 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebd5f4cb9f48919ccf07bbd340aab332bcfbf69f062f922c4dd1db19d7cae7b`  
		Last Modified: Fri, 17 Apr 2020 23:35:44 GMT  
		Size: 212.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a2c0dea6b636e732e36828ed46e7f83b2c52c4509164caf9abaaaaa6a4cb46`  
		Last Modified: Fri, 17 Apr 2020 23:35:44 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919d90125cd88f189b691d875b7cf71ea96250799d2d039c71998f8e02fbbbc9`  
		Last Modified: Sat, 18 Apr 2020 00:15:50 GMT  
		Size: 289.5 KB (289508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402bf7a8c58380ee2b9cab1554766ffe57ac4297e447d65c609dee4d86cf0230`  
		Last Modified: Sat, 18 Apr 2020 00:15:50 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddca5e595f894fcb67c164487e65b1890510140f86c8e473633df2a6c185a18e`  
		Last Modified: Sat, 18 Apr 2020 00:15:48 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70ac0943e854881432da3003ed011639d314b8892f82c75218c66e8bb8ffd1d`  
		Last Modified: Wed, 22 Apr 2020 20:56:17 GMT  
		Size: 2.5 MB (2486736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805109b699bbe2cd4d1142f68088564e0af529ee3fd7b5a141e2331f606040c9`  
		Last Modified: Wed, 22 Apr 2020 20:56:16 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890c48696b5df4b56682f85bf108cf7a558a20cb354543400c5021c6e97b9dd5`  
		Last Modified: Wed, 22 Apr 2020 20:56:17 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e96cdbcd76f0de4a2d6a911ee4b2ec5e3621207f73acbfcb267d5a40a451dd5`  
		Last Modified: Wed, 22 Apr 2020 20:56:17 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; arm variant v5

```console
$ docker pull yourls@sha256:147694c9cd0bf4ada060565cd0637bdd42e543a99d69bf8a8456b547abbd938f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.9 MB (129942903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd162540fc37ddd9522edffd2b04f8856a686106a3cb06f9b32adbc49f0f39c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:52:22 GMT
ADD file:62a9732be4e3237ccc896f724a34606e01f351c4877e52c9a9cd85029c06b956 in / 
# Thu, 23 Apr 2020 00:52:23 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 05:05:35 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 05:05:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 05:06:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 05:06:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 05:06:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 05:10:27 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 05:10:28 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 05:10:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 05:10:55 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 05:10:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 05:10:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 05:10:59 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 05:11:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 05:11:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 05:11:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 06:02:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Apr 2020 06:02:47 GMT
ENV PHP_VERSION=7.2.30
# Thu, 23 Apr 2020 06:02:47 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 06:02:48 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Thu, 23 Apr 2020 06:03:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 06:03:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:06:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 06:06:07 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:06:09 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 06:06:12 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 06:06:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 06:06:13 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 06:06:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 06:06:15 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 06:06:15 GMT
EXPOSE 80
# Thu, 23 Apr 2020 06:06:16 GMT
CMD ["apache2-foreground"]
# Thu, 23 Apr 2020 10:04:06 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 23 Apr 2020 10:04:09 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 23 Apr 2020 10:04:12 GMT
RUN a2enmod rewrite expires
# Thu, 23 Apr 2020 10:04:13 GMT
ENV YOURLS_VERSION=1.7.9
# Thu, 23 Apr 2020 10:04:14 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Thu, 23 Apr 2020 10:04:18 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 23 Apr 2020 10:04:19 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 23 Apr 2020 10:04:21 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 23 Apr 2020 10:04:21 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 23 Apr 2020 10:04:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 10:04:23 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a8c46e5952878f9f324df86c5a2b45b2e0020f6721e820981e74461d77a100dd`  
		Last Modified: Thu, 23 Apr 2020 00:59:50 GMT  
		Size: 24.8 MB (24836319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a265de7879713459cf6e6045e802665b84c49dcb7194d42e80f713168a926d4`  
		Last Modified: Thu, 23 Apr 2020 06:32:43 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710cdb8f85f5abf4fda742431a0310421e7bd540337a4d831a04c9da4f000b2e`  
		Last Modified: Thu, 23 Apr 2020 06:33:06 GMT  
		Size: 58.8 MB (58799213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36a8c43726552051e04d6641b87a0c8dd7104c18f21f0b0a2f06ed6d5e03377`  
		Last Modified: Thu, 23 Apr 2020 06:32:43 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f47e3b4a8efcd60aaee6d37992bab4f13d460aaf38b73cdd30a6d76f99d21c8`  
		Last Modified: Thu, 23 Apr 2020 06:34:02 GMT  
		Size: 18.0 MB (18024804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc537d4bdd514646a167fc552d70b3fc62700d1466708f49dd826723aefb151`  
		Last Modified: Thu, 23 Apr 2020 06:33:55 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74bd7696ab34d6970527a338bbceeea2763f61f021062e941a73a963ce26e45`  
		Last Modified: Thu, 23 Apr 2020 06:33:56 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36c2823e33a5c8ade6b449da5505d0c6f8b02f96ea986839a9092361db9d215`  
		Last Modified: Thu, 23 Apr 2020 06:39:37 GMT  
		Size: 12.6 MB (12620186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b281f6d30ebd55f0cd9b5e50ab7cc7c62b162805d2e5a5d89e6d381bf345c4c4`  
		Last Modified: Thu, 23 Apr 2020 06:39:35 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75ef62a1f48f03d5e76fac0f1f2c246c00807e44632f276c7217e11dfc62461`  
		Last Modified: Thu, 23 Apr 2020 06:39:37 GMT  
		Size: 12.9 MB (12893579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bae8b6cae86040d710a5bdae0a81e2da8065a3c6884949e7d6b318a1eae1115`  
		Last Modified: Thu, 23 Apr 2020 06:39:32 GMT  
		Size: 2.2 KB (2233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf50402d42b66ada11fcf7cd422557e8c7823bfd2d2947a687246382b816302`  
		Last Modified: Thu, 23 Apr 2020 06:39:32 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652f045d73dc13cbb97a8dbf5b4d4409302688eaab7e856b207973cdb41aa533`  
		Last Modified: Thu, 23 Apr 2020 06:39:33 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ecca36e26f25e0ed5dfbd80d17e6faab319fb0884033af450ddfb74aecc2ee`  
		Last Modified: Thu, 23 Apr 2020 06:39:32 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c581022c19b66fb57530c906a9a7ed44ae6afaf75d971130991ef1750e6dd5d`  
		Last Modified: Thu, 23 Apr 2020 10:05:51 GMT  
		Size: 272.4 KB (272436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa982b7562e9d53bd94b2fbc6e891967050c46a6daeefffe843ce9fb414fec0d`  
		Last Modified: Thu, 23 Apr 2020 10:05:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6dab870332361457b4530b0bced5aa829696aee5642ea639b576e119625924c`  
		Last Modified: Thu, 23 Apr 2020 10:05:49 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0adfe950c1eea4122670b2b2b0d482d51cec707682c13038551cf1e26121f5f1`  
		Last Modified: Thu, 23 Apr 2020 10:05:49 GMT  
		Size: 2.5 MB (2486743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a64d1fd28a2bd32e32a44c001d8a9266760d50b7ccb9736644a48caf175e96`  
		Last Modified: Thu, 23 Apr 2020 10:05:49 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad4fb22f2f017a02316f00ec8ce0282f01ce232a865582430b015de8f2fcc8a`  
		Last Modified: Thu, 23 Apr 2020 10:05:49 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c488ce37a95176f5d2c8bcad6f34e4d5c3bab4078018938db16bd7ff11786373`  
		Last Modified: Thu, 23 Apr 2020 10:05:50 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; arm variant v7

```console
$ docker pull yourls@sha256:1d93c4eec30ba43f8a0e77f4b640eecd305198fe2553f97ff48cb59eca1bb558
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127215227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e93c9fe43b6629c04efd8a8241c54aa376065f7e779578cc3331476d9f41f11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 09:52:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 16 Apr 2020 09:52:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 16 Apr 2020 09:53:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 09:53:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 16 Apr 2020 09:53:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 16 Apr 2020 09:56:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 16 Apr 2020 09:56:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 16 Apr 2020 09:57:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 16 Apr 2020 09:57:10 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 16 Apr 2020 09:57:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 16 Apr 2020 09:57:13 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 16 Apr 2020 09:57:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 16 Apr 2020 09:57:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 16 Apr 2020 09:57:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 12:20:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 13:46:15 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 17 Apr 2020 21:42:06 GMT
ENV PHP_VERSION=7.2.30
# Fri, 17 Apr 2020 21:42:07 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 21:42:09 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Fri, 17 Apr 2020 21:42:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 17 Apr 2020 21:42:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 21:45:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 21:45:49 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Fri, 17 Apr 2020 21:45:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 21:46:05 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Fri, 17 Apr 2020 21:46:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 21:46:11 GMT
STOPSIGNAL SIGWINCH
# Fri, 17 Apr 2020 21:46:13 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 17 Apr 2020 21:46:17 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 21:46:20 GMT
EXPOSE 80
# Fri, 17 Apr 2020 21:46:22 GMT
CMD ["apache2-foreground"]
# Fri, 17 Apr 2020 23:09:08 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Fri, 17 Apr 2020 23:09:10 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Apr 2020 23:09:13 GMT
RUN a2enmod rewrite expires
# Wed, 22 Apr 2020 20:23:44 GMT
ENV YOURLS_VERSION=1.7.9
# Wed, 22 Apr 2020 20:23:45 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Wed, 22 Apr 2020 20:23:49 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 22 Apr 2020 20:23:50 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Wed, 22 Apr 2020 20:23:51 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Wed, 22 Apr 2020 20:23:51 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 22 Apr 2020 20:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Apr 2020 20:23:52 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f8fdbff988ba585ce37f923bf4b49474ca9c838dfe877ca1cb91db76b4750d`  
		Last Modified: Thu, 16 Apr 2020 11:20:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8674d4305249be09893f40da34923200030cb3141bef3a0007a7269611c7e1c`  
		Last Modified: Thu, 16 Apr 2020 11:21:11 GMT  
		Size: 59.5 MB (59501464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d380b1b0920e653046b83a9ac2f4faf28f2aca78e9723d0a7d849bb2bb71916`  
		Last Modified: Thu, 16 Apr 2020 11:20:53 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9847b729f5a859a271aaa60b46d48bee309d71554aa55476ea4e8aa99688ece0`  
		Last Modified: Thu, 16 Apr 2020 11:21:41 GMT  
		Size: 17.5 MB (17482026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e06ca2a6c0951b7d743a41e0a318e8181ababbb9af1c3cf8f726aad2fed8b0`  
		Last Modified: Thu, 16 Apr 2020 11:21:36 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195eac7a68bb7f62edcb1ff9051505c0f018ba109e9cb3e004966cdb745d5666`  
		Last Modified: Thu, 16 Apr 2020 11:21:36 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317f32b4b71acb8266e390ce799e8867889c1ac4b56ebf460af526c35d60190a`  
		Last Modified: Fri, 17 Apr 2020 22:38:20 GMT  
		Size: 12.6 MB (12620204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78891e705f6156751705d1c99f727ae02f264eaade9d5185b96c92bfa703a52f`  
		Last Modified: Fri, 17 Apr 2020 22:38:18 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4eee20573b77fd0afeb3fa8cc56e14b3460bd8a0e07a1e26bc46f0095a0fe9`  
		Last Modified: Fri, 17 Apr 2020 22:38:21 GMT  
		Size: 12.2 MB (12164098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e5a2e965262c5363dbcec7a524bf5f71aa99774a7a5b2ef14a0ad6aca757985`  
		Last Modified: Fri, 17 Apr 2020 22:38:17 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc13b9b06fd9d27026bc82e1bd65452378dcce31af5b0cbeab7d0ece44349471`  
		Last Modified: Fri, 17 Apr 2020 22:38:17 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904d472b311e20c791f291353beaf9b4d9f1e92125fff7ed7cde8546971f1f28`  
		Last Modified: Fri, 17 Apr 2020 22:38:17 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27dca827e1c6139c18290286e152500e930c1b80c8dd9eed780363ebbf3b073f`  
		Last Modified: Fri, 17 Apr 2020 22:38:17 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19dab0d57a086bb3da83a97c0c37ecc47e8c5ffdaffc8736e41ca009f17eea77`  
		Last Modified: Fri, 17 Apr 2020 23:11:37 GMT  
		Size: 245.8 KB (245820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13928396910a5eba124768ccb283a3342ba5b5c5e1bef11a825634296c08aa7`  
		Last Modified: Fri, 17 Apr 2020 23:11:37 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deec68ac86b8067615ade06f07c485eed1d3aa192711d50aaa2b1d393380fbd5`  
		Last Modified: Fri, 17 Apr 2020 23:11:35 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:373041c13e49c51501daad3ca952f8035a89801475ef8418c370bd7a00597f09`  
		Last Modified: Wed, 22 Apr 2020 20:24:34 GMT  
		Size: 2.5 MB (2486747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c2890eca896519c08b404fdbfa473afa9216abed319589dd8cccfbea451b11`  
		Last Modified: Wed, 22 Apr 2020 20:24:33 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cb114a623c22dd42c8291f2d8f0efcd77b71f390761bbc780c5d063cd5b7cb`  
		Last Modified: Wed, 22 Apr 2020 20:24:33 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc1ee58000e502d1d8cbc1c24dba5979de6ec844abff6371caf7c0489ef2d33`  
		Last Modified: Wed, 22 Apr 2020 20:24:34 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:0ceb1063cce487b9aaf87901929d60af43382ec52930a1b50922ebad341c89ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.7 MB (143687343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbf9eb5987d6ef53e09d692384d6198bd2bd83e6ba720ec6eae5c9e1b5e6565f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:55 GMT
ADD file:581ee9c3c19f0d971aeda008fd399f59171cae75e8936b967dbf3888db4fc0d0 in / 
# Thu, 23 Apr 2020 00:54:58 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 16:09:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 16:09:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 16:10:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 16:10:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 16:10:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 16:16:15 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 16:16:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 16:16:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 16:16:48 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 16:16:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 16:16:53 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 16:16:54 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 16:16:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 16:16:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 16:16:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 17:20:04 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Apr 2020 17:20:05 GMT
ENV PHP_VERSION=7.2.30
# Thu, 23 Apr 2020 17:20:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 17:20:07 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Thu, 23 Apr 2020 17:20:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 17:20:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:23:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 17:23:22 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:23:25 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 17:23:27 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 17:23:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 17:23:28 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 17:23:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 17:23:29 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 17:23:30 GMT
EXPOSE 80
# Thu, 23 Apr 2020 17:23:31 GMT
CMD ["apache2-foreground"]
# Fri, 24 Apr 2020 02:30:15 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Fri, 24 Apr 2020 02:30:48 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Apr 2020 02:31:08 GMT
RUN a2enmod rewrite expires
# Fri, 24 Apr 2020 02:31:09 GMT
ENV YOURLS_VERSION=1.7.9
# Fri, 24 Apr 2020 02:31:09 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Fri, 24 Apr 2020 02:31:25 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 24 Apr 2020 02:31:27 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Fri, 24 Apr 2020 02:31:31 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Fri, 24 Apr 2020 02:31:35 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 24 Apr 2020 02:31:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 02:31:49 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bdc84a41f2513e28e99efeff9fcbb196b7df9883fb30532184bd67ca415b4673`  
		Last Modified: Thu, 23 Apr 2020 01:03:27 GMT  
		Size: 25.9 MB (25857800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00aeccd126509e0b42d6cba92126cce7c342206083cc40a285bd447cf1f2d46`  
		Last Modified: Thu, 23 Apr 2020 17:51:33 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103463f158e3c7f91314c099c5524db53fd97efd35b7502a2991750063630384`  
		Last Modified: Thu, 23 Apr 2020 17:51:55 GMT  
		Size: 70.3 MB (70334752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c968fd52774e9a63a8ca1cd66b708fb02df8fdc207dc98e23a8682010b0047`  
		Last Modified: Thu, 23 Apr 2020 17:51:33 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059cf3850d2505684647002e52f9e280c1cf6a30b8c49dddd6017ee83798bbb7`  
		Last Modified: Thu, 23 Apr 2020 17:52:43 GMT  
		Size: 18.6 MB (18579535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a2d85f3606b4622b9b2a90e8d654227e9f0ebd232876fe876afc91896d24b7`  
		Last Modified: Thu, 23 Apr 2020 17:52:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48169ea54a2577041dac811d298ab9e023a176fdc6dcb8c95c5cf41ebb9e378b`  
		Last Modified: Thu, 23 Apr 2020 17:52:34 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e8f6a5fc522a3a6a8883e94aec4dec308382d3276dd622c947c731f0d54a63`  
		Last Modified: Thu, 23 Apr 2020 17:57:27 GMT  
		Size: 12.6 MB (12620820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38176f6c994141ea6ff3ea8293aea24c5d9cd42b13118f1a2e7986fd84fc6bae`  
		Last Modified: Thu, 23 Apr 2020 17:57:26 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70dd48731ec10ffd741e4d64784f91f3fd9ac32fc4752874a55a6bd05ccd68b`  
		Last Modified: Thu, 23 Apr 2020 17:57:27 GMT  
		Size: 13.5 MB (13515527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45eea01a1589e29288ffcdcf0e441afccb1477a2b2346114b5ad41d097ed69cd`  
		Last Modified: Thu, 23 Apr 2020 17:57:24 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419a27b6ead13d9076fc242908bae11cd697dce0b2d4972e6108fa32943df22d`  
		Last Modified: Thu, 23 Apr 2020 17:57:24 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d60467826ad6a082394b292c88a6c981a1dce4b5426d2537ceacf8a2e8edf90`  
		Last Modified: Thu, 23 Apr 2020 17:57:24 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9205e491a39ea3315b78ea15f5a1d1f3db36ad51396eea3b1a497d283704389c`  
		Last Modified: Thu, 23 Apr 2020 17:57:24 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af8a190855e7a0bfaa266d34bb2ba3af8bc3ca650e4c87561edb3cd78b5fe68`  
		Last Modified: Fri, 24 Apr 2020 02:35:34 GMT  
		Size: 282.5 KB (282545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8b190bde9aa9a02f23ce2a5015d4b9488aa52ab0a3c855c1af3c2051bab9a0`  
		Last Modified: Fri, 24 Apr 2020 02:35:33 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a03c02485562558cc919fd386278e2e63465d0509090f2792876e4094dd099`  
		Last Modified: Fri, 24 Apr 2020 02:35:30 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9897efa3cddae99d6a34a3adf95130f50685a5d7d2b372cb44aa4212f8ce84`  
		Last Modified: Fri, 24 Apr 2020 02:35:31 GMT  
		Size: 2.5 MB (2486747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae7425df61fc49b209be248a99244f1bcdbc90046075e176fd1cc0decd2b36a`  
		Last Modified: Fri, 24 Apr 2020 02:35:31 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce4815cb8b8cbff070d3ee708fe3b608eddd67030e72fd0a69eafae731c5d12`  
		Last Modified: Fri, 24 Apr 2020 02:35:31 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf8b0b64262ef43a61673fdb031e75f3170a1dd9002ff932ca25f0505123ad2`  
		Last Modified: Fri, 24 Apr 2020 02:35:30 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; 386

```console
$ docker pull yourls@sha256:d27c22c22d5b7333837a840b20324c10196652372759940aacc84de44dfee4fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.6 MB (157623108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:752b15d083de24f0ae195fc7f67c048dcdb0ecbbb09cc70f1fdb3e6e09d7b02c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:36 GMT
ADD file:ca6a74f6b738c738c033152fab2a9aacf22bec5f19a994e6a02b5f919ee33ee9 in / 
# Thu, 23 Apr 2020 00:39:36 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 11:58:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 11:58:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 11:58:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 11:58:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 11:58:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 12:06:34 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 12:06:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 12:06:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 12:06:50 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 12:06:51 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 12:06:52 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 12:06:52 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 12:06:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 12:06:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 12:06:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 13:29:29 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Apr 2020 13:29:29 GMT
ENV PHP_VERSION=7.2.30
# Thu, 23 Apr 2020 13:29:29 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 13:29:29 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Thu, 23 Apr 2020 13:29:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 13:29:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:33:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 13:33:33 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:33:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 13:33:35 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 13:33:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 13:33:36 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 13:33:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 13:33:36 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 13:33:36 GMT
EXPOSE 80
# Thu, 23 Apr 2020 13:33:36 GMT
CMD ["apache2-foreground"]
# Thu, 23 Apr 2020 20:57:22 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 23 Apr 2020 20:57:23 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 23 Apr 2020 20:57:24 GMT
RUN a2enmod rewrite expires
# Thu, 23 Apr 2020 20:57:24 GMT
ENV YOURLS_VERSION=1.7.9
# Thu, 23 Apr 2020 20:57:24 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Thu, 23 Apr 2020 20:57:26 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 23 Apr 2020 20:57:26 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 23 Apr 2020 20:57:27 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 23 Apr 2020 20:57:27 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 23 Apr 2020 20:57:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 20:57:27 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5d3da8f33b97fc107a05b3255a55836b76df9f817de632b1fb63c6e9c024f0df`  
		Last Modified: Thu, 23 Apr 2020 00:44:35 GMT  
		Size: 27.8 MB (27753972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b6f6109ad6afc6066a9a9b19c9903065b90dc4ecb232ad312a50d2a3af7c20`  
		Last Modified: Thu, 23 Apr 2020 14:14:03 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b8d4220a9dc78cfb17d7518deddaa4957545b12088485de215374ec8cd5fcd`  
		Last Modified: Thu, 23 Apr 2020 14:14:26 GMT  
		Size: 81.2 MB (81198126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd893e354bac0fa6072eb200ef4c28c499dce07f2bf148816b9b04550dc27082`  
		Last Modified: Thu, 23 Apr 2020 14:14:02 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a71342deb67ff65b123b84dec7f6dd3772d7418cab3b8f1c9b05d2ed015c00a`  
		Last Modified: Thu, 23 Apr 2020 14:14:52 GMT  
		Size: 19.1 MB (19112697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69b5a5b87d25a9b0d974f78ef0902be086f49e7e4a97921db839b9e6882d06c`  
		Last Modified: Thu, 23 Apr 2020 14:14:46 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbd15ab6153d2103bf3572f753d9ca318b71e50d3a5808c0919f3cbed98c806`  
		Last Modified: Thu, 23 Apr 2020 14:14:45 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d6a2bc540e2770ba1b1471d4fab060edca9a94f1713bca1475f900fa10c05e`  
		Last Modified: Thu, 23 Apr 2020 14:18:46 GMT  
		Size: 12.6 MB (12621172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a53e9baa5cd925f8b872187a291fb7fa4d36dd03f31f739af1af03edb93413e`  
		Last Modified: Thu, 23 Apr 2020 14:18:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5670903c2c4586cc4e4684fcbaba9b4c617fa235f473fca2ef310fe5c70315be`  
		Last Modified: Thu, 23 Apr 2020 14:18:47 GMT  
		Size: 14.1 MB (14143361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d0223e7126e1479e7c22a5e91f07676439b1245f84d1806a4dc0b31529d2d3`  
		Last Modified: Thu, 23 Apr 2020 14:18:42 GMT  
		Size: 2.2 KB (2230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27166397ef9c35985de82bfdb092724bb146bcc0f8d4115615636363ba61d4c4`  
		Last Modified: Thu, 23 Apr 2020 14:18:42 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22dacb890ce665b6f3b812a6d5860568309e7273d3e37d43aeee83ba6268373e`  
		Last Modified: Thu, 23 Apr 2020 14:18:42 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94eaf4812db87fd1a69f374919165e78cfa7e5ea3685635409ebaa8f79f90f2`  
		Last Modified: Thu, 23 Apr 2020 14:18:42 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d071174b4bd7ed0652b84fdabf5a394c60500d96b7c8bdf185e32402362c0410`  
		Last Modified: Thu, 23 Apr 2020 20:58:32 GMT  
		Size: 297.5 KB (297540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302b27caa4cd72d45ab05edfcb9b8c851e241d8669b87e2f28bb9e7d96f9abdb`  
		Last Modified: Thu, 23 Apr 2020 20:58:32 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3a25b82bf509b92c4b796a1e5c8fba8c58646c5acbd9a12da5fb68616d80c6`  
		Last Modified: Thu, 23 Apr 2020 20:58:31 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d352d04297410280ce02e63065b781560c84cfa49be8c54b6526846d9bd266`  
		Last Modified: Thu, 23 Apr 2020 20:58:33 GMT  
		Size: 2.5 MB (2486734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4087de0846263fda869769b1ad38345f0545e7451aa6c673577e9cf94be71bd`  
		Last Modified: Thu, 23 Apr 2020 20:58:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba64e4abbcb8ed7a3e1f9c66ad977080d808b7f1739c1ac584c51d3be58a02ea`  
		Last Modified: Thu, 23 Apr 2020 20:58:32 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e427d4d014ab928b8e6df0a60d653fcd557e6fd267517ea6eec168d77039228e`  
		Last Modified: Thu, 23 Apr 2020 20:58:31 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; ppc64le

```console
$ docker pull yourls@sha256:2c37b75f9677aea715edc2bd3ff3b83fd3f77d66516c2f6eafefe7d9d1a433fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.9 MB (162892463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1c0c952152dd2bf990caf22d5f82d5aaa8476c3128975fef16451b34e0b9f9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:36:00 GMT
ADD file:5b3c3d2945800e1743dc02a4f68bd830fe2f67ca437223692eb460147c158c2b in / 
# Thu, 23 Apr 2020 00:36:04 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 14:58:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 14:58:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 15:00:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 15:01:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 15:01:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 15:07:57 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 15:08:03 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 15:09:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 15:09:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 15:09:24 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 15:09:28 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 15:09:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 15:09:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 15:09:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 15:09:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 16:31:00 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Apr 2020 16:31:03 GMT
ENV PHP_VERSION=7.2.30
# Thu, 23 Apr 2020 16:31:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 16:31:16 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Thu, 23 Apr 2020 16:32:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 16:32:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:36:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 16:36:56 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:37:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 16:37:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 16:37:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 16:37:22 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 16:37:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 16:37:28 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 16:37:30 GMT
EXPOSE 80
# Thu, 23 Apr 2020 16:37:34 GMT
CMD ["apache2-foreground"]
# Fri, 24 Apr 2020 01:04:10 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Fri, 24 Apr 2020 01:04:14 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Apr 2020 01:04:19 GMT
RUN a2enmod rewrite expires
# Fri, 24 Apr 2020 01:04:20 GMT
ENV YOURLS_VERSION=1.7.9
# Fri, 24 Apr 2020 01:04:23 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Fri, 24 Apr 2020 01:04:29 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 24 Apr 2020 01:04:30 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Fri, 24 Apr 2020 01:04:32 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Fri, 24 Apr 2020 01:04:32 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 24 Apr 2020 01:04:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Apr 2020 01:04:36 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:012c6cdbd1af202bbfbea5945fafbb9aca9097f1fa3cb493a29155fdc02cc43c`  
		Last Modified: Thu, 23 Apr 2020 00:50:14 GMT  
		Size: 30.5 MB (30524638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b755a3bf05f4bf7425e586a874481ea765f886765d68e5e3973f9ac727187c6c`  
		Last Modified: Thu, 23 Apr 2020 17:16:22 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81edbd0a9383cf9bc58dcb07cb9b0cc6454030497e3a606ae400db6a3b6a1962`  
		Last Modified: Thu, 23 Apr 2020 17:17:15 GMT  
		Size: 82.3 MB (82259619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947531f183613e1f7fca563adeccbc3242cda14370ed376901fbf634af0264c3`  
		Last Modified: Thu, 23 Apr 2020 17:16:20 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a95e79fe710527d52bde3f306bfd30c4fd804fa4ef236e53a0bcf240504c8aa`  
		Last Modified: Thu, 23 Apr 2020 17:18:21 GMT  
		Size: 19.8 MB (19812607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de97ec0f6e96230894adec6eadf7a2f8cc7608e6dd5b441dfe99cac9ac85357`  
		Last Modified: Thu, 23 Apr 2020 17:18:12 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8347f80ea17e906c812e85500251d7c276e9380aeb01c0326b9026631d2b09b`  
		Last Modified: Thu, 23 Apr 2020 17:18:08 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba124d8e93b2a589eb3f7865f46f3b9ae7f6fe500a16fccadb379ab7702e695`  
		Last Modified: Thu, 23 Apr 2020 17:25:55 GMT  
		Size: 12.6 MB (12621648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca05b738fc378a7320ad7e50829d12298feb36c7f55d321ce9faecbfeddaef32`  
		Last Modified: Thu, 23 Apr 2020 17:25:53 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb7f7b6f9c104d69b2f7aec8b1e780f84fe10e47f5bb81f8d7dfda35b56e5f5`  
		Last Modified: Thu, 23 Apr 2020 17:25:58 GMT  
		Size: 14.9 MB (14856821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1748acb7efb7d100da98b68619253f8906218c9bb3a9599edd4bee8cf5e0cd`  
		Last Modified: Thu, 23 Apr 2020 17:25:49 GMT  
		Size: 2.2 KB (2234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00ce8c51c779b107f9ec2482d319792f190d081ff4fbd2e15b2fc5465d8b840`  
		Last Modified: Thu, 23 Apr 2020 17:25:49 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b28e6e2e33db39b08b4f4f50e3c24a770de61521c256f96b844b593a4fe0a2`  
		Last Modified: Thu, 23 Apr 2020 17:25:49 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c3c6d7a2123346d6872d99770d5a2958ee5571aae92434ecb57ff5a5f819b8`  
		Last Modified: Thu, 23 Apr 2020 17:25:48 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25277730b57976d67c7e201a0a823f014b522435cafa53db6ca5e518bc6640c`  
		Last Modified: Fri, 24 Apr 2020 01:06:08 GMT  
		Size: 320.7 KB (320741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bda9418cec18d762bbef2e145f95d02af560bf4ad15ef28ec4ecb7c09070e8e`  
		Last Modified: Fri, 24 Apr 2020 01:06:08 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c54134383afae141374fb11deb29d27d7f6f05e46a2336534eb71b4cc8c1397`  
		Last Modified: Fri, 24 Apr 2020 01:06:03 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c678ab9e3542814ac3d8af24ab3dd6f0f9ad24b9fc69db3ef4e159c82c5cab02`  
		Last Modified: Fri, 24 Apr 2020 01:06:04 GMT  
		Size: 2.5 MB (2486748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ab15d2592e602772d53673194f6ee4ba678630aa8a94792b13eb4ee81a8128`  
		Last Modified: Fri, 24 Apr 2020 01:06:04 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634794597f465d4ce746152a6b817a6907fe8b0817a467a74c1c9dd7cb4dc431`  
		Last Modified: Fri, 24 Apr 2020 01:06:03 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8597dde0a211df0c04f07f85550f53bd71743207bafae4f1e12e09ede8d39f46`  
		Last Modified: Fri, 24 Apr 2020 01:06:04 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:apache` - linux; s390x

```console
$ docker pull yourls@sha256:02368aa3d500d4084be6e314d05509bc715955078d9647a1da38d3a538250126
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.4 MB (137422780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab3a09e59ac70c200a3b5beedf21ee63aa23e6c6d9c3e0cbe07b8ba3e320c64b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:48 GMT
ADD file:f6c2560f9185c1bcaff95e576e57449f606d51b85fad02646c1b0962bc9353c9 in / 
# Thu, 23 Apr 2020 00:51:50 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 07:06:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Apr 2020 07:06:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Apr 2020 07:07:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 07:07:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 07:07:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 07:10:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 23 Apr 2020 07:10:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 23 Apr 2020 07:10:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 23 Apr 2020 07:10:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 23 Apr 2020 07:10:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 23 Apr 2020 07:10:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 23 Apr 2020 07:10:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 23 Apr 2020 07:10:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 07:10:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 07:10:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 07:43:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Thu, 23 Apr 2020 07:43:47 GMT
ENV PHP_VERSION=7.2.30
# Thu, 23 Apr 2020 07:43:48 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 07:43:48 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Thu, 23 Apr 2020 07:44:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 23 Apr 2020 07:44:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:46:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 07:46:58 GMT
COPY multi:3ab587b19c9ec9c9b34bacbe7fa0911462d0bafd50179d8808e207ed9b82b0b9 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:46:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 07:47:00 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 23 Apr 2020 07:47:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 07:47:00 GMT
STOPSIGNAL SIGWINCH
# Thu, 23 Apr 2020 07:47:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 23 Apr 2020 07:47:01 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 07:47:01 GMT
EXPOSE 80
# Thu, 23 Apr 2020 07:47:02 GMT
CMD ["apache2-foreground"]
# Thu, 23 Apr 2020 15:44:17 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 23 Apr 2020 15:44:18 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 23 Apr 2020 15:44:18 GMT
RUN a2enmod rewrite expires
# Thu, 23 Apr 2020 15:44:19 GMT
ENV YOURLS_VERSION=1.7.9
# Thu, 23 Apr 2020 15:44:19 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Thu, 23 Apr 2020 15:44:21 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 23 Apr 2020 15:44:21 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 23 Apr 2020 15:44:21 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 23 Apr 2020 15:44:21 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 23 Apr 2020 15:44:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Apr 2020 15:44:22 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d89dc3741ad42b79c3d8545495c429f3100d3f22234ff993bd04017b0675e868`  
		Last Modified: Thu, 23 Apr 2020 00:56:00 GMT  
		Size: 25.7 MB (25712105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea08bde6b0b1d4817b549715812249f566ebbdb1c81c26581d3a34e9f0646ac7`  
		Last Modified: Thu, 23 Apr 2020 08:06:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb184ae545a538a5e99fa27bf76f21aeb7324f061ae0e6ed7ab6003f8ec8d861`  
		Last Modified: Thu, 23 Apr 2020 08:06:57 GMT  
		Size: 64.7 MB (64698982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bff96336b89f3c42d3c1ca154c9bee84597dd2e1776952a82e47e94dac6e5c`  
		Last Modified: Thu, 23 Apr 2020 08:06:45 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2101c4a938d8b8d63ad7e9e67ce5e8f648130174093f07c2dba57707145c46e4`  
		Last Modified: Thu, 23 Apr 2020 08:07:42 GMT  
		Size: 18.5 MB (18522444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98988af543b5301ceb878cb0da958a05b2d1ba052efd8780bcbe589b82bcbe1`  
		Last Modified: Thu, 23 Apr 2020 08:07:39 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd3c6a14b8cb1d6330e59c568e4a5aa3c4035eedd019b1b06b7f9aded5e4e66`  
		Last Modified: Thu, 23 Apr 2020 08:07:37 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2c6d68432c475b4af00d0941a04eab250e4c7f007a12e03542fc56242c4a42`  
		Last Modified: Thu, 23 Apr 2020 08:12:04 GMT  
		Size: 12.6 MB (12620485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed345b533ef5dfd890d08118daa005bfc22c1706c3ff6671983bab48f9730444`  
		Last Modified: Thu, 23 Apr 2020 08:12:01 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9213a65eec396193fd6ee358399196ec97d1d94bf663e3ccf0ac346277334d`  
		Last Modified: Thu, 23 Apr 2020 08:12:02 GMT  
		Size: 13.1 MB (13090448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96c4769c36be1d26b4519998329dfcc061733d50eda00505a3082b6a5a00d22`  
		Last Modified: Thu, 23 Apr 2020 08:11:59 GMT  
		Size: 2.2 KB (2229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740354bc612cbeb2f558b8c2e1b95e09761ec4ec09298282860ce603d857a0dc`  
		Last Modified: Thu, 23 Apr 2020 08:12:05 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869ca0d35a9e25f3eebf7fcaf5e3bf61f3ec4b5d614bca8d867ffe45b2b6f9f2`  
		Last Modified: Thu, 23 Apr 2020 08:12:05 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38222bfdf3e3b63104ef74a2bbf711e41b42d4bbc572b330797367b517ba72d8`  
		Last Modified: Thu, 23 Apr 2020 08:12:05 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e0e68513f8b58b54dce5350b388734790be6a4d19572590859e625fdda5851`  
		Last Modified: Thu, 23 Apr 2020 15:45:07 GMT  
		Size: 282.0 KB (281970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3cc510195f4fe1db1f832246f8e2c5a1f39544c9161da299750cbeae0cca9e9`  
		Last Modified: Thu, 23 Apr 2020 15:45:06 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2260e9a129a4ea26168f1af671747a2477b10a0bba21d3101dbe15842694917`  
		Last Modified: Thu, 23 Apr 2020 15:45:05 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8224b4672c85473affa8a4cb36ae0b194f1bfe5ab03148b76307b5a46eea29`  
		Last Modified: Thu, 23 Apr 2020 15:45:05 GMT  
		Size: 2.5 MB (2486744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1605b1148caddbe240576e8900345bd19228de139a5af8c24a4fbdc8c5fcff5e`  
		Last Modified: Thu, 23 Apr 2020 15:45:10 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784ef11e02c9658af52a18523b4cd79688d0361fb611e618dc1b08a85cc13f3b`  
		Last Modified: Thu, 23 Apr 2020 15:45:10 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063f089c5fbc302d1bb05fcd93357ffc13cc22806b22a106084fb30f360ae774`  
		Last Modified: Thu, 23 Apr 2020 15:45:10 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
