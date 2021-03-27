## `yourls:latest`

```console
$ docker pull yourls@sha256:595eaa42672d60ae4f0b260419a350cb08ee3405b0593744d123853ca232cc67
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

### `yourls:latest` - linux; amd64

```console
$ docker pull yourls@sha256:fcbac80d60011fec10bf86d8ffe2f8cdf1553afb9a3c4a86888c4e30ac882fc7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.3 MB (151304449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd27e84b5446e581f8115b7a38ba15aac6a9641e43b7a88ceac83fb287eab3e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:40 GMT
ADD file:3c32f1cd03198e141dd233a7ffd13444157d4150ad917d548f3ee9bf5953ce22 in / 
# Fri, 12 Mar 2021 02:20:41 GMT
CMD ["bash"]
# Sat, 13 Mar 2021 02:15:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 13 Mar 2021 02:15:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 13 Mar 2021 02:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 13 Mar 2021 02:16:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Mar 2021 02:16:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Mar 2021 02:22:36 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 13 Mar 2021 02:22:36 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 13 Mar 2021 02:22:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 13 Mar 2021 02:22:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 13 Mar 2021 02:22:47 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 13 Mar 2021 02:22:47 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 13 Mar 2021 02:22:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 13 Mar 2021 02:22:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Mar 2021 02:22:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Mar 2021 02:22:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Mar 2021 02:22:48 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 13 Mar 2021 02:22:49 GMT
ENV PHP_VERSION=8.0.3
# Sat, 13 Mar 2021 02:22:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Sat, 13 Mar 2021 02:22:49 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Sat, 13 Mar 2021 02:22:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 13 Mar 2021 02:22:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Mar 2021 02:28:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Mar 2021 02:28:32 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Sat, 13 Mar 2021 02:28:33 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Mar 2021 02:28:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Mar 2021 02:28:34 GMT
STOPSIGNAL SIGWINCH
# Sat, 13 Mar 2021 02:28:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 13 Mar 2021 02:28:34 GMT
WORKDIR /var/www/html
# Sat, 13 Mar 2021 02:28:34 GMT
EXPOSE 80
# Sat, 13 Mar 2021 02:28:34 GMT
CMD ["apache2-foreground"]
# Sat, 13 Mar 2021 17:39:58 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 13 Mar 2021 17:39:59 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 13 Mar 2021 17:40:00 GMT
RUN a2enmod rewrite expires
# Sat, 13 Mar 2021 17:40:00 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 13 Mar 2021 17:40:00 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 13 Mar 2021 17:40:03 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 13 Mar 2021 17:40:03 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 13 Mar 2021 17:40:03 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 13 Mar 2021 17:40:03 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Sat, 13 Mar 2021 17:40:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 17:40:04 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6f28985ad1843afd6fd4fe0b42a30bfab63c27d302362e7341e3316e8ba25ced`  
		Last Modified: Fri, 12 Mar 2021 02:26:11 GMT  
		Size: 27.1 MB (27101001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db883aae18bc008a4ef1e00647660bd700053b7a3f00c26d613533d22e4945d8`  
		Last Modified: Sat, 13 Mar 2021 03:42:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffae70ea03a956afbb3c504bd109810da75045c9c96c03fbb36669922ffbc161`  
		Last Modified: Sat, 13 Mar 2021 03:42:20 GMT  
		Size: 76.7 MB (76678257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8027612378a55bb01d4b8d62d26e17252295f14b45039c08331829b3c8629d`  
		Last Modified: Sat, 13 Mar 2021 03:42:06 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec32e53dce528cbba7ea7aceb0366268f9160c7e39f67e95b36f1361bb30453`  
		Last Modified: Sat, 13 Mar 2021 03:43:18 GMT  
		Size: 18.7 MB (18679185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb74037bf77523cf411601ba1a154818d3f7ca9d747f8175a17122f3c4a318c`  
		Last Modified: Sat, 13 Mar 2021 03:43:15 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feda0fbd85b12ead20ee1fdd6019bbb11947c660c98211f8a2b26346fc23d0b5`  
		Last Modified: Sat, 13 Mar 2021 03:43:14 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cbfcace66f7a4d336c924d264830c47768ee1390afc9cbeebf280167d6a09f`  
		Last Modified: Sat, 13 Mar 2021 03:43:15 GMT  
		Size: 11.1 MB (11093891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e59842632d01989622c9f04e31df11d396a938587397be722a5509b2b5470e`  
		Last Modified: Sat, 13 Mar 2021 03:43:12 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a29d8ab032cfc9a99e82ccc0dfbe8ad24a40a589cdeb379b6a4f89181311fc0`  
		Last Modified: Sat, 13 Mar 2021 03:43:15 GMT  
		Size: 14.5 MB (14480781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5435aacb32555bfcb8e5df1f90b7c7fb698a9d7e3b59fecc5c043bc29fb6a6b7`  
		Last Modified: Sat, 13 Mar 2021 03:43:12 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f9bba5897a43f5984cd1094ac605c99870ab11be7ef5559741b0223bbd599e`  
		Last Modified: Sat, 13 Mar 2021 03:43:12 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c89fe480edad8140f2246cd98bfadccbca768dab2da0102bff4516256fecdf4`  
		Last Modified: Sat, 13 Mar 2021 03:43:12 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922930eb56516d9262d677ff0ba069223f63be296cf2eb07022471754a9acce`  
		Last Modified: Sat, 13 Mar 2021 17:41:31 GMT  
		Size: 689.6 KB (689572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea87d8b7610d19558ecc59acb75c60714fc2215d4d5cb9a698ecfd3f6700d8c`  
		Last Modified: Sat, 13 Mar 2021 17:41:32 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75615481f541444313cf7b60027e04d2b8b03808911d081ceba01d0d6aed0c4`  
		Last Modified: Sat, 13 Mar 2021 17:41:29 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9866af44a52bee8ece6fd7d3e0f74594e9756b1d225c2944600b35871a32a58`  
		Last Modified: Sat, 13 Mar 2021 17:41:29 GMT  
		Size: 2.6 MB (2572146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e8e709a57cd0edef78c2dd4c30a30b29820b1e6d62176d9f7f7717ece5012d`  
		Last Modified: Sat, 13 Mar 2021 17:41:29 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792dc0201db067ac03e58d6a3594b57c538811ea6111ed4747c5d3a79f6bedb1`  
		Last Modified: Sat, 13 Mar 2021 17:41:29 GMT  
		Size: 2.0 KB (2041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a61e93ab4b9789ecd57d9af9e09e6b501f337f1bd7cde6381c577596a127330`  
		Last Modified: Sat, 13 Mar 2021 17:41:29 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; arm variant v5

```console
$ docker pull yourls@sha256:3ac7e19ee0aed65a8bfbc1786eb1c755ea8bb57b072ac74678df2ae52d094ff8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.9 MB (128900579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2f684155b8a412bc86630b5cc30f66381dd764919caa99d61765ff74565be24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:46 GMT
ADD file:3dd25698bf1578e8580b2f437a2199bfc3b1818480b874d73622357e955a091f in / 
# Fri, 26 Mar 2021 07:51:48 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 12:48:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 26 Mar 2021 12:48:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 26 Mar 2021 12:49:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 12:49:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 26 Mar 2021 12:50:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 26 Mar 2021 12:54:30 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 26 Mar 2021 12:54:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 26 Mar 2021 12:55:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 26 Mar 2021 12:55:10 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 26 Mar 2021 12:55:14 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 26 Mar 2021 12:55:14 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 26 Mar 2021 12:55:16 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 26 Mar 2021 12:55:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 12:55:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 12:55:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Mar 2021 12:55:23 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 26 Mar 2021 12:55:26 GMT
ENV PHP_VERSION=8.0.3
# Fri, 26 Mar 2021 12:55:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 26 Mar 2021 12:55:32 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 26 Mar 2021 12:55:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 26 Mar 2021 12:55:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:59:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 12:59:41 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:59:44 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 12:59:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 12:59:45 GMT
STOPSIGNAL SIGWINCH
# Fri, 26 Mar 2021 12:59:46 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:59:47 GMT
WORKDIR /var/www/html
# Fri, 26 Mar 2021 12:59:48 GMT
EXPOSE 80
# Fri, 26 Mar 2021 12:59:49 GMT
CMD ["apache2-foreground"]
# Fri, 26 Mar 2021 23:42:08 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 26 Mar 2021 23:42:11 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 26 Mar 2021 23:42:15 GMT
RUN a2enmod rewrite expires
# Fri, 26 Mar 2021 23:42:16 GMT
ENV YOURLS_VERSION=1.8.1
# Fri, 26 Mar 2021 23:42:17 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Fri, 26 Mar 2021 23:42:22 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 26 Mar 2021 23:42:24 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 23:42:24 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Fri, 26 Mar 2021 23:42:25 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 26 Mar 2021 23:42:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 23:42:27 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:997e59852ec0e1a23e4a179db14793947d60390c392ce15abc0f811e797c49ca`  
		Last Modified: Fri, 26 Mar 2021 08:00:22 GMT  
		Size: 24.8 MB (24846159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4f992f1746b0ab08c849afc6fcbe26e6527dba7d8ea30442d6fa1947df30a9`  
		Last Modified: Fri, 26 Mar 2021 14:06:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bb1b488e61bd718851af1ed0f5528cd36d27e57974287f9de9a240a8fbe92c`  
		Last Modified: Fri, 26 Mar 2021 14:07:17 GMT  
		Size: 58.8 MB (58815829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d255b28d593bbda7f415959ea6754f02bd0faad03b926ce0a7aadb8d0f8a138c`  
		Last Modified: Fri, 26 Mar 2021 14:06:36 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27590a9c336cc028096a0baad977a98b37633b170c69f77ff725bcf69dd3463c`  
		Last Modified: Fri, 26 Mar 2021 14:08:12 GMT  
		Size: 18.0 MB (18026328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a048ea915c0e87dcac98cbdceab3e15d8dbf286c70e72e213ac51b9410972001`  
		Last Modified: Fri, 26 Mar 2021 14:08:02 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599c57a01ac5fd675c85c9e92145408192631acb0055508e233841b68ddd90ec`  
		Last Modified: Fri, 26 Mar 2021 14:08:02 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870827b1d700fd48ec2cb0bd02c5e3d621c8c0eaa376dd2f46b5e9dfdaa626cd`  
		Last Modified: Fri, 26 Mar 2021 14:08:01 GMT  
		Size: 11.1 MB (11092105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bf57f0beff004435ae3160de143039d2b8d64fad0a6dbfc8552d442ee26b58`  
		Last Modified: Fri, 26 Mar 2021 14:08:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3415d166555f3181b1e7211b8e97ea41ac4d0796bb197907d6510ee6ce7655f1`  
		Last Modified: Fri, 26 Mar 2021 14:08:05 GMT  
		Size: 13.2 MB (13198376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273f8225d27735cd279337039db9141c168b43481b0e686ad09ea4a9481f2a12`  
		Last Modified: Fri, 26 Mar 2021 14:08:00 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fad3691911db1f59139952a773b449acd795c6e024417174ecac03791c9cd71`  
		Last Modified: Fri, 26 Mar 2021 14:08:00 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4818947057c9d9f3bafd1b35ac70143bd8ac5ca0538b7b7c1bddf69964a0f2c3`  
		Last Modified: Fri, 26 Mar 2021 14:07:57 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51377abd19818a6658b8e80a5e0520423d91f6a9af209e6b348b16b6aab90f32`  
		Last Modified: Fri, 26 Mar 2021 23:44:03 GMT  
		Size: 340.0 KB (339985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747f820e48d3fced7f8d0e683cd06e8627f29d56d650ab6d6556e179a0daeb41`  
		Last Modified: Fri, 26 Mar 2021 23:44:03 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3832b211882666118d175a1a32b25c60332d3efda803fa4e2979937efc477d`  
		Last Modified: Fri, 26 Mar 2021 23:44:01 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1830953f649ef4d57146e8cdebeae9fbc8f6af34e68c29450b806e06aed37bb7`  
		Last Modified: Fri, 26 Mar 2021 23:44:03 GMT  
		Size: 2.6 MB (2572149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b95989ac2aecc0afe19d1238f52e94c0871aa15da4664999e944cccea44b5b`  
		Last Modified: Fri, 26 Mar 2021 23:44:02 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8601963e48cb2985d64bf768de55aa55c1cbe939dfec667f2f3f4e9a153ffad3`  
		Last Modified: Fri, 26 Mar 2021 23:44:02 GMT  
		Size: 2.0 KB (2041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd3ea7085888b60275748eef60b27053dfc99dc7cb2c3c3863330a9806b3f62`  
		Last Modified: Fri, 26 Mar 2021 23:44:01 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; arm variant v7

```console
$ docker pull yourls@sha256:494f297b8b87d26467e608d1c5a0f506edbf73785791af7541984614abfe173c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126180063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1476dbfcbcba05b7978a1dc2f4f780674b6f224fe35727b9ce74ceccc34fcbf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 12 Mar 2021 02:00:12 GMT
ADD file:123da9848f87c8ed4c5122a104b8650564c09767725916f822def7b645a019f1 in / 
# Fri, 12 Mar 2021 02:00:14 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 08:58:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 12 Mar 2021 08:58:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 12 Mar 2021 08:59:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 08:59:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Mar 2021 08:59:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Mar 2021 09:03:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 12 Mar 2021 09:03:10 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 12 Mar 2021 09:03:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 12 Mar 2021 09:03:36 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 12 Mar 2021 09:03:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 12 Mar 2021 09:03:39 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 12 Mar 2021 09:03:43 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 12 Mar 2021 09:03:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 09:03:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 09:03:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Mar 2021 09:03:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 12 Mar 2021 09:03:50 GMT
ENV PHP_VERSION=8.0.3
# Fri, 12 Mar 2021 09:03:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 12 Mar 2021 09:03:52 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 12 Mar 2021 09:04:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 12 Mar 2021 09:04:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Mar 2021 09:07:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Mar 2021 09:07:04 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 12 Mar 2021 09:07:06 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Mar 2021 09:07:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Mar 2021 09:07:07 GMT
STOPSIGNAL SIGWINCH
# Fri, 12 Mar 2021 09:07:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 12 Mar 2021 09:07:09 GMT
WORKDIR /var/www/html
# Fri, 12 Mar 2021 09:07:09 GMT
EXPOSE 80
# Fri, 12 Mar 2021 09:07:10 GMT
CMD ["apache2-foreground"]
# Sat, 13 Mar 2021 03:20:14 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 13 Mar 2021 03:20:17 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 13 Mar 2021 03:20:21 GMT
RUN a2enmod rewrite expires
# Sat, 13 Mar 2021 03:20:22 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 13 Mar 2021 03:20:24 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 13 Mar 2021 03:20:29 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 13 Mar 2021 03:20:30 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 13 Mar 2021 03:20:31 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 13 Mar 2021 03:20:32 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Sat, 13 Mar 2021 03:20:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 03:20:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e12d26f75fe8b7fd14712965ff5178762227d07d2151bb35fa21105ddfc4a14a`  
		Last Modified: Fri, 12 Mar 2021 02:10:28 GMT  
		Size: 22.7 MB (22709467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97de6173b7f7c8cb90cb7c3294b87fc1eee1e42223b91620341128b5119594a`  
		Last Modified: Fri, 12 Mar 2021 10:02:21 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2b82824d7becee8957d19b795e585f7a5154d758780f636358ad5dfc638124`  
		Last Modified: Fri, 12 Mar 2021 10:02:40 GMT  
		Size: 59.5 MB (59513006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732ffe8153f5415ad0deaf603c13ca07696188324be500902aa2d60abf5f657b`  
		Last Modified: Fri, 12 Mar 2021 10:02:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38df2bb5f9338849fe8cd651740bfa74e601be8674ef98a4530a9fdca80ff99d`  
		Last Modified: Fri, 12 Mar 2021 10:03:17 GMT  
		Size: 17.5 MB (17481742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1f17d694ace61a63fe6312fe0956b53a64c151195691b78350348e92c21934`  
		Last Modified: Fri, 12 Mar 2021 10:03:11 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a401a55da75d47e7bff923d871beeddb5f4f58693069e516712ff17d6c6326`  
		Last Modified: Fri, 12 Mar 2021 10:03:15 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ee21e4ff166c21d3ea02cfa1f4d2e2ecf4f54126a15ea130d4cd40d2a6414d`  
		Last Modified: Fri, 12 Mar 2021 10:03:13 GMT  
		Size: 11.1 MB (11092051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6580f45e3fb5a7efd17cc2e91cd8e051f07e9d6c864776f13662c2b82dfe6d27`  
		Last Modified: Fri, 12 Mar 2021 10:03:10 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e413599c2f3a4f4efee14313abb46bb7008e52ffa654f3b2fddcbeaaa23e808`  
		Last Modified: Fri, 12 Mar 2021 10:03:14 GMT  
		Size: 12.5 MB (12495440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6551080d01ab93b7954059d167381b5db8c9cf7126c0f8cb6e7e49a1ae605d94`  
		Last Modified: Fri, 12 Mar 2021 10:03:10 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93742a769d075b2b8bb080b493e8714a50977a01036333f24064f8266736d58f`  
		Last Modified: Fri, 12 Mar 2021 10:03:10 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15327cd65c63630f1ee18fc2523f2ddf5fffd08d28242fe6d9a09ac44f550cfc`  
		Last Modified: Fri, 12 Mar 2021 10:03:10 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f69771f9739a5ca287f91127bfc24e6b58627e1567fd66f79c1adebc29591a0`  
		Last Modified: Sat, 13 Mar 2021 03:22:17 GMT  
		Size: 306.6 KB (306572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0931edf6f0b029d6d5fbe942ca8e5e39c9438f8a9b599a6c085dbcf866d8b099`  
		Last Modified: Sat, 13 Mar 2021 03:22:16 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174537efae4baed3677f3816b05191d59072e22f244dbd3749c4149367cc2744`  
		Last Modified: Sat, 13 Mar 2021 03:22:14 GMT  
		Size: 346.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2355263ddf4f9b4461ceac6e58a2d30fc080c397e7c3e1d789fa5a9f2bd1f9e`  
		Last Modified: Sat, 13 Mar 2021 03:22:16 GMT  
		Size: 2.6 MB (2572151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7a3c2b9a3d5763860231f4dec1b1b3f491eafcd1d59f0f02df12ab0b78741f`  
		Last Modified: Sat, 13 Mar 2021 03:22:14 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab384ebdf36c506873d98db12a4a64779c73029d2d48cf163a8c3ec265cbbf47`  
		Last Modified: Sat, 13 Mar 2021 03:22:14 GMT  
		Size: 2.0 KB (2043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef383c290aa83e9a63a1408092604af3a36f48e91f1b9e06a091a31e098ce8fc`  
		Last Modified: Sat, 13 Mar 2021 03:22:14 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:f56e5afbe42c63ca04497d8a037e751557d028fa2f4b1fc677a92f1adbfc1194
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.7 MB (142734959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc2624b815cba9a75c4eb1fc3bb8d33c071fb5a2d301fa1c561739d58320efe8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:53 GMT
ADD file:6130ddc0a939dd72c0614de4aa77de47aa16fe211274bacb31995aa1a0526164 in / 
# Fri, 12 Mar 2021 01:53:56 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 11:09:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 12 Mar 2021 11:09:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 12 Mar 2021 11:09:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 11:09:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Mar 2021 11:09:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Mar 2021 11:14:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 12 Mar 2021 11:14:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 12 Mar 2021 11:14:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 12 Mar 2021 11:14:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 12 Mar 2021 11:14:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 12 Mar 2021 11:14:28 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 12 Mar 2021 11:14:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 12 Mar 2021 11:14:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 11:14:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 11:14:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Mar 2021 11:14:32 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 12 Mar 2021 11:14:33 GMT
ENV PHP_VERSION=8.0.3
# Fri, 12 Mar 2021 11:14:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 12 Mar 2021 11:14:35 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 12 Mar 2021 11:14:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 12 Mar 2021 11:14:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Mar 2021 11:18:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Mar 2021 11:18:37 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 12 Mar 2021 11:18:40 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Mar 2021 11:18:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Mar 2021 11:18:43 GMT
STOPSIGNAL SIGWINCH
# Fri, 12 Mar 2021 11:18:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 12 Mar 2021 11:18:45 GMT
WORKDIR /var/www/html
# Fri, 12 Mar 2021 11:18:46 GMT
EXPOSE 80
# Fri, 12 Mar 2021 11:18:46 GMT
CMD ["apache2-foreground"]
# Sat, 13 Mar 2021 04:43:47 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 13 Mar 2021 04:43:49 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 13 Mar 2021 04:43:51 GMT
RUN a2enmod rewrite expires
# Sat, 13 Mar 2021 04:43:52 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 13 Mar 2021 04:43:53 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 13 Mar 2021 04:43:56 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 13 Mar 2021 04:43:57 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 13 Mar 2021 04:43:58 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 13 Mar 2021 04:43:59 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Sat, 13 Mar 2021 04:44:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 04:44:01 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:706ee5d0a6b53d9257cbea22d8409fb22c867ab3a001c65f6b8bfd37dace0e58`  
		Last Modified: Fri, 12 Mar 2021 02:01:39 GMT  
		Size: 25.9 MB (25856512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170ce16978fe5d48c07f44f3f3629b803edb31c9a5dabeb7b723d1abadf63ec0`  
		Last Modified: Fri, 12 Mar 2021 12:17:27 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5207eb43926d89dc8c3b70fcdd05040ab06c3bf87b04231bfc61ea95bbddbf79`  
		Last Modified: Fri, 12 Mar 2021 12:17:45 GMT  
		Size: 70.4 MB (70355270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65a8ea3de090ee8a21672a8b8730c898b71122c8207afdbdc1bf86ca40e9f1d`  
		Last Modified: Fri, 12 Mar 2021 12:17:25 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ff200ad58cca751c54b278eedcd37584a3be4228e808c8c018a17ea9348bee`  
		Last Modified: Fri, 12 Mar 2021 12:18:18 GMT  
		Size: 18.6 MB (18579887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a9c44328af7bb11a2d814b999fdc77299886f3e08966d24cf369391d864e15`  
		Last Modified: Fri, 12 Mar 2021 12:18:13 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fce2bf2611e4baa86a937a945a5a2335cc428b434bd55da96e604ae85e19763`  
		Last Modified: Fri, 12 Mar 2021 12:18:12 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f1c8fd3c6c5924617cc052f99fd6b6561c4b3181bcb9539f6fbeb96714386b`  
		Last Modified: Fri, 12 Mar 2021 12:18:17 GMT  
		Size: 11.1 MB (11092771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b50890e8f3880ffed653bd3ad2f04d275fb3bbfdff8c1c0804b22a6876c3ef`  
		Last Modified: Fri, 12 Mar 2021 12:18:11 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a434605cc3cbb7f71baf70c0746933e449614dd11d74f17c28a5740b598530`  
		Last Modified: Fri, 12 Mar 2021 12:18:15 GMT  
		Size: 13.9 MB (13916282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c431f731054dcd7ea2242d6f983c1f2a18b1c971ba1e4ea525d00e3b5179e9`  
		Last Modified: Fri, 12 Mar 2021 12:18:11 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4246f694b9e042ae7ed4d6161c473ba135c5837f3d1294103da83cbf881c4c9d`  
		Last Modified: Fri, 12 Mar 2021 12:18:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79be32c01ac671e1f94f8272e2e0cc90543fae0a49239020631a4860acd48594`  
		Last Modified: Fri, 12 Mar 2021 12:18:12 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af22c8c90137ef2f33a48874b3e3761c2bc9d7de1714ad9cb4e7cfc29cf1af22`  
		Last Modified: Sat, 13 Mar 2021 04:45:46 GMT  
		Size: 352.5 KB (352462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946104b345b45e9114ebedc5231208661f51852df65ecb4349cdc9a2124586df`  
		Last Modified: Sat, 13 Mar 2021 04:45:46 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba5aabb009585f772db8c52ff00a826ff0bccd0417a56d24e941cf2fc2de1f4`  
		Last Modified: Sat, 13 Mar 2021 04:45:44 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c40988a4390c90160a5ab3abe5c7b7ca9e6feb538baf7559b281f6fbf2303987`  
		Last Modified: Sat, 13 Mar 2021 04:45:44 GMT  
		Size: 2.6 MB (2572147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aeb24867697320510b5d5782264b21fe08d426ceb4b7de3e99a5401e41e19b5`  
		Last Modified: Sat, 13 Mar 2021 04:45:43 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc528d25ce48d17770835ddbc8848647d2889d3c7b16cb4c05985ad4cf865cb`  
		Last Modified: Sat, 13 Mar 2021 04:45:44 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6a60c62cd7bb65b0093d46018ab0809fcf64c4a1433d14e814575b4bd0fb4c`  
		Last Modified: Sat, 13 Mar 2021 04:45:43 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; 386

```console
$ docker pull yourls@sha256:541bcb9b8aaf38dec983be664c8b20330cd66ebb84e90f1312c0e62201514ecc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156629142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26a2ecb1f5eabef101246bc71eda3f89ed039d940a31abcbae9e2aa535b777db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 12 Mar 2021 01:44:27 GMT
ADD file:90c103e04bd6fe0f39733cbf8eb2d8845aed3e4fc3fd1e5c3354df69e40aa615 in / 
# Fri, 12 Mar 2021 01:44:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 13:55:26 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 12 Mar 2021 13:55:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 12 Mar 2021 13:55:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 13:55:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Mar 2021 13:55:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Mar 2021 14:00:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 12 Mar 2021 14:00:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 12 Mar 2021 14:00:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 12 Mar 2021 14:00:54 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 12 Mar 2021 14:00:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 12 Mar 2021 14:00:55 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 12 Mar 2021 14:00:56 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 12 Mar 2021 14:00:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 14:00:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 14:00:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Mar 2021 14:00:56 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 12 Mar 2021 14:00:57 GMT
ENV PHP_VERSION=8.0.3
# Fri, 12 Mar 2021 14:00:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 12 Mar 2021 14:00:57 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 12 Mar 2021 14:01:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 12 Mar 2021 14:01:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Mar 2021 14:06:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Mar 2021 14:06:08 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 12 Mar 2021 14:06:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Mar 2021 14:06:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Mar 2021 14:06:10 GMT
STOPSIGNAL SIGWINCH
# Fri, 12 Mar 2021 14:06:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 12 Mar 2021 14:06:10 GMT
WORKDIR /var/www/html
# Fri, 12 Mar 2021 14:06:11 GMT
EXPOSE 80
# Fri, 12 Mar 2021 14:06:11 GMT
CMD ["apache2-foreground"]
# Sat, 13 Mar 2021 04:11:11 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 13 Mar 2021 04:11:12 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 13 Mar 2021 04:11:13 GMT
RUN a2enmod rewrite expires
# Sat, 13 Mar 2021 04:11:13 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 13 Mar 2021 04:11:13 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 13 Mar 2021 04:11:15 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 13 Mar 2021 04:11:15 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 13 Mar 2021 04:11:16 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 13 Mar 2021 04:11:16 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Sat, 13 Mar 2021 04:11:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 04:11:16 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0898aa7472f57f223652846337cf862f142e109d0c039b41886e7f20c345f85e`  
		Last Modified: Fri, 12 Mar 2021 01:52:08 GMT  
		Size: 27.8 MB (27760948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ebe5c00547dff203bc3fc4d74077af7cd9f76c7d8b6e70a1f96df6d23ee131`  
		Last Modified: Fri, 12 Mar 2021 15:25:07 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74690855a3e75dc8fea8a2212b35303aac5a38c1b3da1f70a00f00ebf65b8007`  
		Last Modified: Fri, 12 Mar 2021 15:25:27 GMT  
		Size: 81.2 MB (81229571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e6f0f3985167d1630c0f3f8239a0484c8bc7e65bdc459da1365d6fb45bce7f`  
		Last Modified: Fri, 12 Mar 2021 15:25:06 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20440cb15482f13eb667ca3b369306b16a2561d1ea0d3bfad3f6cdeab022ebb8`  
		Last Modified: Fri, 12 Mar 2021 15:26:47 GMT  
		Size: 19.1 MB (19114965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe3f048018674d839a44a213740c9eb63e205afdf7145a34d19703b3c569208`  
		Last Modified: Fri, 12 Mar 2021 15:26:37 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2005d0d5e4bfc5861ea22e7cae45144a445ab856dc46042d471f23a361e50b`  
		Last Modified: Fri, 12 Mar 2021 15:26:36 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9161e3c020ac83bd264d77c12e833ec093df70ec0de0820aabab5f38270f804b`  
		Last Modified: Fri, 12 Mar 2021 15:26:36 GMT  
		Size: 11.1 MB (11093256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22522e515b45ca5ca6ef4077d439d5e6a413243070986ca0f1630b8bf57f41a5`  
		Last Modified: Fri, 12 Mar 2021 15:26:33 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df16e5c2fb803d695d18879a5825f171a37c87220a1ef2db57442d5401f71357`  
		Last Modified: Fri, 12 Mar 2021 15:26:37 GMT  
		Size: 14.5 MB (14476192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a31675d12e6276072b1fa37aae933fef916e2e068a3a2c3c5f29d259b431c3`  
		Last Modified: Fri, 12 Mar 2021 15:26:32 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12e27e5f755007086eb41c8d11bdbb423d0fe45959d9d69c8e793d58bd03244`  
		Last Modified: Fri, 12 Mar 2021 15:26:35 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be734f9511d2320990353b86eccd446cd1a151cca334363543d91167156741e`  
		Last Modified: Fri, 12 Mar 2021 15:26:34 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0825de74e309fe5a0510e049e7f36e2a05f9ea06440986dead13fc61fd1e5714`  
		Last Modified: Sat, 13 Mar 2021 04:12:51 GMT  
		Size: 372.5 KB (372456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9693d4f41ce0312e09f1f544e806d06d2734ffe070221ca39fa17595c68e940`  
		Last Modified: Sat, 13 Mar 2021 04:12:50 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acca9b769c55992ee9b76c747266981e6f73ae26ca3647c0a6da7d4e437d3136`  
		Last Modified: Sat, 13 Mar 2021 04:12:47 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fc8b5d0a13acdffa647f72c46a783af4b2d006956b4b4570dc409dfa30a322`  
		Last Modified: Sat, 13 Mar 2021 04:12:48 GMT  
		Size: 2.6 MB (2572149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4866ecc07fdfa141ced0eb8994f6cd03daf65648cf4c43cf343ebcbba9f51207`  
		Last Modified: Sat, 13 Mar 2021 04:12:47 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22e6a5fcef398cd53a643f8aebe2f13e6d12e9f55ca49098740a2b94f20cd5d1`  
		Last Modified: Sat, 13 Mar 2021 04:12:48 GMT  
		Size: 2.0 KB (2039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9327de0577c9674e58afeadc4ed58dd4b170d1a232644e0b8827f0c8e98d765`  
		Last Modified: Sat, 13 Mar 2021 04:12:47 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; mips64le

```console
$ docker pull yourls@sha256:cf44a6e5203f5c893d4f183ce0053a01a208f9d98b5087d526c0b249009ae666
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133234636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75a0d236414a6e20beac89094da21ec76f3b51ad58654ecaa0f62413799ceaf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 26 Mar 2021 08:09:56 GMT
ADD file:74d504a9a34f47729165ef4ceedc9f0eaa2e91bfb6a24ebfc3ceed0248267a27 in / 
# Fri, 26 Mar 2021 08:09:57 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 08:46:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 26 Mar 2021 08:46:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 26 Mar 2021 08:46:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 08:46:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 26 Mar 2021 08:47:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 26 Mar 2021 08:59:38 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 26 Mar 2021 08:59:38 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 26 Mar 2021 09:00:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 26 Mar 2021 09:00:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 26 Mar 2021 09:00:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 26 Mar 2021 09:00:08 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 26 Mar 2021 09:00:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 26 Mar 2021 09:00:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 09:00:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 09:00:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Mar 2021 09:00:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 26 Mar 2021 09:00:10 GMT
ENV PHP_VERSION=8.0.3
# Fri, 26 Mar 2021 09:00:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 26 Mar 2021 09:00:11 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 26 Mar 2021 09:00:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 26 Mar 2021 09:00:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:12:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 09:12:42 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:12:44 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 09:12:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 09:12:45 GMT
STOPSIGNAL SIGWINCH
# Fri, 26 Mar 2021 09:12:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 26 Mar 2021 09:12:46 GMT
WORKDIR /var/www/html
# Fri, 26 Mar 2021 09:12:46 GMT
EXPOSE 80
# Fri, 26 Mar 2021 09:12:46 GMT
CMD ["apache2-foreground"]
# Fri, 26 Mar 2021 21:42:01 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 26 Mar 2021 21:42:03 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 26 Mar 2021 21:42:05 GMT
RUN a2enmod rewrite expires
# Fri, 26 Mar 2021 21:42:05 GMT
ENV YOURLS_VERSION=1.8.1
# Fri, 26 Mar 2021 21:42:05 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Fri, 26 Mar 2021 21:42:09 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 26 Mar 2021 21:42:10 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Fri, 26 Mar 2021 21:42:10 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Fri, 26 Mar 2021 21:42:10 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 26 Mar 2021 21:42:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 21:42:11 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5f863e006c40853ec8c23aa5b7a0e95918001f96878fb45770410ac4df51cf88`  
		Last Modified: Fri, 26 Mar 2021 08:16:29 GMT  
		Size: 25.8 MB (25772487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9917ef2e3fa9a9a75c1035ce8562e1089983ed624743c4708c4d2018071f53b6`  
		Last Modified: Fri, 26 Mar 2021 11:00:12 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c039fb3abecd33217b5c88dc3534e112402036ef8e200a3123e52cf68a041b`  
		Last Modified: Fri, 26 Mar 2021 11:01:02 GMT  
		Size: 61.4 MB (61403203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d6086af3e9bd8107de474e634822da995e1488ff71a5b3a04e92b3822df21b`  
		Last Modified: Fri, 26 Mar 2021 11:00:12 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfad885d228afea86ff6e4aa91e2fecc251fa6c54d8269954d8a42fb160a5f`  
		Last Modified: Fri, 26 Mar 2021 11:02:11 GMT  
		Size: 18.6 MB (18611789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04cb2d84817e7bb4f22a6c8d9b3c9bf86a5e916a2ae22d65b41597d90b0afd64`  
		Last Modified: Fri, 26 Mar 2021 11:01:58 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34f7317c10f29ecf082d786e5d30678159d9410a5f914ca157e0ff59540da29`  
		Last Modified: Fri, 26 Mar 2021 11:01:58 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72095dbaee5bec17539d2b67cacd96e3476e400730b686ffa294702c32827eba`  
		Last Modified: Fri, 26 Mar 2021 11:02:08 GMT  
		Size: 11.1 MB (11091301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df04831e9561e14720cf1be9866a62d2d658bd7f82b4edd85e6a7297d99ec4ce`  
		Last Modified: Fri, 26 Mar 2021 11:01:55 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e92c68d95684b6925f425da50cba67bf278c7e176397ac42b869ab212b6f7c1`  
		Last Modified: Fri, 26 Mar 2021 11:02:08 GMT  
		Size: 13.4 MB (13425899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca4eca329340cdad32d9d16a4ba6e9a21661a5b83afc5fc2a9fc5596b917f8e`  
		Last Modified: Fri, 26 Mar 2021 11:01:55 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1472699aa99ec09d23a16f326a2a5badc4853754e376d84dc1fdcb1c33ee4aa4`  
		Last Modified: Fri, 26 Mar 2021 11:01:56 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaf4f779d44752cc4d864139bac4f298a1f9bacb4ea7f0ef09a83db9d3c26eb`  
		Last Modified: Fri, 26 Mar 2021 11:01:55 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39be5c79cd0de31cecfec7688f7b90264cae851af34740994b946c02b923f0d`  
		Last Modified: Fri, 26 Mar 2021 21:44:25 GMT  
		Size: 348.3 KB (348312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1863bca7a20209a68f5efa9f24e759acf9236e49ee1bad842f0b420eedfb5d`  
		Last Modified: Fri, 26 Mar 2021 21:44:25 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d47dc69afbda6fbac035538810271d91940001555f0867c58e81f250bec4065`  
		Last Modified: Fri, 26 Mar 2021 21:44:22 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635addeddc05cd19c393636c079834e62722faee9971ad08c3b52468709f5cde`  
		Last Modified: Fri, 26 Mar 2021 21:44:25 GMT  
		Size: 2.6 MB (2572126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb697fe2e92c1e9b4875ad46dfbfda2f61ab0216da229361bd9154cfc1f3b2a`  
		Last Modified: Fri, 26 Mar 2021 21:44:22 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27d041e3e7c450d95312c1917c55a0382e30b13a2a28b6dcb2bde9736ac189b`  
		Last Modified: Fri, 26 Mar 2021 21:44:22 GMT  
		Size: 2.0 KB (2040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ada988e913dbf06a34d628b40fd919ca0e0151f024e78da4ebb4004f3ce68f`  
		Last Modified: Fri, 26 Mar 2021 21:44:22 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; ppc64le

```console
$ docker pull yourls@sha256:28f6644d32f853c7e4d1761ecd1104c20aafbae056b3455bf7e1a7b088a5d82d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.9 MB (161912340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49c952fb8868937ba1617f4d410f4f5fa96a26dc410b49a8905dbe7af6973231`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 12 Mar 2021 02:32:43 GMT
ADD file:6a0c0cfa71979cf6fdd859dce1e32582f0e55ed382b9e17b77a2001defc2c9db in / 
# Fri, 12 Mar 2021 02:32:50 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 17:34:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 12 Mar 2021 17:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 12 Mar 2021 17:37:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 17:37:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Mar 2021 17:37:46 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Mar 2021 17:45:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 12 Mar 2021 17:45:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 12 Mar 2021 17:46:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 12 Mar 2021 17:46:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 12 Mar 2021 17:47:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 12 Mar 2021 17:47:08 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 12 Mar 2021 17:47:11 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 12 Mar 2021 17:47:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 17:47:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 17:47:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Mar 2021 17:47:26 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 12 Mar 2021 17:47:33 GMT
ENV PHP_VERSION=8.0.3
# Fri, 12 Mar 2021 17:47:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 12 Mar 2021 17:47:43 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 12 Mar 2021 17:48:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 12 Mar 2021 17:48:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:55:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Mar 2021 17:55:13 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:55:25 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Mar 2021 17:55:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Mar 2021 17:55:40 GMT
STOPSIGNAL SIGWINCH
# Fri, 12 Mar 2021 17:55:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 12 Mar 2021 17:55:44 GMT
WORKDIR /var/www/html
# Fri, 12 Mar 2021 17:55:48 GMT
EXPOSE 80
# Fri, 12 Mar 2021 17:55:53 GMT
CMD ["apache2-foreground"]
# Sat, 13 Mar 2021 12:53:37 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 13 Mar 2021 12:53:46 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 13 Mar 2021 12:53:53 GMT
RUN a2enmod rewrite expires
# Sat, 13 Mar 2021 12:53:57 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 13 Mar 2021 12:54:03 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 13 Mar 2021 12:54:16 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 13 Mar 2021 12:54:19 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 13 Mar 2021 12:54:21 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 13 Mar 2021 12:54:23 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Sat, 13 Mar 2021 12:54:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 12:54:32 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1d686056fdac1848f4fd78ba2b335502055ffe98c79619e21d0c2fb7db95257e`  
		Last Modified: Fri, 12 Mar 2021 02:45:35 GMT  
		Size: 30.5 MB (30525728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:994f1c929cf4cdf280602a39a5424c2a98bd1ce0fbb2880c809bb43caa96bee2`  
		Last Modified: Fri, 12 Mar 2021 19:28:26 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f67d778602ea1f65e87b664100468b01997ab3269ca189acff1347986108636`  
		Last Modified: Fri, 12 Mar 2021 19:29:41 GMT  
		Size: 82.3 MB (82289990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7763e63ddfa88dbf082b4847b929463333096d46fce614f628fd8fd64bf702`  
		Last Modified: Fri, 12 Mar 2021 19:28:26 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e3ab6495cdb7bcf3603dd8c5a406e8a3ef98937e940de1bc83b17d4d78b9f7`  
		Last Modified: Fri, 12 Mar 2021 19:30:41 GMT  
		Size: 19.8 MB (19818252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30c4d5d9cf1f635be2d2deead0e2e6a090ef5b14afe4d27a3e50d7e45feebe3`  
		Last Modified: Fri, 12 Mar 2021 19:30:37 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fee7450d93a58e5f56788dba235f3bbd7cca66111dff9a385d2f781e11c30fd`  
		Last Modified: Fri, 12 Mar 2021 19:30:37 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e7a7590c3bc6efc94957d2d75630c15b73633de25e9afcfbbb5da17e4ec24a`  
		Last Modified: Fri, 12 Mar 2021 19:30:38 GMT  
		Size: 11.1 MB (11093863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f20a787a7d5c4b168fc93774152f0d5e9bd8503cff6ed1857ed36dc8a6e145d`  
		Last Modified: Fri, 12 Mar 2021 19:30:34 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59eb6e9833227916a51e0f5938f6073ccedb872945e8c9269ec20db6a415f819`  
		Last Modified: Fri, 12 Mar 2021 19:30:38 GMT  
		Size: 15.2 MB (15201538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275ac1fdbaef42324d932f507806c0a99ec8090f3240b0af64ddac43c6a0711f`  
		Last Modified: Fri, 12 Mar 2021 19:30:34 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd91c4c6b9ee88c2324ee6123edcc060a5d25abbcf33380b49943ff042f29f6`  
		Last Modified: Fri, 12 Mar 2021 19:30:34 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d4d4aef5dd9fa16b83fa7c6c7c8416037564b94689f99afdc80d051a6b9782`  
		Last Modified: Fri, 12 Mar 2021 19:30:34 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85b772c3ce66324a183cbb5e0362ce722ca62b6f4cb9e158c6a63b5aa94d743`  
		Last Modified: Sat, 13 Mar 2021 12:57:01 GMT  
		Size: 401.2 KB (401172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5855daf188bbe52e3347982cd55c23836023a59273abdac5003a2228272914f`  
		Last Modified: Sat, 13 Mar 2021 12:57:00 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffcfd17501254bd49ad8d7ddf5068dc816ffce6631294bc9e3dab7fbda23463`  
		Last Modified: Sat, 13 Mar 2021 12:56:53 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fff18890ed96c7ab74b91c071b25837cd0d5e5dfc69cbff897cc0332383511`  
		Last Modified: Sat, 13 Mar 2021 12:56:53 GMT  
		Size: 2.6 MB (2572148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6ae913422ac17e94c9e3c5b4e6e718f05bf460e2f25e61f644286c6efa2256`  
		Last Modified: Sat, 13 Mar 2021 12:56:53 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafea4278228d299a6befb118cd960917291834ef0c5c28554b6e80b39eb6ce4`  
		Last Modified: Sat, 13 Mar 2021 12:56:53 GMT  
		Size: 2.0 KB (2044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645700eac9f757ac333b1391714d5717690967c67b7a717f367683e1ed8f4119`  
		Last Modified: Sat, 13 Mar 2021 12:56:53 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; s390x

```console
$ docker pull yourls@sha256:e9190f83a21f2221a7cb2b9d548dfbdd65335523d9fadba7a1b7b82fa10f2488
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136325246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc720b7c446887cd321afc4951c76bd56b24b5e6d94412e56617f6abcc21ed6c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 12 Mar 2021 01:46:04 GMT
ADD file:afec039adf230a9186a38b57eed85262696f8d178ac649a445657066f16fe806 in / 
# Fri, 12 Mar 2021 01:46:07 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 06:25:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 12 Mar 2021 06:25:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 12 Mar 2021 06:25:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 06:26:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Mar 2021 06:26:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Mar 2021 06:29:11 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 12 Mar 2021 06:29:11 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 12 Mar 2021 06:29:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 12 Mar 2021 06:29:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 12 Mar 2021 06:29:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 12 Mar 2021 06:29:26 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 12 Mar 2021 06:29:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 12 Mar 2021 06:29:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 06:29:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Mar 2021 06:29:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Mar 2021 06:29:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 12 Mar 2021 06:29:28 GMT
ENV PHP_VERSION=8.0.3
# Fri, 12 Mar 2021 06:29:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 12 Mar 2021 06:29:29 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 12 Mar 2021 06:29:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 12 Mar 2021 06:29:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Mar 2021 06:32:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Mar 2021 06:32:27 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 12 Mar 2021 06:32:28 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Mar 2021 06:32:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Mar 2021 06:32:29 GMT
STOPSIGNAL SIGWINCH
# Fri, 12 Mar 2021 06:32:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 12 Mar 2021 06:32:29 GMT
WORKDIR /var/www/html
# Fri, 12 Mar 2021 06:32:29 GMT
EXPOSE 80
# Fri, 12 Mar 2021 06:32:30 GMT
CMD ["apache2-foreground"]
# Fri, 12 Mar 2021 14:16:46 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 12 Mar 2021 14:16:47 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 12 Mar 2021 14:16:49 GMT
RUN a2enmod rewrite expires
# Fri, 12 Mar 2021 14:16:49 GMT
ENV YOURLS_VERSION=1.8.1
# Fri, 12 Mar 2021 14:16:50 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Fri, 12 Mar 2021 14:16:52 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 12 Mar 2021 14:16:53 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Fri, 12 Mar 2021 14:16:53 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Fri, 12 Mar 2021 14:16:54 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 12 Mar 2021 14:16:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 14:16:54 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d41215965c091534e809ab2e8f4a2c1cebee3de536c2c74a7bc8302bbc8af7e1`  
		Last Modified: Fri, 12 Mar 2021 01:50:30 GMT  
		Size: 25.7 MB (25716294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9dd141052a65d998740b690bf23f87e66d5b424444a5ff93d6c48111ae249e`  
		Last Modified: Fri, 12 Mar 2021 07:08:55 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3bab8af34a0dbb027eb2a45b656ff1fac103644336c21897261781a5e1af4d`  
		Last Modified: Fri, 12 Mar 2021 07:09:09 GMT  
		Size: 64.7 MB (64709520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6048fd685ab61503dafb7e0f87745aad2b5333c1619b088ae5494895426349a`  
		Last Modified: Fri, 12 Mar 2021 07:08:53 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271f221477d4822a9d925f001d26c13fb7998b92db69d831b54ca5b4bd1e24a4`  
		Last Modified: Fri, 12 Mar 2021 07:09:40 GMT  
		Size: 18.5 MB (18524956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ff7e38c41f365dd65becc9c8e1340709af4368653258b91a64e2da62ba0699`  
		Last Modified: Fri, 12 Mar 2021 07:09:38 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59060dc72885f5f6a59b6badfe231da87b05039b0bc5993b5234b3e99b779136`  
		Last Modified: Fri, 12 Mar 2021 07:09:38 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2530ede18afa8cb4893e2fed9fa766c0e08965033f31a60fa79172ac9561ebc1`  
		Last Modified: Fri, 12 Mar 2021 07:09:38 GMT  
		Size: 11.1 MB (11092369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b70451244b8697182a0023ce4b1655f17ae2440e52de25fa04250dcc421bcc`  
		Last Modified: Fri, 12 Mar 2021 07:09:36 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b564822b07225cc692a0c243ed6855c0a57fb52f0ebe2fa112605bdf4f8fe1e`  
		Last Modified: Fri, 12 Mar 2021 07:09:38 GMT  
		Size: 13.3 MB (13349966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393086872c8b08e3b515688e3b51c6e6c8198874704a88115fd35956592f10be`  
		Last Modified: Fri, 12 Mar 2021 07:09:36 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c7c8f25923e393b233cf934335f8b9fbdb0f3a535b48b4d51f7a70e42fa4de`  
		Last Modified: Fri, 12 Mar 2021 07:09:36 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1241335641e5aa039b741b679caa8569e9ccddb66f883c9fb0234a9a8b45d041`  
		Last Modified: Fri, 12 Mar 2021 07:09:36 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6cfc77cec0a2eb5cd58dc642669a3f15dd34a49bb04b8636fd010bdd03758c`  
		Last Modified: Fri, 12 Mar 2021 14:18:02 GMT  
		Size: 350.4 KB (350399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212d2e20d13efcfd42836d5a47ed310b7e0054dc4c30c85b051b772a9ea9b994`  
		Last Modified: Fri, 12 Mar 2021 14:18:02 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fece2a67c2a5d9d9e030be4cde6525cdb17738c56307e7f1b8392f39819691`  
		Last Modified: Fri, 12 Mar 2021 14:18:00 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ceddebddb06a35232f4164fad426f2369abdb76fdc48ce8e679a5d6a7f00d1`  
		Last Modified: Fri, 12 Mar 2021 14:18:01 GMT  
		Size: 2.6 MB (2572144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:181b925f848e855bc59e2915051bac505f3da0740bec98c5cadafc982172fa3d`  
		Last Modified: Fri, 12 Mar 2021 14:18:00 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461df924fd5cf18577399114dd96cc96d4d072e0d5003dccbd15f3d141a6e45d`  
		Last Modified: Fri, 12 Mar 2021 14:18:00 GMT  
		Size: 2.0 KB (2039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc7619b873ee72fd663e5f1df83fc5672c170523b2adb986dcbeb1a3a74ad30`  
		Last Modified: Fri, 12 Mar 2021 14:18:00 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
