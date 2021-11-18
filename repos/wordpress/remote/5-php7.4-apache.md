## `wordpress:5-php7.4-apache`

```console
$ docker pull wordpress@sha256:215072fbe54a0b84d03c0d97c42e740ff4790d55f123f58f5528e2c983273fd4
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

### `wordpress:5-php7.4-apache` - linux; amd64

```console
$ docker pull wordpress@sha256:7d1a52e4ad9f315c74822951fb6a773f19f49dbb720765300df9328f69b17fed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.9 MB (211937190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c6aae97be76e37b99ffc27c0c96ee2fdcb0c0aa46bb2f8354fcfb5ae051bef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:38:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 04:38:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 04:38:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:38:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 04:38:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 04:45:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 04:45:06 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 04:45:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 04:45:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 19:36:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:36:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:36:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 23:04:42 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 22 Oct 2021 17:24:17 GMT
ENV PHP_VERSION=7.4.25
# Fri, 22 Oct 2021 17:24:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Fri, 22 Oct 2021 17:24:17 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Fri, 22 Oct 2021 17:24:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 22 Oct 2021 17:24:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Oct 2021 17:27:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 22 Oct 2021 17:27:16 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 22 Oct 2021 17:27:16 GMT
RUN docker-php-ext-enable sodium
# Fri, 22 Oct 2021 17:27:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 22 Oct 2021 17:27:17 GMT
STOPSIGNAL SIGWINCH
# Fri, 22 Oct 2021 17:27:17 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 22 Oct 2021 17:27:17 GMT
WORKDIR /var/www/html
# Fri, 22 Oct 2021 17:27:17 GMT
EXPOSE 80
# Fri, 22 Oct 2021 17:27:18 GMT
CMD ["apache2-foreground"]
# Fri, 22 Oct 2021 19:50:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 19:51:43 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.5.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 19:51:44 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 22 Oct 2021 19:51:44 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 22 Oct 2021 19:51:45 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 11 Nov 2021 03:08:54 GMT
RUN set -eux; 	version='5.8.2'; 	sha1='c3b1b59553eafbf301c83b14c5eeae4cf1c86044'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 11 Nov 2021 03:08:55 GMT
VOLUME [/var/www/html]
# Thu, 11 Nov 2021 03:08:55 GMT
COPY --chown=www-data:www-datafile:76be5fadb2e2d2b7a74d2770397579cd1402963fdca23912220f983ef906f582 in /usr/src/wordpress/ 
# Thu, 11 Nov 2021 03:08:56 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 11 Nov 2021 03:08:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 03:08:57 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b15dfd3cfa205395e33cb9ea4155c38a2a83a7acee7cb46fb9c169fcbe7411`  
		Last Modified: Tue, 12 Oct 2021 09:03:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64625c2e355fe69d0228e8a97fd6a1eb71879d7abe06240beec04e919e259c02`  
		Last Modified: Tue, 12 Oct 2021 09:04:08 GMT  
		Size: 91.6 MB (91605096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275a8dd8f3587f8c1fe7fc1f672f2e0757e95d18a018a5378cca93b98312415d`  
		Last Modified: Tue, 12 Oct 2021 09:03:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb1c8ccc797aa9ff6819e95d6b867b2696860e31d2cac35e904316766ac9b44d`  
		Last Modified: Tue, 12 Oct 2021 09:04:43 GMT  
		Size: 19.2 MB (19235736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf98f0c33af1f7822072ae2d18f8296d65b117192dbef2026b4bca3737656d`  
		Last Modified: Tue, 12 Oct 2021 09:04:48 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e7c544c3e3203131f005689418e38d82298c3bc2bce4db3efe927345f6e34e`  
		Last Modified: Tue, 12 Oct 2021 09:04:39 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae870a5fb80ce3484e74279b4dc30776f3c9bf904fb93d8ce7759091aac2ed9`  
		Last Modified: Fri, 22 Oct 2021 18:45:32 GMT  
		Size: 10.7 MB (10717432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98833c4f4a49e0a1b6d641e4e0aabac059852f89007a961c1560390a0074f3e8`  
		Last Modified: Fri, 22 Oct 2021 18:45:28 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a6af6bf10a909fceb67a1718266e2a5a54c57d44ae3ae177db2e0328a57494`  
		Last Modified: Fri, 22 Oct 2021 18:45:32 GMT  
		Size: 13.9 MB (13907016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ec4dacea3b4d222c5be7af9c081cbe8cee087e02bbe3f37a6d9a63371b800`  
		Last Modified: Fri, 22 Oct 2021 18:45:28 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab49679021a9b2ce00addf5fcc84e1d5ca28f67f82dfe2332d779ba515a2b434`  
		Last Modified: Fri, 22 Oct 2021 18:45:28 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d224267322b40969fd09cc425e3a8025335edda479c5acb46f783e145dd419`  
		Last Modified: Fri, 22 Oct 2021 18:45:28 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50baad31f9e0dd6f185e22c2fc4ea071da3ef813e042d94cbff51c8a1fa5f496`  
		Last Modified: Fri, 22 Oct 2021 19:57:34 GMT  
		Size: 19.0 MB (18982572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dce3ac87bb9078d7ce75c7755d40feddd81ac9f681377061a509243a5f0a7a4`  
		Last Modified: Fri, 22 Oct 2021 19:57:33 GMT  
		Size: 11.2 MB (11186506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8719cc3579402c444b922036d402c9d25ccee181f6ed8b03632c13058dc59b`  
		Last Modified: Fri, 22 Oct 2021 19:57:31 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69628185e06b0d866a2b31fecdb1db99c78e15b8e9278f43e729fee4b2b7d808`  
		Last Modified: Fri, 22 Oct 2021 19:57:28 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a97cd45ec0271c8f0f7eb3691b735b5ff1c8c0d1a1625b2a55339e620141137`  
		Last Modified: Fri, 22 Oct 2021 19:57:28 GMT  
		Size: 19.5 KB (19497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb42ef6cbf39c23f181c338a7d542ab51fe3e45ef26fde89c510cb1ce881468`  
		Last Modified: Thu, 11 Nov 2021 03:12:30 GMT  
		Size: 14.9 MB (14915745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b88db9d84ead032d724277670bfb95cc7b1c047180a0e5586226ec5c2d3a30`  
		Last Modified: Thu, 11 Nov 2021 03:12:27 GMT  
		Size: 2.3 KB (2348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe8bf4c22f94c368ec96ca8abf94d8fd8d8b3cc3bd5ddcec9b1b3abc1ac64f8`  
		Last Modified: Thu, 11 Nov 2021 03:12:27 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.4-apache` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:9a8ea1493c1e3ce3f6340dd8b4a8a082f9543ee091294764c8ce02356787d598
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.9 MB (187857269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:640adde46eb353277abc4c35bb79b61273177ae02ca097e3ecd1f21054cc0c51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 17 Nov 2021 02:50:37 GMT
ADD file:738a04a17bdb9077594ad9a847333abe28216a7f04d3058718a5e21c236c24bb in / 
# Wed, 17 Nov 2021 02:50:38 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 11:47:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 17 Nov 2021 11:47:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 17 Nov 2021 11:48:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 11:48:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 17 Nov 2021 11:48:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 17 Nov 2021 11:54:37 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 17 Nov 2021 11:54:38 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 17 Nov 2021 11:55:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 17 Nov 2021 11:55:04 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 17 Nov 2021 11:55:06 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 17 Nov 2021 11:55:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 11:55:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 11:55:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 17 Nov 2021 13:24:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 17 Nov 2021 13:24:48 GMT
ENV PHP_VERSION=7.4.25
# Wed, 17 Nov 2021 13:24:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Wed, 17 Nov 2021 13:24:49 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Wed, 17 Nov 2021 13:25:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 17 Nov 2021 13:25:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 17 Nov 2021 13:29:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 17 Nov 2021 13:29:20 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 17 Nov 2021 13:29:21 GMT
RUN docker-php-ext-enable sodium
# Wed, 17 Nov 2021 13:29:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 17 Nov 2021 13:29:22 GMT
STOPSIGNAL SIGWINCH
# Wed, 17 Nov 2021 13:29:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 17 Nov 2021 13:29:23 GMT
WORKDIR /var/www/html
# Wed, 17 Nov 2021 13:29:23 GMT
EXPOSE 80
# Wed, 17 Nov 2021 13:29:24 GMT
CMD ["apache2-foreground"]
# Thu, 18 Nov 2021 01:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 01:49:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.5.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 01:49:25 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 18 Nov 2021 01:49:27 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 18 Nov 2021 01:49:29 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 18 Nov 2021 01:49:37 GMT
RUN set -eux; 	version='5.8.2'; 	sha1='c3b1b59553eafbf301c83b14c5eeae4cf1c86044'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 18 Nov 2021 01:49:37 GMT
VOLUME [/var/www/html]
# Thu, 18 Nov 2021 01:49:38 GMT
COPY --chown=www-data:www-datafile:76be5fadb2e2d2b7a74d2770397579cd1402963fdca23912220f983ef906f582 in /usr/src/wordpress/ 
# Thu, 18 Nov 2021 01:49:38 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 18 Nov 2021 01:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 01:49:39 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a960a56baa1baffbe2aa1e0c1fb02f9ee4816337d02fec259b312c409d77fafc`  
		Last Modified: Wed, 17 Nov 2021 03:06:09 GMT  
		Size: 28.9 MB (28911006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d62576d1f6422c12c501987232cd6f109fa674dc90280a6e5f6df8a00ae06e`  
		Last Modified: Wed, 17 Nov 2021 14:52:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0656b9bd7ea73f5f220dc0afd21463ece375910ea9be93642df3ebe82adb6dfe`  
		Last Modified: Wed, 17 Nov 2021 14:53:02 GMT  
		Size: 73.7 MB (73684261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8f131fa288cff4e5199651721306dde0c83007d84f312a29e3b52dc74ce94e`  
		Last Modified: Wed, 17 Nov 2021 14:52:11 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d6c1536456cc545cb407c3b891f7080543b47eb4148d28998c839d79d18c36`  
		Last Modified: Wed, 17 Nov 2021 14:53:53 GMT  
		Size: 18.5 MB (18525659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5cf7cbd672acd1680272f57a540436ba2906de5a1a7347128ddc8071ed033e`  
		Last Modified: Wed, 17 Nov 2021 14:53:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0366e9bd9df4f3876ff7dcd3089019696af4de6ad3003aab4e1515e32cb0f2`  
		Last Modified: Wed, 17 Nov 2021 14:53:42 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fd5395ad7d49926bfdfeb6b78a0f7966829992e86e52c37cd52586b7463e69`  
		Last Modified: Wed, 17 Nov 2021 15:06:25 GMT  
		Size: 10.7 MB (10716105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e79436e84bb1ce437465295665482bf12ef44d4c86befb46da5b4575bf6ab`  
		Last Modified: Wed, 17 Nov 2021 15:06:21 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ff0f98a04576de47f661d011b208ebda1bef871eb4a7db692e264b2c777de5`  
		Last Modified: Wed, 17 Nov 2021 15:06:30 GMT  
		Size: 13.0 MB (12980625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3944c1d9d681d71c0b9da5429680d0258b6f747061874ba85b724e206eba8fd8`  
		Last Modified: Wed, 17 Nov 2021 15:06:21 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948cc1956ba9f61a4fac349d8e33b21245a8dc5665eba5dd68d7dc61e15b4cc9`  
		Last Modified: Wed, 17 Nov 2021 15:06:21 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28887401f7736aa19db1b95eb649015f163c7a8df04bb6e2e03350f895b040b6`  
		Last Modified: Wed, 17 Nov 2021 15:06:21 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e475d40523e9b29d70ea5b6b69084fd0ca67e79fb1e4eaa94a7309b9ac24f1e1`  
		Last Modified: Thu, 18 Nov 2021 02:12:38 GMT  
		Size: 18.6 MB (18566546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a6412464abf7e5cbe1ec06ac2e5dd2faee01064167bdaa8229d4b65d64fe7af`  
		Last Modified: Thu, 18 Nov 2021 02:12:26 GMT  
		Size: 9.5 MB (9527527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:307c9efdd2a40e89be3c71add6015d8b2b671e052d5df93728339629c9f32f61`  
		Last Modified: Thu, 18 Nov 2021 02:12:20 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0f95fa381cc59fa17e58db96771970a9c7682c70cf08797f92ca0c1b76da2b`  
		Last Modified: Thu, 18 Nov 2021 02:12:18 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f618d1978c182e676af241842d5b39d0906ebc7524c4bada969e33f2350c56`  
		Last Modified: Thu, 18 Nov 2021 02:12:18 GMT  
		Size: 19.5 KB (19502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abb46e5194a58107d18d2123b98d8c26c26c5ee732d2d33bad1dc1348746dfc`  
		Last Modified: Thu, 18 Nov 2021 02:12:31 GMT  
		Size: 14.9 MB (14915748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9053a2e78e4d2d991bb77d29481700eaf9d2163bda960e9abd31f5ebe214766`  
		Last Modified: Thu, 18 Nov 2021 02:12:18 GMT  
		Size: 2.4 KB (2350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5b935fe10b1b180227d27c74ad88f44bc370190aef7a0dea7d5e8900a53bb7`  
		Last Modified: Thu, 18 Nov 2021 02:12:18 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.4-apache` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:c67dd1edf31cb068b78a604650115c7b3e5b5821494c7a4ec9e2d90f9dc06e8d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.5 MB (178530063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13e6cf09bc366a91255ba5c4315e877361232087a0923cefa3e32061d23f71a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 10:11:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 10:11:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 10:12:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 10:12:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 10:12:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 10:17:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 10:17:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 10:18:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 10:18:19 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 10:18:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 19:13:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:13:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:13:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 21:18:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 22 Oct 2021 19:00:32 GMT
ENV PHP_VERSION=7.4.25
# Fri, 22 Oct 2021 19:00:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Fri, 22 Oct 2021 19:00:33 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Fri, 22 Oct 2021 19:00:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 22 Oct 2021 19:00:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Oct 2021 19:04:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 22 Oct 2021 19:04:46 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 22 Oct 2021 19:04:48 GMT
RUN docker-php-ext-enable sodium
# Fri, 22 Oct 2021 19:04:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 22 Oct 2021 19:04:49 GMT
STOPSIGNAL SIGWINCH
# Fri, 22 Oct 2021 19:04:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 22 Oct 2021 19:04:50 GMT
WORKDIR /var/www/html
# Fri, 22 Oct 2021 19:04:50 GMT
EXPOSE 80
# Fri, 22 Oct 2021 19:04:51 GMT
CMD ["apache2-foreground"]
# Sat, 23 Oct 2021 01:00:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Oct 2021 01:03:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.5.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Oct 2021 01:03:53 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 23 Oct 2021 01:03:55 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 23 Oct 2021 01:03:57 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 11 Nov 2021 03:55:09 GMT
RUN set -eux; 	version='5.8.2'; 	sha1='c3b1b59553eafbf301c83b14c5eeae4cf1c86044'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 11 Nov 2021 03:55:09 GMT
VOLUME [/var/www/html]
# Thu, 11 Nov 2021 03:55:10 GMT
COPY --chown=www-data:www-datafile:76be5fadb2e2d2b7a74d2770397579cd1402963fdca23912220f983ef906f582 in /usr/src/wordpress/ 
# Thu, 11 Nov 2021 03:55:11 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 11 Nov 2021 03:55:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 03:55:12 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd9f480a07dd663124a4fa2dd037ecfa121fb7f48c5611ad0bfdcc1a8620a95`  
		Last Modified: Tue, 12 Oct 2021 13:25:43 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541b04bc4262d66b1debf2bdfc8f9af3aaaf35857a5129ef875c83b66d9ca381`  
		Last Modified: Tue, 12 Oct 2021 13:26:25 GMT  
		Size: 69.3 MB (69314813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0c01531f1abfd9002da0136f1c5f9d7f1dded1e9c635594a2416f9b2592b57`  
		Last Modified: Tue, 12 Oct 2021 13:25:43 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46f326eb4d7df5b1062f7cf9febcde80dff286e3c58467e4b0bb4fe994e1c49`  
		Last Modified: Tue, 12 Oct 2021 13:27:16 GMT  
		Size: 18.0 MB (17987465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90b5a512593f340cfcf524a288c914574af941f7ba1ca3407b4c8810ef9f2f9`  
		Last Modified: Tue, 12 Oct 2021 13:27:06 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5ae29d359a60994986ddf2bc5eeffe6ec88d873499473e034fd5633404c155`  
		Last Modified: Tue, 12 Oct 2021 13:27:06 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441c420d4fa4eaabac2d85eabd8d25631ea0c56187b104b9c0a3e2c8a1830586`  
		Last Modified: Fri, 22 Oct 2021 20:26:40 GMT  
		Size: 10.7 MB (10716107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98eb56e31d13a77459334c669880680d4f964431c674d684f0a324539e2f2de2`  
		Last Modified: Fri, 22 Oct 2021 20:26:36 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda4deb6685590b000c82f67aabb0917683305a5e133220712c771bb48ac31ea`  
		Last Modified: Fri, 22 Oct 2021 20:26:44 GMT  
		Size: 12.3 MB (12278026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25b6d00aec06af4c9b5332f45b4830e8a05cf6c69ac6423e723958a461e8911`  
		Last Modified: Fri, 22 Oct 2021 20:26:36 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a81f6f9da40aae5eea040ef9a937042286e69c8ccf03f8799aa8871e69cccf7`  
		Last Modified: Fri, 22 Oct 2021 20:26:36 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca2220ed6db28d39b8629e53c631d502b0841b3b8ed2a7034c76f8613e7346f`  
		Last Modified: Fri, 22 Oct 2021 20:26:36 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47112e1d246e554ea4a227adb1bc68dbc586d877d6eda1d567cf5719fdd06a89`  
		Last Modified: Sat, 23 Oct 2021 01:20:53 GMT  
		Size: 18.1 MB (18113042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25233b538ca588787452b4a065698575f0365a5acafe23ffe72e8824a69ff5ce`  
		Last Modified: Sat, 23 Oct 2021 01:20:46 GMT  
		Size: 8.6 MB (8613987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd58a47886afb877a7b75fdc6d01681a3d0ed39bfeaab8727f67f51daaa2a79`  
		Last Modified: Sat, 23 Oct 2021 01:20:41 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed726e8ebf2172e2fbb81bdd3cac644e3eba80cefd974e50be1c734ba87623d`  
		Last Modified: Sat, 23 Oct 2021 01:20:39 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869a51f172c5d1dd7da4277307781adb44b265313d11ec0c7dfb96dea560e5eb`  
		Last Modified: Sat, 23 Oct 2021 01:20:39 GMT  
		Size: 19.5 KB (19497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa76ed8dcdbe3e31fae964277799d509ca73aa0f4b75172d44990e9349f60ea8`  
		Last Modified: Thu, 11 Nov 2021 04:05:30 GMT  
		Size: 14.9 MB (14915762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a883653db671f87aeae43515c52d8299e42e81bd012703bbb01c41bf8cff8e`  
		Last Modified: Thu, 11 Nov 2021 04:05:18 GMT  
		Size: 2.4 KB (2352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d96d31e2a8467f362ffefc2b08ccadff77db1ae87b6631f3d7d1df9992f663de`  
		Last Modified: Thu, 11 Nov 2021 04:05:18 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.4-apache` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:4f558e257de9b79f12bceabae0d3fa611ae114a5dc2c66e0e28da093e5ba33b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.7 MB (202661753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9aaf2a0e3215e3110be58c91872f8c363789f2c3f454065467dc2371f3d34822`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:15 GMT
ADD file:4203242b2b09a65239092c4780b59181da7b861b3c0be40810b3588aa200f72c in / 
# Wed, 17 Nov 2021 02:40:16 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 06:44:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 17 Nov 2021 06:44:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 17 Nov 2021 06:45:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 06:45:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 17 Nov 2021 06:45:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 17 Nov 2021 06:50:52 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 17 Nov 2021 06:50:52 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 17 Nov 2021 06:51:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 17 Nov 2021 06:51:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 17 Nov 2021 06:51:04 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 17 Nov 2021 06:51:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 06:51:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 06:51:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 17 Nov 2021 07:56:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 17 Nov 2021 07:56:07 GMT
ENV PHP_VERSION=7.4.25
# Wed, 17 Nov 2021 07:56:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Wed, 17 Nov 2021 07:56:09 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Wed, 17 Nov 2021 07:56:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 17 Nov 2021 07:56:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 17 Nov 2021 07:58:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 17 Nov 2021 07:58:33 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 17 Nov 2021 07:58:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 17 Nov 2021 07:58:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 17 Nov 2021 07:58:35 GMT
STOPSIGNAL SIGWINCH
# Wed, 17 Nov 2021 07:58:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 17 Nov 2021 07:58:37 GMT
WORKDIR /var/www/html
# Wed, 17 Nov 2021 07:58:38 GMT
EXPOSE 80
# Wed, 17 Nov 2021 07:58:39 GMT
CMD ["apache2-foreground"]
# Wed, 17 Nov 2021 19:06:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 19:08:11 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.5.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 19:08:12 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 17 Nov 2021 19:08:14 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 17 Nov 2021 19:08:15 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 17 Nov 2021 19:08:32 GMT
RUN set -eux; 	version='5.8.2'; 	sha1='c3b1b59553eafbf301c83b14c5eeae4cf1c86044'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Wed, 17 Nov 2021 19:08:33 GMT
VOLUME [/var/www/html]
# Wed, 17 Nov 2021 19:08:34 GMT
COPY --chown=www-data:www-datafile:76be5fadb2e2d2b7a74d2770397579cd1402963fdca23912220f983ef906f582 in /usr/src/wordpress/ 
# Wed, 17 Nov 2021 19:08:35 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Wed, 17 Nov 2021 19:08:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 19:08:36 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:eb9a2845ed124d072b117aba4f0508e00c1ecd0d147dc324d14b00d24092046c`  
		Last Modified: Wed, 17 Nov 2021 02:47:17 GMT  
		Size: 30.1 MB (30056521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1847f78773be660931f29a4050db3271037ee366cac5ce00ae85e7947d8cdc3d`  
		Last Modified: Wed, 17 Nov 2021 08:46:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff48a7e6ce3d33defbe3abff6655704311cbb0ad65a855b59a422e4bc8df4e7`  
		Last Modified: Wed, 17 Nov 2021 08:47:10 GMT  
		Size: 86.7 MB (86716235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3c1623fb1adb820df0baf352d9746fe483abf563eab7f2a512afeb7514c530`  
		Last Modified: Wed, 17 Nov 2021 08:46:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1c53e8f2d4cbefdac4405673b073684e0803a42e9c5d6df5af0c617020402c`  
		Last Modified: Wed, 17 Nov 2021 08:47:46 GMT  
		Size: 18.9 MB (18939848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5483b3a0c1fcbff43752a1c36e0dfebfaaeccd5194e7bfae4283ed40dd34d65`  
		Last Modified: Wed, 17 Nov 2021 08:47:43 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64c488b1ecacf5edaebdaa18ba90df5e598f29800581c5d92a239f7e6ec737a`  
		Last Modified: Wed, 17 Nov 2021 08:47:43 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ae177d66a318552d9e1cb4bc3635c7f1af8d60aa09f7467fd4d0f7266b77e1`  
		Last Modified: Wed, 17 Nov 2021 08:56:00 GMT  
		Size: 10.5 MB (10500209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cc28d930a0a9aeeb24d1a710141f75a463a82ba2425d279c33e4f623603a74`  
		Last Modified: Wed, 17 Nov 2021 08:55:57 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd150d4b019a9a7b03264dc1c300da08b6d663ad6376b881b6d61f4373d27363`  
		Last Modified: Wed, 17 Nov 2021 08:55:59 GMT  
		Size: 13.6 MB (13646962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1acc9fcbff8c35beb6d19b7197632671a690dd7c888e11b83623754017bca781`  
		Last Modified: Wed, 17 Nov 2021 08:55:56 GMT  
		Size: 2.3 KB (2315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ed029351735267a1e482c212762b28844996b015a257b0a311a1d5e2583780`  
		Last Modified: Wed, 17 Nov 2021 08:55:56 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ec067b67c439af057ffb059dfabcf5cfa0263d11061c98de2bf7ae0819d5e4`  
		Last Modified: Wed, 17 Nov 2021 08:55:56 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59464934a7274f707780e248c235f56579e3ea8f2f2267a690e6ba75ec63254c`  
		Last Modified: Wed, 17 Nov 2021 19:21:16 GMT  
		Size: 19.0 MB (18951996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2a8fb651287107df7fccfdb20393d79a33339c53ae841408cb3da29c2f305a`  
		Last Modified: Wed, 17 Nov 2021 19:21:14 GMT  
		Size: 8.9 MB (8906941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd929a9fbde1e7f397a9adb98f15b2ebb07f0d9a1bea2bd48570d7374fda388`  
		Last Modified: Wed, 17 Nov 2021 19:21:12 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab086202c91a6274b3986005c5798e3aed899fb8ff15b5e9b75b59000be6e93f`  
		Last Modified: Wed, 17 Nov 2021 19:21:10 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264765ea8abe425da51a131673a579157e1063679a838d65722f8a1fe9ce4f40`  
		Last Modified: Wed, 17 Nov 2021 19:21:10 GMT  
		Size: 19.5 KB (19493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3500743eed0fd5b5eac41b81f31fa6a88804c51abbfc37a0a2acf85502e5da65`  
		Last Modified: Wed, 17 Nov 2021 19:21:13 GMT  
		Size: 14.9 MB (14913392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0180072a4f99fc7ea4bd5e031be9d39f0aa69355f6ada7abd85b8e706f52497`  
		Last Modified: Wed, 17 Nov 2021 19:21:11 GMT  
		Size: 2.4 KB (2351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4b78610e8bb9272d884e38b7d97f367fe82463040ce0d04f0ffe6b18ecac0a`  
		Last Modified: Wed, 17 Nov 2021 19:21:10 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.4-apache` - linux; 386

```console
$ docker pull wordpress@sha256:59f88c176baa5e7a5e04890546571cef2485877690f8f84801a82ee610f09e8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214455943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7202cfba7e5e42194870ed996c43b53fd46e18668ff39dbfb059a586b5d3e38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 17 Nov 2021 02:39:53 GMT
ADD file:ff018048717c0f5aa1730480d0bfea1c2bf94d6e2dae2d7cef46d05ffb0d93e1 in / 
# Wed, 17 Nov 2021 02:39:53 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 09:16:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 17 Nov 2021 09:16:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 17 Nov 2021 09:16:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 09:16:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 17 Nov 2021 09:16:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 17 Nov 2021 09:23:38 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 17 Nov 2021 09:23:39 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 17 Nov 2021 09:23:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 17 Nov 2021 09:23:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 17 Nov 2021 09:23:53 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 17 Nov 2021 09:23:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 09:23:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 09:23:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 17 Nov 2021 11:03:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 17 Nov 2021 11:03:27 GMT
ENV PHP_VERSION=7.4.25
# Wed, 17 Nov 2021 11:03:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Wed, 17 Nov 2021 11:03:27 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Wed, 17 Nov 2021 11:03:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 17 Nov 2021 11:03:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 17 Nov 2021 11:08:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 17 Nov 2021 11:08:18 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Wed, 17 Nov 2021 11:08:20 GMT
RUN docker-php-ext-enable sodium
# Wed, 17 Nov 2021 11:08:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 17 Nov 2021 11:08:21 GMT
STOPSIGNAL SIGWINCH
# Wed, 17 Nov 2021 11:08:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 17 Nov 2021 11:08:22 GMT
WORKDIR /var/www/html
# Wed, 17 Nov 2021 11:08:22 GMT
EXPOSE 80
# Wed, 17 Nov 2021 11:08:22 GMT
CMD ["apache2-foreground"]
# Wed, 17 Nov 2021 23:32:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 23:33:57 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.5.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 23:33:59 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 17 Nov 2021 23:34:01 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 17 Nov 2021 23:34:03 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Wed, 17 Nov 2021 23:34:09 GMT
RUN set -eux; 	version='5.8.2'; 	sha1='c3b1b59553eafbf301c83b14c5eeae4cf1c86044'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Wed, 17 Nov 2021 23:34:09 GMT
VOLUME [/var/www/html]
# Wed, 17 Nov 2021 23:34:10 GMT
COPY --chown=www-data:www-datafile:76be5fadb2e2d2b7a74d2770397579cd1402963fdca23912220f983ef906f582 in /usr/src/wordpress/ 
# Wed, 17 Nov 2021 23:34:10 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Wed, 17 Nov 2021 23:34:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 17 Nov 2021 23:34:11 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0bae0e1d4cb1d56ffeb9d05de7a097d3157267eef07b6d8131344d99bd97c431`  
		Last Modified: Wed, 17 Nov 2021 02:47:49 GMT  
		Size: 32.4 MB (32380683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e9208767da7df5fdb2170d7142de5a0e92c17b08c9c8b0b50d31d314fabe72`  
		Last Modified: Wed, 17 Nov 2021 12:48:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fea35b73840adac94518cb2d327d4e6d709abf3c5590ba808169ec172b7eb1`  
		Last Modified: Wed, 17 Nov 2021 12:48:47 GMT  
		Size: 92.7 MB (92716817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769bb36e0e1016e5c697903187baaa41d7173041322430b61e0cf51383eafb94`  
		Last Modified: Wed, 17 Nov 2021 12:48:10 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe854d5cfdf4190168816bb74032faeccfa17cee11274c09e4914583c508da6`  
		Last Modified: Wed, 17 Nov 2021 12:49:27 GMT  
		Size: 19.7 MB (19713910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdce16058c1902813c444604c212a40e1f7fbbfdb4e499392d29e2d7a0e82fcd`  
		Last Modified: Wed, 17 Nov 2021 12:49:22 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e8844955045ee8d74f7480cc227291bd4329160fe22bc170ef5c26292d4a85`  
		Last Modified: Wed, 17 Nov 2021 12:49:22 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231eec9b6e0c71fd7f657a29f9d5b822aa0d4b3788827a330be171c86fa5d25d`  
		Last Modified: Wed, 17 Nov 2021 13:00:45 GMT  
		Size: 10.7 MB (10716800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd92cb53f8e92411dc8273d5042bad52cc03d3c98dced67cd1db1b42ab2ee965`  
		Last Modified: Wed, 17 Nov 2021 13:00:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca89c560ccfa65de7dad30b59509a53bf792745f089fdf72f35192335650842f`  
		Last Modified: Wed, 17 Nov 2021 13:00:47 GMT  
		Size: 14.2 MB (14231480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7098c3f11e8cc4b1a43bbfa96ed8adb95a3ed4c0fa65cd81b0c6b012d919991`  
		Last Modified: Wed, 17 Nov 2021 13:00:40 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be487459425c8ab02c859ee1af02d028fdcf72c0f8c36ed0d2c0904671a9c98`  
		Last Modified: Wed, 17 Nov 2021 13:00:40 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e5bc6afe9098679063ef8fc6d0c9070a47c2758c66ccc130c55f60ac288c2b`  
		Last Modified: Wed, 17 Nov 2021 13:00:40 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ceefe8648c7457fea3c714ec12025f57f52375f62e63528dc5b11b8cd6d1e4d`  
		Last Modified: Wed, 17 Nov 2021 23:50:37 GMT  
		Size: 19.3 MB (19328540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747fb09d0d68e3cb340d1226eee5983c85d96c33ed05aae77d51b6bb680b40df`  
		Last Modified: Wed, 17 Nov 2021 23:50:35 GMT  
		Size: 10.4 MB (10422157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32d0787aa794e648743aee00883490e503693917bc9744653ba08dc476ab200`  
		Last Modified: Wed, 17 Nov 2021 23:50:31 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea702914a857c5be6fb5a1431f9baa3b8b65a8b9f0bff441c80ac802cedc57bc`  
		Last Modified: Wed, 17 Nov 2021 23:50:28 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def7d371f8a6d6f636b4ea3477a5d028961d1bbd1e51496f5e57cd1df32996eb`  
		Last Modified: Wed, 17 Nov 2021 23:50:28 GMT  
		Size: 19.5 KB (19501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d8deaa82548d2f4e0ed202937eac15770239786dcf947bd8cc8381a6240bd8`  
		Last Modified: Wed, 17 Nov 2021 23:50:33 GMT  
		Size: 14.9 MB (14915767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f506dd5776f2cacb2714fdecbe43c8d04e923a29e9976c64b76be1a1f124c5`  
		Last Modified: Wed, 17 Nov 2021 23:50:28 GMT  
		Size: 2.4 KB (2352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944e1cf40521c9a45ab74650196186047d5563dbba8efee7fc753ebe9bd93de`  
		Last Modified: Wed, 17 Nov 2021 23:50:28 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.4-apache` - linux; mips64le

```console
$ docker pull wordpress@sha256:528c51a22f82ee48d724a6b177659cc5bd9f00cc199867a1761cb9d8b567e6d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.5 MB (187537641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ebb1967c8202823e185ba8a7068dd1fc3d79a79dd8fdebccb2aed00467d2fe5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:11:15 GMT
ADD file:f90ca8957172106f42a9096c9a21082d51f3201aa78e6f64621a73117e2b7b6a in / 
# Tue, 12 Oct 2021 01:11:16 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:09:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 18:09:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 18:10:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:10:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 18:10:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 18:24:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 18:24:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 18:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 18:24:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 18:24:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 19:23:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:23:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:23:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 22:46:30 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 22 Oct 2021 18:19:56 GMT
ENV PHP_VERSION=7.4.25
# Fri, 22 Oct 2021 18:19:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Fri, 22 Oct 2021 18:19:57 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Fri, 22 Oct 2021 18:20:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 22 Oct 2021 18:20:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:28:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 22 Oct 2021 18:28:10 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:28:12 GMT
RUN docker-php-ext-enable sodium
# Fri, 22 Oct 2021 18:28:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 22 Oct 2021 18:28:13 GMT
STOPSIGNAL SIGWINCH
# Fri, 22 Oct 2021 18:28:13 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:28:13 GMT
WORKDIR /var/www/html
# Fri, 22 Oct 2021 18:28:14 GMT
EXPOSE 80
# Fri, 22 Oct 2021 18:28:14 GMT
CMD ["apache2-foreground"]
# Fri, 22 Oct 2021 20:44:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 20:48:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.5.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Oct 2021 20:48:27 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 22 Oct 2021 20:48:29 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 22 Oct 2021 20:48:31 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 11 Nov 2021 02:35:43 GMT
RUN set -eux; 	version='5.8.2'; 	sha1='c3b1b59553eafbf301c83b14c5eeae4cf1c86044'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 11 Nov 2021 02:35:44 GMT
VOLUME [/var/www/html]
# Thu, 11 Nov 2021 02:35:44 GMT
COPY --chown=www-data:www-datafile:76be5fadb2e2d2b7a74d2770397579cd1402963fdca23912220f983ef906f582 in /usr/src/wordpress/ 
# Thu, 11 Nov 2021 02:35:44 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 11 Nov 2021 02:35:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 02:35:45 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:59ddca50ce05605e6234c1e7213c39cdedabc48ef11637e12156b7bd69afe161`  
		Last Modified: Tue, 12 Oct 2021 01:20:03 GMT  
		Size: 29.6 MB (29618732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ff87c2332509770737b3726a7edbc9070eb8965e3168af4e323e11735f2c92`  
		Last Modified: Wed, 13 Oct 2021 00:47:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb84497951b93c12a62afde8f02ebbea1b6bc7408856d226297b5a3be0a7c92`  
		Last Modified: Wed, 13 Oct 2021 00:48:33 GMT  
		Size: 72.0 MB (72014027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d4e4615e6fe3d8e364eacce72f7ccce515209e2da18447ca24da978c31e38c`  
		Last Modified: Wed, 13 Oct 2021 00:47:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4922634a24fcda8d05a799ce9a76bad0bc77f74e6183b0c01c24561c5fcdf50a`  
		Last Modified: Wed, 13 Oct 2021 00:49:17 GMT  
		Size: 19.1 MB (19143667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727d7b8f91bd9e80b3890e0309546b7201a45d40c6c45c35efca82a3c5fe40ff`  
		Last Modified: Wed, 13 Oct 2021 00:49:04 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d4efcc601a141d1be58474d763f5f131619fdfdcc0d3d3bee16bfb8e7241e7`  
		Last Modified: Wed, 13 Oct 2021 00:49:04 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff39d4b515e0968dad6a8960841e25b323021a58aba19c5d09e56ee406cf94b`  
		Last Modified: Fri, 22 Oct 2021 19:31:44 GMT  
		Size: 10.7 MB (10715274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0535ace4b47c86005f9cead5c00d83b4bdcbc8bb128e76b5f357de73fab2bd`  
		Last Modified: Fri, 22 Oct 2021 19:31:39 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f558493c0114bccc3c3ddb28645f1912a6aa12cf581cb5c879214ff0511a6a`  
		Last Modified: Fri, 22 Oct 2021 19:31:50 GMT  
		Size: 13.2 MB (13193042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c86c2b8f2fd1abab0b333bebc4bb70f7d22e72e3e5e139fca608b6e018f022c`  
		Last Modified: Fri, 22 Oct 2021 19:31:39 GMT  
		Size: 2.3 KB (2312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a680d76054af3dc42315a5f462ad671525b0a330111c977cf5fe4d7ddb2d98f3`  
		Last Modified: Fri, 22 Oct 2021 19:31:39 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbf28cec544ed1dfbe7330d7bd1d2d435a5e13ba98c358ef6e7773a0654f7bc`  
		Last Modified: Fri, 22 Oct 2021 19:31:39 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce14436617152438aa3c9c06dc3a6efbffb5cf4de4d3061dc35523d65963752`  
		Last Modified: Fri, 22 Oct 2021 20:54:11 GMT  
		Size: 18.8 MB (18795642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0665285259fc7d726908c64efc6da3f8c5bb8590944f5da46c91a30d2d186ed8`  
		Last Modified: Fri, 22 Oct 2021 20:54:02 GMT  
		Size: 9.1 MB (9111871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f57fe12c60e03c6fe10444a12edafb7a5b8c6fde623c12cf38a326a11c6359`  
		Last Modified: Fri, 22 Oct 2021 20:53:55 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19204ea24ba5f9c05e4c2fbebf3785233679202679626b0d8b64786fca7b45ea`  
		Last Modified: Fri, 22 Oct 2021 20:53:52 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf0df08afbc50f594d7028d9592a2e7b058deb19efa0e56ccb862bfe7441519`  
		Last Modified: Fri, 22 Oct 2021 20:53:52 GMT  
		Size: 19.5 KB (19502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b71509d74f77b3b3fb49b26f6c0102ef5b3e1c816754317be0835b6b3d50c94`  
		Last Modified: Thu, 11 Nov 2021 02:37:54 GMT  
		Size: 14.9 MB (14915722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d40addb0c0e754cfa2de779cc18d5fbc9cb6bfb2ff211bf6514df7ee5dd551`  
		Last Modified: Thu, 11 Nov 2021 02:37:43 GMT  
		Size: 2.3 KB (2349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d73315a1dfdb2efa30ec79702640bb4c5743d672cfb7a50c4b5638dedccdff`  
		Last Modified: Thu, 11 Nov 2021 02:37:43 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.4-apache` - linux; ppc64le

```console
$ docker pull wordpress@sha256:5e4b6ac0b2fad60ea7eb149a78c9acce47074ab7c29857be9a665ff379346177
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.4 MB (213355969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:819c0790207d6f0265cf7db546eded045af13587f553e581dce8e4ab0d0d070b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Oct 2021 01:25:45 GMT
ADD file:d8794fadf16c9948c3574ba28740d08393eca57766340333ad91f9c2a33eb719 in / 
# Tue, 12 Oct 2021 01:25:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 10:23:39 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Oct 2021 10:23:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Oct 2021 10:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 10:26:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Oct 2021 10:26:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Oct 2021 10:33:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Oct 2021 10:33:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Oct 2021 10:34:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Oct 2021 10:34:39 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Oct 2021 10:34:47 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 14 Oct 2021 19:29:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:29:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 19:29:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 21:55:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 22 Oct 2021 18:14:55 GMT
ENV PHP_VERSION=7.4.25
# Fri, 22 Oct 2021 18:15:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Fri, 22 Oct 2021 18:15:14 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Fri, 22 Oct 2021 18:16:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 22 Oct 2021 18:16:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:20:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 22 Oct 2021 18:20:34 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:20:40 GMT
RUN docker-php-ext-enable sodium
# Fri, 22 Oct 2021 18:20:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 22 Oct 2021 18:20:46 GMT
STOPSIGNAL SIGWINCH
# Fri, 22 Oct 2021 18:20:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:20:51 GMT
WORKDIR /var/www/html
# Fri, 22 Oct 2021 18:20:56 GMT
EXPOSE 80
# Fri, 22 Oct 2021 18:21:01 GMT
CMD ["apache2-foreground"]
# Sat, 23 Oct 2021 03:25:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Oct 2021 03:32:25 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.5.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Oct 2021 03:32:33 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 23 Oct 2021 03:32:40 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 23 Oct 2021 03:32:50 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 11 Nov 2021 06:10:31 GMT
RUN set -eux; 	version='5.8.2'; 	sha1='c3b1b59553eafbf301c83b14c5eeae4cf1c86044'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 11 Nov 2021 06:10:36 GMT
VOLUME [/var/www/html]
# Thu, 11 Nov 2021 06:10:38 GMT
COPY --chown=www-data:www-datafile:76be5fadb2e2d2b7a74d2770397579cd1402963fdca23912220f983ef906f582 in /usr/src/wordpress/ 
# Thu, 11 Nov 2021 06:10:39 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 11 Nov 2021 06:10:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Nov 2021 06:10:45 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6c28c1405c677dd809094d06190225b38cee3d24f18da38d287ef5bcc67884d6`  
		Last Modified: Tue, 12 Oct 2021 01:37:00 GMT  
		Size: 35.3 MB (35258729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007cbc0c1bbccf469e9d9fc6e98e3d4ad1e4469d5f23cc0d263aa3bdc8f9c5`  
		Last Modified: Tue, 12 Oct 2021 14:32:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6750fd2121e14e6e55c726ed712f7b485e03363824dd42e9fa37ca714848f4c6`  
		Last Modified: Tue, 12 Oct 2021 14:33:23 GMT  
		Size: 86.6 MB (86624771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6280509c1db590ff214716adca9daabd1ac3c060c29e70cf6ed8dc17061d64db`  
		Last Modified: Tue, 12 Oct 2021 14:32:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dfb045a88eef5b0550b8548fbf2106468aac82881db516e679b9d5811ab750`  
		Last Modified: Tue, 12 Oct 2021 14:34:14 GMT  
		Size: 20.4 MB (20441245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b153f7d4d58c38f56768aadaefa599fdeb615c6c4940ce33f129d7df3c44d8a`  
		Last Modified: Tue, 12 Oct 2021 14:33:57 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed81b8cad279c736a63388220d89e0dc436c6f8586239e6e9c3b975efaf6c1f`  
		Last Modified: Tue, 12 Oct 2021 14:33:57 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6664c5fe31628f3d13610e4e1621cd22bb13a7eda72537009e392cf738843e7`  
		Last Modified: Fri, 22 Oct 2021 19:37:55 GMT  
		Size: 10.7 MB (10717801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a168131fa66134b551b307d5bd68fbe670aca9d7999c9bc7915677ca673f2c7`  
		Last Modified: Fri, 22 Oct 2021 19:37:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0de409f50eaa52b6803598f2104f7ec3fa0ee57be889704cd49ee6b87051f0`  
		Last Modified: Fri, 22 Oct 2021 19:37:55 GMT  
		Size: 14.9 MB (14923889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de451f8c6d03d3e2dcd9630682fb5495c6f72179689bc04cc7c17d50055cd11`  
		Last Modified: Fri, 22 Oct 2021 19:37:52 GMT  
		Size: 2.3 KB (2318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25017d0a4d4690d8232ce2a73642c1c49fb033165ddafe6f039e20b528d9d9c1`  
		Last Modified: Fri, 22 Oct 2021 19:37:51 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b32079592457acbdb41ffe48dcbebb40f00c2c875cd50fd64a502f807e7fa02`  
		Last Modified: Fri, 22 Oct 2021 19:37:51 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e90f944f494204cd7aa70fe251b7c7357cfb3c51cac75ac859744a6087187e`  
		Last Modified: Sat, 23 Oct 2021 03:51:17 GMT  
		Size: 19.8 MB (19822958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b6f85bdc11a295417fc34412c0872e7c6ae06a662ab468225ba06b6da89d55`  
		Last Modified: Sat, 23 Oct 2021 03:51:14 GMT  
		Size: 10.6 MB (10621018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86bff22404b777e968f9b28da115070fbf2b5d415c1085c177664192328218de`  
		Last Modified: Sat, 23 Oct 2021 03:51:13 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f213b96ab5fc7c19c1d75dfeefed12b64c897610de2c1c6ff0c1a827891265`  
		Last Modified: Sat, 23 Oct 2021 03:51:10 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a981d74289957c25dfc3af7ba09cad660436366ce22df3acdea8b5f21f1f084e`  
		Last Modified: Sat, 23 Oct 2021 03:51:10 GMT  
		Size: 19.5 KB (19501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf867d1d754cc74aa694ac1fe2302a247de2ef523e65acb29269f8d62549e6dc`  
		Last Modified: Thu, 11 Nov 2021 06:22:36 GMT  
		Size: 14.9 MB (14915753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ca603582a153c2e343342510bfddd9f7d4f3a015e99d30a72607f53e90410c`  
		Last Modified: Thu, 11 Nov 2021 06:22:31 GMT  
		Size: 2.4 KB (2352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7d030d2a38e0c7cd0009ef77dc30fcdf99d8e4b451f679e9f8ce7395baffa5`  
		Last Modified: Thu, 11 Nov 2021 06:22:32 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.4-apache` - linux; s390x

```console
$ docker pull wordpress@sha256:dd25c71dec3c9bb2174d23b5d432d7e592d1155b557a3092f560536e93a8f9e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.2 MB (187247798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d387483a82193a9c8fc22ae2b481e99e5e6d5eb0d8aa8e4e85349a9961c0a586`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 17 Nov 2021 02:42:27 GMT
ADD file:42f73dac307a6a5232e3100f3d3b36e8125f73a4ca504b106e60e2b66d242b2f in / 
# Wed, 17 Nov 2021 02:42:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 05:10:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 17 Nov 2021 05:10:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 17 Nov 2021 05:10:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 05:10:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 17 Nov 2021 05:10:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 17 Nov 2021 05:13:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 17 Nov 2021 05:13:27 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 17 Nov 2021 05:13:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 17 Nov 2021 05:13:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 17 Nov 2021 05:13:35 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 17 Nov 2021 05:13:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 05:13:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 17 Nov 2021 05:13:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 17 Nov 2021 05:51:42 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 15:57:26 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 15:57:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 15:57:26 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 15:57:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 18 Nov 2021 15:57:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 15:58:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 15:58:54 GMT
COPY multi:ee8b9bb4e448c5d38508b40a8ace77d14cf000229390e687b6d467283c9826e6 in /usr/local/bin/ 
# Thu, 18 Nov 2021 15:58:54 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 15:58:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 15:58:54 GMT
STOPSIGNAL SIGWINCH
# Thu, 18 Nov 2021 15:58:54 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 18 Nov 2021 15:58:55 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 15:58:55 GMT
EXPOSE 80
# Thu, 18 Nov 2021 15:58:55 GMT
CMD ["apache2-foreground"]
# Thu, 18 Nov 2021 18:41:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 18:41:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.5.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 18:41:53 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 18 Nov 2021 18:41:53 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 18 Nov 2021 18:41:54 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 18 Nov 2021 18:41:57 GMT
RUN set -eux; 	version='5.8.2'; 	sha1='c3b1b59553eafbf301c83b14c5eeae4cf1c86044'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 18 Nov 2021 18:41:58 GMT
VOLUME [/var/www/html]
# Thu, 18 Nov 2021 18:41:58 GMT
COPY --chown=www-data:www-datafile:76be5fadb2e2d2b7a74d2770397579cd1402963fdca23912220f983ef906f582 in /usr/src/wordpress/ 
# Thu, 18 Nov 2021 18:41:58 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 18 Nov 2021 18:41:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Nov 2021 18:41:58 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8d71e885edf612b507bbdcc48a970548d436b8709eeedfc2c98f6843a214b5e2`  
		Last Modified: Wed, 17 Nov 2021 02:48:25 GMT  
		Size: 29.7 MB (29650960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebdd8d18b7ab54ddb669daaba48a71baf1b3a0cb976f3fc4b5b3edf02cda5a8`  
		Last Modified: Wed, 17 Nov 2021 06:30:10 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4daa3182042feab841aef3d3a6a2463510fbe4bf9a26a3b52f442569a85f51`  
		Last Modified: Wed, 17 Nov 2021 06:30:20 GMT  
		Size: 71.6 MB (71617991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd38782fa05c1d801350f268b3b15331b42a4d1677db396470848b08df91fd8c`  
		Last Modified: Wed, 17 Nov 2021 06:30:10 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c1f597bb2393a2cd22490f07981d83b4210d87c1286d7a0c63443e2c025da5`  
		Last Modified: Wed, 17 Nov 2021 06:30:42 GMT  
		Size: 19.1 MB (19052098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6af84d908fcda7a7d0292ea6000e4a866d7b5975c0c6dafb5978cd458c3986`  
		Last Modified: Wed, 17 Nov 2021 06:30:39 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1f06d6154f302f59760587c718c597d71d72217c7b8fa91ccd1b6d4bcb23bf`  
		Last Modified: Wed, 17 Nov 2021 06:30:39 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14cbfe954e6c8c83f2fc89665e06351a90468c16daa931e0cefdb3bc9b07a2c`  
		Last Modified: Thu, 18 Nov 2021 17:11:24 GMT  
		Size: 10.8 MB (10758959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0d74e4e023b8b26a5dc7bf40758c30fe4b03588a1450d08d3133ccc2e873c2`  
		Last Modified: Thu, 18 Nov 2021 17:11:22 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2b0995e7f2d3c6c59617bdcd605d801efa779ffff4e546a6c1c0cb5e29fabd`  
		Last Modified: Thu, 18 Nov 2021 17:11:24 GMT  
		Size: 13.1 MB (13144411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4a21dffd5b66dbcae0dc0cdebd0bb253318526570e0a3827921902d35afef0`  
		Last Modified: Thu, 18 Nov 2021 17:11:22 GMT  
		Size: 2.3 KB (2313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21dbb4925b30e5be89dfac1b7e1178e97238fcfaff843a7cda1e8472f08c52d`  
		Last Modified: Thu, 18 Nov 2021 17:11:22 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80f2b1bdbcebc7c14badfe1693da5ec8ea479ce561d44be73d1759207907a24`  
		Last Modified: Thu, 18 Nov 2021 17:11:22 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4132db77c5f32bb04768f504c8494026a2fa6de04db20f736b8e6c5bf7bf7f9e`  
		Last Modified: Thu, 18 Nov 2021 18:51:59 GMT  
		Size: 18.9 MB (18907737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c540d0f820bb32abb43bc6c934aed7a2150f237585c7172b4aac21caea2a85f`  
		Last Modified: Thu, 18 Nov 2021 18:51:57 GMT  
		Size: 9.2 MB (9170119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dcbfb8ded78c4f92fa74e190b7d44a41d45753e96de4e3d76d974d5b129ca7`  
		Last Modified: Thu, 18 Nov 2021 18:51:56 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28285c6e5655b97ab6d544cc77b4ee257571c59f188ea762f1efcdf4f5d1f82`  
		Last Modified: Thu, 18 Nov 2021 18:51:55 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1152a5feb62b6edbc72dc284737e23ea00c56215dd83e8f136c178397f5a8cc`  
		Last Modified: Thu, 18 Nov 2021 18:51:55 GMT  
		Size: 19.5 KB (19495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3f12d522467fa0e0879099a9a6016689e7cefaa63aa0fdc82504cff278de90`  
		Last Modified: Thu, 18 Nov 2021 18:51:57 GMT  
		Size: 14.9 MB (14915747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdd7cb9a6576d9a6cf9cd8f9b8aad5603408a39e5b693f139c5959b359936d4`  
		Last Modified: Thu, 18 Nov 2021 18:51:55 GMT  
		Size: 2.4 KB (2353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84dfec8f3bfe322162932710a8dfe394f4cc82c62497521a349ef8837a404a00`  
		Last Modified: Thu, 18 Nov 2021 18:51:55 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
