## `php:8-apache`

```console
$ docker pull php@sha256:99dd27122a436af177c97ffea1171658ce5d6b8648effff7ec640c97d543838a
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

### `php:8-apache` - linux; amd64

```console
$ docker pull php@sha256:b03a470cb6f3006a08ce0d94b68f32872dc59989b71125235bfd73f397e3d404
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148109751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2f21214ebe4824b82ed73ea0bab19310bdcde76148f48974a7ccbcdc1db2dc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 11:48:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 11:48:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 11:48:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 11:48:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 11:48:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 11:55:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 11:55:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 11:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 11:55:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 11:55:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 11:55:55 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 11:55:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 11:55:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 11:55:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 11:55:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 12:25:06 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Jun 2021 12:25:07 GMT
ENV PHP_VERSION=8.0.7
# Wed, 23 Jun 2021 12:25:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Wed, 23 Jun 2021 12:25:07 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Mon, 28 Jun 2021 20:34:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 20:34:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:42:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 20:42:28 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:42:30 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 20:42:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 20:42:31 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 20:42:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:42:32 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 20:42:32 GMT
EXPOSE 80
# Mon, 28 Jun 2021 20:42:33 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b85dd8f01492a64ab518247894d5b93db91b5ef9c770b601b37f612278b602`  
		Last Modified: Wed, 23 Jun 2021 13:53:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8589b26a90be6577309788924232d8900e0e44f0a7fb4ca01c32c6467578a27d`  
		Last Modified: Wed, 23 Jun 2021 13:53:50 GMT  
		Size: 76.7 MB (76680976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5af5d6419462987bdb2cd60de0729dcf0c35933ca87692f2eb9ca1ae292a642`  
		Last Modified: Wed, 23 Jun 2021 13:53:31 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614ec6f0b8d6a562071e6a2584ca97b4237364aa3b78b00aa6c601a00c80d019`  
		Last Modified: Wed, 23 Jun 2021 13:54:26 GMT  
		Size: 18.7 MB (18679261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b28f3797fbefaacc6339a39139cd689c6038bdbe1ee96bd947d58397be3538`  
		Last Modified: Wed, 23 Jun 2021 13:54:22 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bcb7d2e6b049343069918b727a239aa0ae67500a2f20744af37dd6c89d90d9`  
		Last Modified: Wed, 23 Jun 2021 13:54:22 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f498fead0caf67f3ed895e2aa4f2710ef70ceed79417751a5a4460e3f212e05`  
		Last Modified: Tue, 29 Jun 2021 00:41:31 GMT  
		Size: 11.1 MB (11107208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b3ae361dfff263f5d291f4e25641687471afd13c70b288cf92933854632144b`  
		Last Modified: Tue, 29 Jun 2021 00:41:27 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d90e97ce896d9002a630da78d749f64fb3b37d8014ee731f9b7e65bd576a343`  
		Last Modified: Tue, 29 Jun 2021 00:41:31 GMT  
		Size: 14.5 MB (14491056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c5d5835f79ae5591d5ccfa1784bcfc7190b3ca845322bb3b1ef6b0dc7c33c0`  
		Last Modified: Tue, 29 Jun 2021 00:41:27 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feeffb96e797e7a2879c53b1653b1268e440dee4e0631e34543a5b4a17565acc`  
		Last Modified: Tue, 29 Jun 2021 00:41:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f70a1317ab5d213f09a7979ca976483bf4298b387c7d7e506e955fbe7a7614`  
		Last Modified: Tue, 29 Jun 2021 00:41:27 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache` - linux; arm variant v5

```console
$ docker pull php@sha256:1029c848aa609cf7562f5d10f6acbb7870452f73c0b553c744d60b1bbf77a611
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126041567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:152b06ea34edea081826c35fe837988d43ca023c3a63773857083d4e83a2a71b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:34:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 06:34:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 06:35:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:35:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 06:35:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 06:41:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 06:41:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 06:41:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 06:41:33 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 06:41:35 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 06:41:35 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 06:41:35 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 06:41:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 06:41:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 06:41:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 07:04:26 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Jun 2021 07:04:27 GMT
ENV PHP_VERSION=8.0.7
# Wed, 23 Jun 2021 07:04:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Wed, 23 Jun 2021 07:04:27 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Mon, 28 Jun 2021 19:23:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 19:23:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:28:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 19:28:15 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:28:17 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 19:28:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 19:28:18 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 19:28:19 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:28:19 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 19:28:19 GMT
EXPOSE 80
# Mon, 28 Jun 2021 19:28:20 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4201a900b66f4e05c8ee53ef7ecdffa56d4cfc141826c4899ba2c7ea1565c3`  
		Last Modified: Wed, 23 Jun 2021 08:37:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8759f5b6f404f221d7035198880caf6e5b60d43c01daf59b9c7ff32e8ba5038f`  
		Last Modified: Wed, 23 Jun 2021 08:37:51 GMT  
		Size: 58.8 MB (58820428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bee84cde96b6e1abd89640d87273fd846cad74593b3ec8bdd0167bb76f06398`  
		Last Modified: Wed, 23 Jun 2021 08:37:06 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d04a75937c26e6facc2a34e28c4f30008fb2c8c38d4a6109ab3bd73a1a4d516`  
		Last Modified: Wed, 23 Jun 2021 08:38:40 GMT  
		Size: 18.0 MB (18026172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ecd491048519ab1e7d82a3cf53d86795ba9b3b230f90332de7efe0d76f16cd`  
		Last Modified: Wed, 23 Jun 2021 08:38:29 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b63bc3f991d218876d985827b11cbce08ca267e836215529cbbfbd0a0abf7b`  
		Last Modified: Wed, 23 Jun 2021 08:38:29 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b6cf18394211863f531172a5d81e0024d1b3741551bbdb52da7c15615f1b56`  
		Last Modified: Mon, 28 Jun 2021 21:00:40 GMT  
		Size: 11.1 MB (11105084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75111b970224a47844e63c7d150804c50ceed614e836dfae1dc7d525a27b9248`  
		Last Modified: Mon, 28 Jun 2021 21:00:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6490fd0f7755b6ab553a5fbdfd7dab77cf9bd413a142aa0d3d6b737f451906d7`  
		Last Modified: Mon, 28 Jun 2021 21:00:46 GMT  
		Size: 13.2 MB (13205536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:618e2671b0dc930717408fa36e3239ecb58d5aed862fc3ab7e46347ac4f8aec0`  
		Last Modified: Mon, 28 Jun 2021 21:00:35 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768fe26668889cdff2d8146b232c957abfd9e5d06a3d1db69756527b4bc3561c`  
		Last Modified: Mon, 28 Jun 2021 21:00:35 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d3ce11ba8ecc6dc7fb9a4c6c3b6848e8537922437ce09558ba1843faf8d71e`  
		Last Modified: Mon, 28 Jun 2021 21:00:35 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache` - linux; arm variant v7

```console
$ docker pull php@sha256:5e48375e1803af79dfcf2d5d00e7c202b7d9824216fec551ca1c281c35b79142
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123355819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:030a8050ff7af9b92a80557b90059ceabdf5e1e0bb2d8dd39fed67b1791aafee`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:21:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 08:21:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 08:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:22:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 08:22:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 08:27:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 08:27:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 08:27:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 08:27:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 08:27:28 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 08:27:29 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 08:27:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 08:27:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:27:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:27:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 09:06:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Jun 2021 09:06:47 GMT
ENV PHP_VERSION=8.0.7
# Wed, 23 Jun 2021 09:06:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Wed, 23 Jun 2021 09:06:47 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Mon, 28 Jun 2021 20:36:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 20:36:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:41:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 20:41:21 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:41:23 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 20:41:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 20:41:24 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 20:41:24 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:41:24 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 20:41:25 GMT
EXPOSE 80
# Mon, 28 Jun 2021 20:41:25 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9600bb4c83e3ef3465228eed7d6e9dfed7dc9078d2ab47f0bbdc8ccd6cb2b4`  
		Last Modified: Wed, 23 Jun 2021 11:51:40 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4b7395146be79190767115c26cc6b70ac8d5af36c4a7acf9de1f34d06b41d7`  
		Last Modified: Wed, 23 Jun 2021 11:52:18 GMT  
		Size: 59.5 MB (59514051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3641f6e3173b95d08e8b4ec00f48cb7e09d9813f88a086a422173594dfc93ddd`  
		Last Modified: Wed, 23 Jun 2021 11:51:40 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7d1aa9268ffe2596e041fe0130bbdc37fb7e587a9b8d7c5346360e2f27b41d`  
		Last Modified: Wed, 23 Jun 2021 11:53:09 GMT  
		Size: 17.5 MB (17481801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56adf5c38075c402f8bf5f30dee3d2dd1d1f5c327b12641f29af33f5ba950a`  
		Last Modified: Wed, 23 Jun 2021 11:52:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bf5eeb5d260e70dda8e6cf6bf12b837eca9e5650117ad4e659861a5ecc31f5`  
		Last Modified: Wed, 23 Jun 2021 11:52:58 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2221de5e1d4ac2ed19abe7d79067a8c6a7038c2cc7ae45c5999dd562e7190d2`  
		Last Modified: Mon, 28 Jun 2021 23:33:44 GMT  
		Size: 11.1 MB (11105159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2a4cb942b2a12ed76d0ffcdf9fe07302abe1bb6453bff985f8878f03f1a821`  
		Last Modified: Mon, 28 Jun 2021 23:33:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbf5fb3e8cc8336a4d22a36d92df0136aa05fac7971b2288300790ab1b0d5a2`  
		Last Modified: Mon, 28 Jun 2021 23:33:47 GMT  
		Size: 12.5 MB (12503351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca1d340fd824cb8a87fac542cef12bd7a64e63b61bea77ede0010b89bbe3064`  
		Last Modified: Mon, 28 Jun 2021 23:33:37 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd80dfa600ea572cc6a3baf88d684f4d88510485b4797f8a2fa669c6dd75902`  
		Last Modified: Mon, 28 Jun 2021 23:33:37 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa1b9865710f236a68f634b06ef4029bbfe36b720ed3a6608d53d0e13d9ff0d`  
		Last Modified: Mon, 28 Jun 2021 23:33:37 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache` - linux; arm64 variant v8

```console
$ docker pull php@sha256:97e58db9c7203548759864b8acee9c8b2ab692254fe2abbb6d07ecf254117e19
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139887655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b36c76b2d2465491d02881b9ab1bbeac34a8e367a16cbd20b711a3f56bb641b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:48:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 08:48:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 08:48:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:48:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 08:48:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 08:53:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 08:53:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 08:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 08:53:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 08:53:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:53:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 09:16:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Jun 2021 09:16:09 GMT
ENV PHP_VERSION=8.0.7
# Wed, 23 Jun 2021 09:16:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Wed, 23 Jun 2021 09:16:10 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Mon, 28 Jun 2021 20:35:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 20:35:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:38:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 20:38:18 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:38:19 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 20:38:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 20:38:20 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 20:38:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:38:20 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 20:38:20 GMT
EXPOSE 80
# Mon, 28 Jun 2021 20:38:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce6585fd70baac65871dafb05b7f408940165f163c30d7e0f9ec3518709e908`  
		Last Modified: Wed, 23 Jun 2021 10:25:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab6c01ccebb7fc71b44dfe6966672e34b47ea5e22d53a11e4481e76243cd44b`  
		Last Modified: Wed, 23 Jun 2021 10:25:24 GMT  
		Size: 70.4 MB (70356352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ed9f96098643713fabf62c17f792254db16c6623e3cec0b4a4ea602af2e742`  
		Last Modified: Wed, 23 Jun 2021 10:25:12 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6852e08c882a542c19980b469e16cebe09c20c56cb6a883fe46d7fa71c77a5bf`  
		Last Modified: Wed, 23 Jun 2021 10:26:10 GMT  
		Size: 18.6 MB (18579813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650d5012e5fa16b3bcc69043ccc3b45a8e75bd3651354579204af7abe7ae4eae`  
		Last Modified: Wed, 23 Jun 2021 10:26:01 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390447f485b4746ca973bb40b4a5ef8edc132fc2fd3b4c1e3681b22c5fa1ca47`  
		Last Modified: Wed, 23 Jun 2021 10:26:01 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70d78575cb6260a4420a960c672f5958ed5f4adc7096e4ac775db7cf190a1b6`  
		Last Modified: Mon, 28 Jun 2021 22:56:39 GMT  
		Size: 11.1 MB (11105822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecbecf926b49d8ea92949301b7ebaba8695e893cc9aa239e5123f7851fbc950`  
		Last Modified: Mon, 28 Jun 2021 22:56:35 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:333b2226f8d700c8b54d76fc11b5f83939b4b3ce4d29d7b25d3c6667d5f74880`  
		Last Modified: Mon, 28 Jun 2021 22:56:38 GMT  
		Size: 13.9 MB (13925286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6075fbe309a96d0ee78d0b71999a7b4f456bf59bcc3ffad0d493fddf04c7875c`  
		Last Modified: Mon, 28 Jun 2021 22:56:35 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63c08d2270685294b8f7b4129e42ed72457963378134eeff4bd3056f06afc06`  
		Last Modified: Mon, 28 Jun 2021 22:56:35 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eabbfe4ac4a2193e5001eeafc5f1f2e3588fcab881994afd98b2bcecfbdd1ac`  
		Last Modified: Mon, 28 Jun 2021 22:56:35 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache` - linux; 386

```console
$ docker pull php@sha256:f6b88df0a9deba1b5148d7af3ca5e490451f4f5a8529729c47315a8047418a05
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.0 MB (154048245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eb0ca100961be09bfee2c794f466a5d821d64a8914abaa46d093bbf0da8d987`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 09:40:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 09:40:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 09:40:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 09:40:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 09:40:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 09:49:27 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 09:49:27 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 09:49:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 09:49:44 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 09:49:46 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 09:49:46 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 10:26:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Jun 2021 10:26:09 GMT
ENV PHP_VERSION=8.0.7
# Wed, 23 Jun 2021 10:26:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Wed, 23 Jun 2021 10:26:10 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Mon, 28 Jun 2021 21:05:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 21:05:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:12:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 21:12:25 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:12:27 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 21:12:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 21:12:27 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 21:12:28 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:12:28 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 21:12:29 GMT
EXPOSE 80
# Mon, 28 Jun 2021 21:12:29 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851ded1e6779ac12f2623fa13c3d156987e0e3748e10171438e042c4a18cada8`  
		Last Modified: Wed, 23 Jun 2021 12:27:42 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9108f1298d19c1c39f13396485b32141017e3d97dcc7093d43854940c92b6c`  
		Last Modified: Wed, 23 Jun 2021 12:28:14 GMT  
		Size: 81.2 MB (81230041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a8cc691843125fa492ce4109092746e47e36d222eceef5b59dd10271176374`  
		Last Modified: Wed, 23 Jun 2021 12:27:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce571916f9fd350c507c0b0f4ba7db9c473cb95da721dfeab5acd167c05197`  
		Last Modified: Wed, 23 Jun 2021 12:29:05 GMT  
		Size: 19.1 MB (19115037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abad9c9b3f342c41ff79e0b1832309d795f17e4aaafd51a979891c9c747684c`  
		Last Modified: Wed, 23 Jun 2021 12:28:58 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ecb5db768b6cdd9c3b371c253bc49fc82700b113499943217799b6cf74aab9`  
		Last Modified: Wed, 23 Jun 2021 12:28:58 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b1b48ad1ed7d2d40025adbd0820ec703f5c6ffbb451dcec25b353658a50866`  
		Last Modified: Tue, 29 Jun 2021 01:21:36 GMT  
		Size: 11.1 MB (11106458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:254c66a2fdd0ff987d26738e9795291949d71119c2de9c8637b04f933ac60823`  
		Last Modified: Tue, 29 Jun 2021 01:21:30 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1810198f1fe2537f6d088552984225e1996ffb15d82282fc1126b490304b43c2`  
		Last Modified: Tue, 29 Jun 2021 01:21:39 GMT  
		Size: 14.8 MB (14793905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60076d48e896433197581e5e62e4ab6978bd3302b7ec5d747e921a184c2814d6`  
		Last Modified: Tue, 29 Jun 2021 01:21:30 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb76d476f81c892f96199daa4e7e69b4649627ce946a6f39f1fcaa83f35400f1`  
		Last Modified: Tue, 29 Jun 2021 01:21:30 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c4437b4bdee67fadd2b81b1dd818914bd64cd093beee6c1ce85c9081c3651e`  
		Last Modified: Tue, 29 Jun 2021 01:21:30 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache` - linux; mips64le

```console
$ docker pull php@sha256:8a226b270dd6a8e8931ddbc30e29ae24a5270e51497d76e2c35ade2a29b02ce5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130369217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96cea32aa18bd9777a3e16228aa04161aed5d2f06158380a15544296c3895c70`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:29 GMT
ADD file:ca8422268fc66c67d19fd3a33a14a9bd6280ef21404677767ffd561a8ecf6724 in / 
# Wed, 23 Jun 2021 00:09:30 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 02:39:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 02:39:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 02:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 02:40:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 02:40:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 02:52:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 02:52:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 02:53:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 02:53:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 02:53:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 02:53:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 03:45:43 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Jun 2021 03:45:43 GMT
ENV PHP_VERSION=8.0.7
# Wed, 23 Jun 2021 03:45:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Wed, 23 Jun 2021 03:45:43 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Mon, 28 Jun 2021 20:12:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 20:12:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:25:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 20:25:03 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:25:05 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 20:25:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 20:25:05 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 20:25:06 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 20:25:06 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 20:25:06 GMT
EXPOSE 80
# Mon, 28 Jun 2021 20:25:07 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4b9d1870c33c63bfde89c401b4af9582fbbff99d4036171a7a456706bf805d6d`  
		Last Modified: Wed, 23 Jun 2021 00:15:49 GMT  
		Size: 25.8 MB (25812890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c90d345f251f9a0ec80cf41b5f35febb67c1c989281d9e68b2aeefee1c00143`  
		Last Modified: Wed, 23 Jun 2021 05:55:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf25841fee636dffd0610ecca37bade0d96a921f21482eda088538659d329a`  
		Last Modified: Wed, 23 Jun 2021 05:55:57 GMT  
		Size: 61.4 MB (61404106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b88a019f1da6587ce2665903b08be861bc197f91d09bfbfb6e62a368de4a231`  
		Last Modified: Wed, 23 Jun 2021 05:55:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e208dcf88dd78c21b0c19c351345924790c3caa4bbca1580e2e289d738c874ab`  
		Last Modified: Wed, 23 Jun 2021 05:56:42 GMT  
		Size: 18.6 MB (18611849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe3845bbf14eccd94071a1ab8d234fe05503b03c7d92b53ed1643a1ca33d9a4`  
		Last Modified: Wed, 23 Jun 2021 05:56:29 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec3aa526d170c9dd2f45b8bd19f5f8f080e143f30ba8431c0e6d9105ec4d0c`  
		Last Modified: Wed, 23 Jun 2021 05:56:29 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2675a0957aaa767d1ce054e74c7a8a0cf86f4be8669e81447a176d1b0df54f88`  
		Last Modified: Mon, 28 Jun 2021 22:25:29 GMT  
		Size: 11.1 MB (11104259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab31d7acb7ec675c50e0f913419bcd93d29027de26291f0a8fb5ccc07934b68`  
		Last Modified: Mon, 28 Jun 2021 22:25:23 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d465a3ee3e424bd136ec763ecc6d97eebd39d90919ff39ea357e01be7c7b92e`  
		Last Modified: Mon, 28 Jun 2021 22:25:35 GMT  
		Size: 13.4 MB (13430816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3222ccd29285c6fbf8c5b16a93d11ec3c6daeca9960b60331da033fb0274c06`  
		Last Modified: Mon, 28 Jun 2021 22:25:23 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4e0c04d98b28365b154429181b09f7d8d397fb4e6e2d9fe18937b282ebfb4f`  
		Last Modified: Mon, 28 Jun 2021 22:25:23 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65df6a89364cc499768fca8b192a155d8405c0f0394015299b10a360217db455`  
		Last Modified: Mon, 28 Jun 2021 22:25:23 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache` - linux; ppc64le

```console
$ docker pull php@sha256:09d6e01b3a0dc9989e99dddeaec44d10b7ed365909fa467e3211eda25675a301
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (158987035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff5b0e84d15d385235f26e31c856488becce062b5dd4064a0add6e305d835a7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Sat, 26 Jun 2021 04:04:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 26 Jun 2021 04:04:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 26 Jun 2021 04:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Jun 2021 04:09:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 26 Jun 2021 04:09:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 26 Jun 2021 04:24:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 26 Jun 2021 04:24:28 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 26 Jun 2021 04:26:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 26 Jun 2021 04:26:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 26 Jun 2021 04:26:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 26 Jun 2021 04:26:47 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 26 Jun 2021 04:26:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 26 Jun 2021 04:26:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 04:27:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 04:27:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 26 Jun 2021 05:48:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 26 Jun 2021 05:48:46 GMT
ENV PHP_VERSION=8.0.7
# Sat, 26 Jun 2021 05:48:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Sat, 26 Jun 2021 05:48:57 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Mon, 28 Jun 2021 21:07:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 21:07:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:16:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 21:17:02 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:17:17 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 21:17:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 21:17:27 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 21:17:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:17:34 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 21:17:38 GMT
EXPOSE 80
# Mon, 28 Jun 2021 21:17:45 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bede12a66c305ed12d280c6b7a6022061a73d9568433f643b06ec9893f790c0`  
		Last Modified: Sat, 26 Jun 2021 09:01:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b569ead47e80d494e6f64ea9e5b97bcc6a4d42355effc0aedead32f63c7ba733`  
		Last Modified: Sat, 26 Jun 2021 09:03:27 GMT  
		Size: 82.3 MB (82291015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b0e4b30eb84311f540a9331dfc8db99c35e188d1fc36e8862ed80fd320c431`  
		Last Modified: Sat, 26 Jun 2021 09:01:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0be226e932ae202655cabfbdf039de068fd0668bc10270960d28e04010caf9d`  
		Last Modified: Sat, 26 Jun 2021 09:04:48 GMT  
		Size: 19.8 MB (19818544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a6a8c2dc286478f193e642b39db64063501e03463223f793d17bf4b4d548a4`  
		Last Modified: Sat, 26 Jun 2021 09:04:35 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d8e7e98a0047f2938ddec0785e0b8a93b3b086bfd03f29c6d1a903ec5bfd69`  
		Last Modified: Sat, 26 Jun 2021 09:04:35 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad5885b7beefd8b4178b76dad44c002529b9735739f66ff40e630995a9190b0`  
		Last Modified: Tue, 29 Jun 2021 00:13:03 GMT  
		Size: 11.1 MB (11107262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d301873d166fd2a0480949a22f0482ebc24cb81ec0d58753cfe982cc66101f2a`  
		Last Modified: Tue, 29 Jun 2021 00:12:57 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8be4538e713490a1e91384108c5118cdab74dbb1aea3cc111bf547ca764d863`  
		Last Modified: Tue, 29 Jun 2021 00:13:01 GMT  
		Size: 15.2 MB (15211177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c10a5b0d4da5e10026769ab6350539d5d0cb7b353f1c3a779061aa8e9ac9d68`  
		Last Modified: Tue, 29 Jun 2021 00:12:57 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d76c186456651f3549d6fbc41a661534d567f5a2c589312557f6b734eff8d6`  
		Last Modified: Tue, 29 Jun 2021 00:12:57 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d93504aa55c47673a7596f10ae36917ba31f459fe704504a5ff71b1e4aaaa0`  
		Last Modified: Tue, 29 Jun 2021 00:12:57 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache` - linux; s390x

```console
$ docker pull php@sha256:e90a4f6c49c32b828b2ae41a0a80f4131e833893a9eeffc5efa7e396be430eee
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133467452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afcf1bcfa2e45bb08209d4b1010ab7fca4526c04ee5739c1739ea7845035b33d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:28 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Tue, 22 Jun 2021 23:42:29 GMT
CMD ["bash"]
# Sat, 26 Jun 2021 00:09:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 26 Jun 2021 00:09:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 26 Jun 2021 00:10:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Jun 2021 00:10:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 26 Jun 2021 00:10:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 26 Jun 2021 00:13:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 26 Jun 2021 00:13:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 26 Jun 2021 00:14:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 26 Jun 2021 00:14:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 26 Jun 2021 00:14:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 26 Jun 2021 00:14:09 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 26 Jun 2021 00:40:37 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 26 Jun 2021 00:40:37 GMT
ENV PHP_VERSION=8.0.7
# Sat, 26 Jun 2021 00:40:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Sat, 26 Jun 2021 00:40:37 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Mon, 28 Jun 2021 19:19:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 19:19:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:23:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 19:23:06 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:23:07 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 19:23:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 19:23:08 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 19:23:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:23:09 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 19:23:09 GMT
EXPOSE 80
# Mon, 28 Jun 2021 19:23:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61297595675dd5f94c60485ec6670e0d45420c73a569aebae232822f3805f5f4`  
		Last Modified: Sat, 26 Jun 2021 02:18:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ab5f68c432394e6815ad9808418b4300224b46b5898a0f90a1fedbfdf9ca7f`  
		Last Modified: Sat, 26 Jun 2021 02:18:46 GMT  
		Size: 64.7 MB (64710315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6def165c1dbb7cd43c8e70e00b2ec5aa53eae70056635c2ff93bdaf25ec061ef`  
		Last Modified: Sat, 26 Jun 2021 02:18:36 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b3e7236868c26c00547364caef50791abcea8d5a62d4fac4ff00f1acf28308`  
		Last Modified: Sat, 26 Jun 2021 02:19:14 GMT  
		Size: 18.5 MB (18525085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae502a4e5daabc91e5f674004c64396c939ee72f05af0b913531fd51c79a37e`  
		Last Modified: Sat, 26 Jun 2021 02:19:11 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c27e0c3d22fb08edda2488324e9cbcd02f8ff31f5bad766bdd1470e2ea7048`  
		Last Modified: Sat, 26 Jun 2021 02:19:11 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f655ce624d975e487b4e2974123f62d8ae234d29fe586d786ba573df0b014bc`  
		Last Modified: Mon, 28 Jun 2021 21:06:20 GMT  
		Size: 11.1 MB (11105527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08d906ae709098b209ac6b3e8080d276444249fceb359cf6cb62767d65975a0`  
		Last Modified: Mon, 28 Jun 2021 21:06:17 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8fea9b06e9b2a6a70c2c7749e8945dea110b0eea427b912fc779ca5bcc1bff`  
		Last Modified: Mon, 28 Jun 2021 21:06:20 GMT  
		Size: 13.4 MB (13360418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af44f1e269e1dde4a87a73e1c73a34767add0d9fbf3faa03b0735a173484cb5`  
		Last Modified: Mon, 28 Jun 2021 21:06:17 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839fdb8453357522768e684c10f9d96c680c28e78d451620f7f9ea05e4a9aa1d`  
		Last Modified: Mon, 28 Jun 2021 21:06:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee7b25dd6a0565de10d2e14fd297b344ee8f4e9344625c48c1aaecc2cf07fb3`  
		Last Modified: Mon, 28 Jun 2021 21:06:17 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
