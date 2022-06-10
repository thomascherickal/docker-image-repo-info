## `wordpress:php8.0-apache`

```console
$ docker pull wordpress@sha256:8370a738db6268005c5900edcf8d31f5dda873e60f5494c867c26d90e2e47907
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

### `wordpress:php8.0-apache` - linux; amd64

```console
$ docker pull wordpress@sha256:000bec71381916e46c4766662ad97753cb527e4f9c01487486693d7bcbe56377
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215642500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1f7b142c37d44435e094d97d526d95b7cab03fc06b024e65fbe5849d839ed4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:08:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:08:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:09:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:09:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:09:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 08:12:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 08:12:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 08:12:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 08:12:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 08:12:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:12:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 08:39:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 00:50:28 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 00:50:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 00:50:29 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 00:50:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 00:50:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:53:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 00:53:34 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:53:34 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 00:53:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 00:53:35 GMT
STOPSIGNAL SIGWINCH
# Fri, 10 Jun 2022 00:53:35 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:53:35 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 00:53:35 GMT
EXPOSE 80
# Fri, 10 Jun 2022 00:53:35 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 03:50:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 03:52:04 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 10 Jun 2022 03:52:05 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Jun 2022 03:52:05 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 10 Jun 2022 03:52:06 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 10 Jun 2022 03:52:09 GMT
RUN set -eux; 	version='6.0'; 	sha1='7a5a6d0591771e730b05c49d0c3fc134624d0491'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 10 Jun 2022 03:52:09 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 03:52:09 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Fri, 10 Jun 2022 03:52:10 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Fri, 10 Jun 2022 03:52:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Jun 2022 03:52:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8934009a9160aba4a97afe1cd14b108784c0b2c40aaf08733963f85614b048c9`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357ac116991b8f9e62b4346e8f8f8fbfc911a8675a7022102aa05bf070b4296`  
		Last Modified: Sat, 28 May 2022 09:50:10 GMT  
		Size: 91.6 MB (91603774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ae63894b5a892892f9c32ecf1277bdb7f54f7be8b8583edecdc1e527321475`  
		Last Modified: Sat, 28 May 2022 09:49:56 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772088206f8568203e6d410d3b89fbe52c179aff6abed864eb98bbb88600a463`  
		Last Modified: Sat, 28 May 2022 09:51:08 GMT  
		Size: 19.2 MB (19247884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b81c5474649ebdbc8488baf5cd66754f83eab0486a88885f482b0e7f964fdca`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62a528527ae803d0d6a51823792cd9d053c716c464e181fe3ec3d727e54bb20`  
		Last Modified: Sat, 28 May 2022 09:51:05 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8da7928e6794c3678151992e658fc20885b6d267319d4cdcefa1cf36d61f121`  
		Last Modified: Fri, 10 Jun 2022 01:42:54 GMT  
		Size: 11.2 MB (11218836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa0c876b41f525bfd65d8aa2bd90f2a21e4646fefa346f40b4c96ca4f095c05`  
		Last Modified: Fri, 10 Jun 2022 01:42:51 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf79d622325039c1d301c7152e7e9a8583852e18d82b5dbaf8e54c07b3120a52`  
		Last Modified: Fri, 10 Jun 2022 01:42:53 GMT  
		Size: 10.8 MB (10774751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff0e31f4907cc931e04204514f6ddc7dde3a008847646a34a6578f618426ae6`  
		Last Modified: Fri, 10 Jun 2022 01:42:51 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97ccd5e9d41a7718d888fc5f36bb6ae9f445ae909838a18beece388ffe13ace`  
		Last Modified: Fri, 10 Jun 2022 01:42:51 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd678d497712d7c9e108a6af8ae2158a6de7e4e39a8c24661855231097d05d7`  
		Last Modified: Fri, 10 Jun 2022 01:42:51 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2f606455234fc882bef9630036337a56584132b9c14da0d3a48d7c06ca33d3`  
		Last Modified: Fri, 10 Jun 2022 04:07:13 GMT  
		Size: 19.0 MB (18983618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c28fa9bc26730b095114de8011347c2e16dd2c0786dcd74454b76f059178c71`  
		Last Modified: Fri, 10 Jun 2022 04:07:12 GMT  
		Size: 11.4 MB (11414288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2213bb5527bd0bcbf4c12aaad74a016181a9ac14a895fb6b0a4d4ed3cb624d6`  
		Last Modified: Fri, 10 Jun 2022 04:07:09 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696e6cfc9f78df8396663318401804e638c5230865b508855465c415fc6947d1`  
		Last Modified: Fri, 10 Jun 2022 04:07:07 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961c2faba72741e50161580481cdc469232c9842550a3b0594e077944b9b03ad`  
		Last Modified: Fri, 10 Jun 2022 04:07:07 GMT  
		Size: 19.5 KB (19494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f55598275c82a8904fae9044f1a49b02ad027b34c91a5cea1b510ceb019f0f9`  
		Last Modified: Fri, 10 Jun 2022 04:07:10 GMT  
		Size: 21.0 MB (20990145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120e80d1d32a0d47e952623b61215ab3a8f40ec3efd4d0b9f63dc607791b91e3`  
		Last Modified: Fri, 10 Jun 2022 04:07:07 GMT  
		Size: 2.3 KB (2342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654aa6118c0e0f7ed1bdd751b249b1048d106277460db22ea1e40eccbbec1999`  
		Last Modified: Fri, 10 Jun 2022 04:07:07 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.0-apache` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:ab0f6529adbc0b0062d88398131e15e1b2463e0afd1dbf490a6c1a76a7c74dc0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.5 MB (191485561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880acf380ba87e99bd9da9e7a1c6619d56b880bef513fb5cb7a6ea3cbe8b2b6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 02:03:06 GMT
ADD file:d9560b279f64bc3973a6aaa0e0ab8f483d60a1c66647899850689eee01a729ec in / 
# Sat, 28 May 2022 02:03:07 GMT
CMD ["bash"]
# Sat, 28 May 2022 20:41:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 20:41:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 20:42:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 20:42:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 20:42:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 20:48:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 20:48:32 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 20:48:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 20:48:59 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 20:49:01 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 20:49:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 20:49:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 20:49:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 21:35:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 00:44:50 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 00:44:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 00:44:51 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 00:45:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 00:45:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:50:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 00:50:20 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:50:21 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 00:50:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 00:50:22 GMT
STOPSIGNAL SIGWINCH
# Fri, 10 Jun 2022 00:50:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:50:23 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 00:50:24 GMT
EXPOSE 80
# Fri, 10 Jun 2022 00:50:24 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 05:32:02 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 10 Jun 2022 05:32:04 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Jun 2022 05:32:05 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 10 Jun 2022 05:32:07 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 10 Jun 2022 05:32:17 GMT
RUN set -eux; 	version='6.0'; 	sha1='7a5a6d0591771e730b05c49d0c3fc134624d0491'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 10 Jun 2022 05:32:18 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 05:32:18 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Fri, 10 Jun 2022 05:32:19 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Fri, 10 Jun 2022 05:32:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Jun 2022 05:32:20 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:b24540c95c3d5b61dba94dfa3665e0cc1231b3602edfb61432041c1f108be50d`  
		Last Modified: Sat, 28 May 2022 02:18:37 GMT  
		Size: 28.9 MB (28921471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12cf3513616b2ea05dba65517d17dda27a1ceee04ba9287047dd04f6979c06f9`  
		Last Modified: Sat, 28 May 2022 23:50:24 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443372867141fb1f3fe996587efd00d75c4718138718a4515907898d5c1ad900`  
		Last Modified: Sat, 28 May 2022 23:51:14 GMT  
		Size: 73.7 MB (73685298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728498cc6c6df3b79ec87ce8985063790e5399f12d368c50f635e46a6816ba2e`  
		Last Modified: Sat, 28 May 2022 23:50:24 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f6d50db4989699647f4c394e9aef999773f8a496b313303ffc3c8665901e4`  
		Last Modified: Sat, 28 May 2022 23:52:34 GMT  
		Size: 18.5 MB (18545645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9f7c0f3b50b323983f84cd011c8ea4519565b27c40440a1b846f174d150fef`  
		Last Modified: Sat, 28 May 2022 23:52:23 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a503817e72acf78b1cc840aa44ee7198695c2a849e8d9edeb51cf75d4ae5f7`  
		Last Modified: Sat, 28 May 2022 23:52:23 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a49988dcfcdcc0c64ac8498e83cf7e714da4867c333329839a1fbb075a914e`  
		Last Modified: Fri, 10 Jun 2022 01:39:42 GMT  
		Size: 11.2 MB (11217636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718080e8040cd75ad1509cb514ee5ce5f419dc6bb6300c2f3aa75cb7f870c129`  
		Last Modified: Fri, 10 Jun 2022 01:39:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b459c1e73d1150a0f0ee2f7cb3652e231cdc7ea7d13d05c27164856462f0abd`  
		Last Modified: Fri, 10 Jun 2022 01:39:45 GMT  
		Size: 9.8 MB (9790378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204e6cf1ed4e7c7dc03e2cc18b84e440480ea4d646371927966bacdf23acde4a`  
		Last Modified: Fri, 10 Jun 2022 01:39:37 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e65e59fb05eb9959c808b6799c84d079e792478a9d472b7a4323abd59b9fdff`  
		Last Modified: Fri, 10 Jun 2022 01:39:37 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f166c4a1e0c07ab72b621f02733a05bb1281a6a6ab80a18c3e7640278762b39f`  
		Last Modified: Fri, 10 Jun 2022 01:39:37 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544c8f708082483f9f170109ffbfcf0fe3df05e3a78b34721e7edf8dfa274197`  
		Last Modified: Fri, 10 Jun 2022 05:53:00 GMT  
		Size: 18.6 MB (18567383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1a1386344aef26ee414abb845d93ef6eec91e38999e572ce9ffb5ebfc1d142`  
		Last Modified: Fri, 10 Jun 2022 05:52:54 GMT  
		Size: 9.7 MB (9737648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76010f9a1e91f088285ea411368b282c702ce795d48ec2070ec7f7f029fc39b1`  
		Last Modified: Fri, 10 Jun 2022 05:52:48 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663d36e94a95ab0290c8a797549d05c85678a8d62922391fee7497555482f0b2`  
		Last Modified: Fri, 10 Jun 2022 05:52:46 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3720196b8a7c8d4cbbd366901be1d5f3cf60ca0e0387506cfd88d246ea5cd133`  
		Last Modified: Fri, 10 Jun 2022 05:52:46 GMT  
		Size: 19.5 KB (19514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb606d9d4e532400e02b9752aeed9bcc7588bb586beb932755ec3d9d02cdf92`  
		Last Modified: Fri, 10 Jun 2022 05:53:00 GMT  
		Size: 21.0 MB (20990158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a15aa1a76aafec67d153b98de5eed4333e24a0c78c7ca50db5d95503715811f`  
		Last Modified: Fri, 10 Jun 2022 05:52:46 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb4b915b807661ab3324883e8bb72c81998f833b3b4541c76c545bef17f2e5a`  
		Last Modified: Fri, 10 Jun 2022 05:52:46 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.0-apache` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:f61071af6233ecf0bc2a933b7c7730ca88c41137be78a4cf287a9622a4b01dcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.3 MB (182265183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e4e34a4047e85bf72bfd9a798340aa49997f70aebd6e7df7347bda25ea53c79`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 00:59:48 GMT
ADD file:975c801b5b50aa75e07d18e69af11f21e165561abc16246e2c413c2ef96ce4c6 in / 
# Sat, 28 May 2022 00:59:49 GMT
CMD ["bash"]
# Sun, 29 May 2022 07:20:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sun, 29 May 2022 07:20:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sun, 29 May 2022 07:21:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 07:21:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sun, 29 May 2022 07:21:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sun, 29 May 2022 07:26:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sun, 29 May 2022 07:26:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sun, 29 May 2022 07:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sun, 29 May 2022 07:27:05 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sun, 29 May 2022 07:27:06 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sun, 29 May 2022 07:27:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 29 May 2022 07:27:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sun, 29 May 2022 07:27:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sun, 29 May 2022 08:12:06 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sun, 29 May 2022 08:54:55 GMT
ENV PHP_VERSION=8.0.19
# Sun, 29 May 2022 08:54:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Sun, 29 May 2022 08:54:56 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Sun, 29 May 2022 08:55:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 29 May 2022 08:55:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sun, 29 May 2022 09:00:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sun, 29 May 2022 09:00:33 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sun, 29 May 2022 09:00:34 GMT
RUN docker-php-ext-enable sodium
# Sun, 29 May 2022 09:00:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sun, 29 May 2022 09:00:35 GMT
STOPSIGNAL SIGWINCH
# Sun, 29 May 2022 09:00:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sun, 29 May 2022 09:00:36 GMT
WORKDIR /var/www/html
# Sun, 29 May 2022 09:00:37 GMT
EXPOSE 80
# Sun, 29 May 2022 09:00:37 GMT
CMD ["apache2-foreground"]
# Mon, 30 May 2022 06:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 May 2022 06:15:49 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Mon, 30 May 2022 06:15:51 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 30 May 2022 06:15:53 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Mon, 30 May 2022 06:15:55 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Mon, 30 May 2022 06:16:04 GMT
RUN set -eux; 	version='6.0'; 	sha1='7a5a6d0591771e730b05c49d0c3fc134624d0491'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Mon, 30 May 2022 06:16:04 GMT
VOLUME [/var/www/html]
# Mon, 30 May 2022 06:16:05 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Mon, 30 May 2022 06:16:05 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Mon, 30 May 2022 06:16:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 30 May 2022 06:16:06 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:eeb117569618df53320eb28d32b7a1d87792bda3362017123fa1025b55db44c3`  
		Last Modified: Sat, 28 May 2022 01:15:35 GMT  
		Size: 26.6 MB (26576237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d3aba112689c02d6b26a241e0065c97e4d937ec22a83ec2611313d531e8b0a`  
		Last Modified: Sun, 29 May 2022 10:31:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c1acd8b719bd38a8741d6d093c916a6a558e402efb4f9e8a9c0d8331959d0d`  
		Last Modified: Sun, 29 May 2022 10:31:44 GMT  
		Size: 69.3 MB (69318858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669dd875526c016d77dc484bfa38a4f856de0994a919ad17c67ba551ea39613a`  
		Last Modified: Sun, 29 May 2022 10:31:01 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b62250e8ba44edd5728ef78550f4413110a8e30299f9759013a4a2cc1895e2`  
		Last Modified: Sun, 29 May 2022 10:33:02 GMT  
		Size: 18.0 MB (17993441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ada171d9ed11a53015749eebc93e05f658d1b63f4b62423ef83f2886cb2611`  
		Last Modified: Sun, 29 May 2022 10:32:52 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f5395bf69c3010288a162f6244f829e5cff002fa2f6e52ca8ed267c3f27b64`  
		Last Modified: Sun, 29 May 2022 10:32:52 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b680272c0b514c21641af35cbf5c37fb7597fb583f84f8ddd7ab4b625caa3fd3`  
		Last Modified: Sun, 29 May 2022 10:45:07 GMT  
		Size: 11.1 MB (11117608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4fb3b30ce91806dbd7b7e9df8d3a3ddc88ac58b2479831174c068588741839`  
		Last Modified: Sun, 29 May 2022 10:45:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152359f28e87c5696587f755907814e173c55b3c58fbcaae704f28911a4992d3`  
		Last Modified: Sun, 29 May 2022 10:45:09 GMT  
		Size: 9.3 MB (9305756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4f049bd24016991fc54aed29952593de89bf7516d7ef4c3b4ad9ab0291dc55`  
		Last Modified: Sun, 29 May 2022 10:45:02 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62df8574ec8ca9a4e84626ad6d0c6b82540039289f45c58505cfb93460ba60bd`  
		Last Modified: Sun, 29 May 2022 10:45:02 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec11260cbc398ed3df848049fe60aa764a26774b30ba573e0118bc081ad87c73`  
		Last Modified: Sun, 29 May 2022 10:45:02 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd54c7f78456a7a44d11c6d5b890b9978a77d3b01832bc27fe5e757610eded2`  
		Last Modified: Mon, 30 May 2022 06:39:01 GMT  
		Size: 18.1 MB (18113932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cad62c9046f819ea4d6569e1d5b7f2dd4c2b123063bef89eb1b36960c41452`  
		Last Modified: Mon, 30 May 2022 06:38:54 GMT  
		Size: 8.8 MB (8819286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc39f74416fa547b2b27b668454ecd3d13b8a882d885432daed78a00deb42e86`  
		Last Modified: Mon, 30 May 2022 06:38:49 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f84ba08b62081a1afff1afe5a64a643a4cfe6a89435ca86377aa14150f5c8c`  
		Last Modified: Mon, 30 May 2022 06:38:47 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d8a48c9c79caa3c5378b1f0e193306d2806a7e408f8440238e30e1efc9dce1`  
		Last Modified: Mon, 30 May 2022 06:38:47 GMT  
		Size: 19.5 KB (19505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1c1f9a41d3a9d4b831ce39d0043abcd7d66287ef5efbcc3593b8ad22b0475b`  
		Last Modified: Mon, 30 May 2022 06:39:02 GMT  
		Size: 21.0 MB (20990140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd374beddaf913ad91d1490abd08260dc4b0923b03297635f680e2ffa8c60be`  
		Last Modified: Mon, 30 May 2022 06:38:47 GMT  
		Size: 2.3 KB (2339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcde85d81cae191ad382bb4a2b0e2d5418f8dd1f15af1e91eedd79bfc890784`  
		Last Modified: Mon, 30 May 2022 06:38:47 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.0-apache` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:1f83f60926c987774e9cb2c8eec184e9bf03b85a5a5217e311e02ea4ca353f67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.1 MB (206066053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2083fbdb076278350e193583a0f9ebc73eea7a0ff4e78ec8a8a3862c98f3d5ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 04:40:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 04:40:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 04:40:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 04:40:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 04:40:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 04:45:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 04:45:05 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 04:45:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 04:45:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 04:45:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 04:45:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 04:45:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 04:45:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 05:18:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 02:15:45 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 02:15:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 02:15:47 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 02:15:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 02:16:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 02:18:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 02:18:32 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 10 Jun 2022 02:18:33 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 02:18:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 02:18:34 GMT
STOPSIGNAL SIGWINCH
# Fri, 10 Jun 2022 02:18:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 10 Jun 2022 02:18:36 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 02:18:37 GMT
EXPOSE 80
# Fri, 10 Jun 2022 02:18:38 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 05:13:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 05:14:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 10 Jun 2022 05:14:53 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Jun 2022 05:14:54 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 10 Jun 2022 05:14:56 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 10 Jun 2022 05:14:59 GMT
RUN set -eux; 	version='6.0'; 	sha1='7a5a6d0591771e730b05c49d0c3fc134624d0491'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 10 Jun 2022 05:15:00 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 05:15:01 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Fri, 10 Jun 2022 05:15:02 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Fri, 10 Jun 2022 05:15:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Jun 2022 05:15:03 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57f60612e180c578a7a4978e5e3ec509e89e091d56490e890ab31c0413f7907`  
		Last Modified: Sat, 28 May 2022 06:31:07 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1687b455bba4be0b923345f633dd5dedf683b31e562d99c279245ae0386f68b2`  
		Last Modified: Sat, 28 May 2022 06:31:20 GMT  
		Size: 86.7 MB (86719287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d450e89c3c60d5fa89af649f1d70e79286f0f1f1f77330c59c5d151d2f3a0494`  
		Last Modified: Sat, 28 May 2022 06:31:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84998b35516f3d7f2e539a4ffe18540848e79bcbf7709fd3fe43b66df50cd44d`  
		Last Modified: Sat, 28 May 2022 06:32:22 GMT  
		Size: 18.9 MB (18943025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42a5e38b7d70dbd4536bd189fd964987a26c5df0bbb13331f55f1b24916e922`  
		Last Modified: Sat, 28 May 2022 06:32:19 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15f72cf0569c75117b02b41ae5148546f981267634e0eb39730186db838cc4b`  
		Last Modified: Sat, 28 May 2022 06:32:19 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2f7629fb10cfb330b010dc2c7afb988f01e018da27e75f1c1c9209d3047bd5`  
		Last Modified: Fri, 10 Jun 2022 03:11:03 GMT  
		Size: 11.0 MB (11003364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace7ba41989dfe085b9f103eccad2f388e715027c77ac70b0aad2e7c8e1543ab`  
		Last Modified: Fri, 10 Jun 2022 03:11:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778e0f3e1abbbdc8e1e9121eb7e3c8b94f173706a8cfc078b9f51085a44bdf2c`  
		Last Modified: Fri, 10 Jun 2022 03:11:18 GMT  
		Size: 10.2 MB (10231543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0304469ff2b00d2940315b206bf3175fd9f5b6d95e33fd3f6ca7e30ade80b5b6`  
		Last Modified: Fri, 10 Jun 2022 03:11:17 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502780ded633e924d129364143f5e0e01e76b2b970018db37a1fe01a821f791b`  
		Last Modified: Fri, 10 Jun 2022 03:11:26 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0b627642ad603d87eb457d5f08de66a9d9edfd84a5aed7c9613a8243358d28`  
		Last Modified: Fri, 10 Jun 2022 03:11:00 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e16eaa5363c9e77e0287e23fec4ea709b801d9d0336fb13af46ca3afd4e93a`  
		Last Modified: Fri, 10 Jun 2022 05:32:55 GMT  
		Size: 19.0 MB (18952892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40a938cd56810a26dcb6c9a4856d443dc1c028b8b49da654801c677613ea447`  
		Last Modified: Fri, 10 Jun 2022 05:32:52 GMT  
		Size: 9.1 MB (9130925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d227ab1e3dcc673b2c504be93b513cf8bc9090ea15e645f028fd43c0667dcb7`  
		Last Modified: Fri, 10 Jun 2022 05:32:51 GMT  
		Size: 377.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92d8dae27949a321095e1531b8b86c5968e42fe7e28c256b9f254d57f1536ad`  
		Last Modified: Fri, 10 Jun 2022 05:32:48 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393758ff6b4f54d971638fb75acd25c2d95135bb08f3bdb70e236c42fed3deb6`  
		Last Modified: Fri, 10 Jun 2022 05:32:48 GMT  
		Size: 19.5 KB (19494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66f0dfca682403950b9863d6057cb98657e34934fd72f370b3805ec8e8774f7`  
		Last Modified: Fri, 10 Jun 2022 05:32:52 GMT  
		Size: 21.0 MB (20989490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12982b714d7728c528eb2e9f620adad4456ebd6ebb507c43c56f564bfbe6afb1`  
		Last Modified: Fri, 10 Jun 2022 05:32:48 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3ae3cdf30a2473202cb9613acbff5dffae219cec03101fb865b61032606855`  
		Last Modified: Fri, 10 Jun 2022 05:32:49 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.0-apache` - linux; 386

```console
$ docker pull wordpress@sha256:e6a725e4930d782f148b71eef917a304db8c8b2b88059407265dc9b8276bce6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.1 MB (217145539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:443974c353738bd24cfeb9177c683f075c9c550ee05c1dc229b8c9a1fe606bec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 00:39:33 GMT
ADD file:8320d7b95b9f68313e086faff974bb38977e0c9da4984afb6382eb0405742bde in / 
# Sat, 28 May 2022 00:39:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 12:54:26 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 12:54:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 12:54:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 12:54:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 12:54:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 12:58:09 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 12:58:10 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 12:58:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 12:58:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 12:58:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 12:58:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 12:58:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 12:58:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 13:25:01 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 00:37:23 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 00:37:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 00:37:25 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 00:37:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 00:37:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:40:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 00:40:18 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:40:18 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 00:40:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 00:40:20 GMT
STOPSIGNAL SIGWINCH
# Fri, 10 Jun 2022 00:40:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 10 Jun 2022 00:40:22 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 00:40:23 GMT
EXPOSE 80
# Fri, 10 Jun 2022 00:40:24 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 04:51:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 04:52:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 10 Jun 2022 04:52:29 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Jun 2022 04:52:29 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 10 Jun 2022 04:52:30 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 10 Jun 2022 04:52:34 GMT
RUN set -eux; 	version='6.0'; 	sha1='7a5a6d0591771e730b05c49d0c3fc134624d0491'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 10 Jun 2022 04:52:35 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 04:52:36 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Fri, 10 Jun 2022 04:52:37 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Fri, 10 Jun 2022 04:52:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Jun 2022 04:52:38 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5e7494d2ee6c81c73ce32f8bde3ea8658c6224c2cc22d7bb01df4bc3d42949aa`  
		Last Modified: Sat, 28 May 2022 00:46:43 GMT  
		Size: 32.4 MB (32390321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c02a78549ec8030de8b3a962c06643d7d8ed9a217cca23d33fec7c51be6b9d`  
		Last Modified: Sat, 28 May 2022 14:39:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491b4ce327992f77619335bcb7ceb213894da2ffaf99044a3546f17bbdb5ed82`  
		Last Modified: Sat, 28 May 2022 14:39:23 GMT  
		Size: 92.5 MB (92512638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85e0a52eb6f63802a15b9900b474ab734e50c976ecef2881f270d3cec6fa5c7`  
		Last Modified: Sat, 28 May 2022 14:39:05 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee337ee34dae18b14d13efac3c4c4ff9f6225121d86f8575dbbdaf42b3830206`  
		Last Modified: Sat, 28 May 2022 14:40:26 GMT  
		Size: 19.5 MB (19501543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ebf1b1340c66a5a7ec4007bbd718e77613da64437f4d905f0cfdaf939ab276f`  
		Last Modified: Sat, 28 May 2022 14:40:22 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a2e8255d90fd6aa0249eca22a052e599e338ced71fd3f912ea4447c429ff50`  
		Last Modified: Sat, 28 May 2022 14:40:22 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e2ebda27aa82e3a72310a73bee94414b7c575fdffe8c7b15f142c1f3c6c3dd`  
		Last Modified: Fri, 10 Jun 2022 01:34:35 GMT  
		Size: 11.0 MB (11003367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5ccf6405d0ee07b6585d28a9f26572527f179fbdc73ba5ca368e4b2e34482`  
		Last Modified: Fri, 10 Jun 2022 01:34:32 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd65bf7246670eac2d11c9f3b1b2649e99b2eca6334235cc51a2523c20a5ee5`  
		Last Modified: Fri, 10 Jun 2022 01:34:33 GMT  
		Size: 11.0 MB (10978713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d73f4616512e58cd68ebb0dbbfb429a20daa9bd1d8e715daf7aed66dc1282b`  
		Last Modified: Fri, 10 Jun 2022 01:34:32 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d258fa24cb214ab7b99b1a20bc812da50dd14c20e291a878c8a393a2469f63b1`  
		Last Modified: Fri, 10 Jun 2022 01:34:32 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f71d11eb9f3255f6477b9607481b0e43407d5bc84c98b16938262a8aa035d13`  
		Last Modified: Fri, 10 Jun 2022 01:34:32 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff3be7a4658109bf031aa0f96cc09d83ca865cd1869fd7d681dba822adc9df8`  
		Last Modified: Fri, 10 Jun 2022 05:10:03 GMT  
		Size: 19.3 MB (19326519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437bd0d70fef38d0a3a7f2162aeadcd69fda4811a909756dc3cd1b8bc2b20b0e`  
		Last Modified: Fri, 10 Jun 2022 05:10:01 GMT  
		Size: 10.4 MB (10413167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8035ce1cb157d65194989400d8381a36cfff16b07c755b088228a2ca5bdd9bd0`  
		Last Modified: Fri, 10 Jun 2022 05:09:59 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e784e9acd52f5338ed7f119e326de948ae5b795803f30edebcca052c51e2371`  
		Last Modified: Fri, 10 Jun 2022 05:09:57 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd2a1aa0004d2583f8d3b5688a2a35f86df71f874e7a33ca35013a6f754570c`  
		Last Modified: Fri, 10 Jun 2022 05:09:57 GMT  
		Size: 19.5 KB (19495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691be659c5e8d25100e856d5d3cb5abf4357dbca9019c41266ddec907a98f044`  
		Last Modified: Fri, 10 Jun 2022 05:10:00 GMT  
		Size: 21.0 MB (20989483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036ad590fdb7c862e9d9183fd3017b4f9669f9827aac3714d5d5c1e4224455eb`  
		Last Modified: Fri, 10 Jun 2022 05:09:56 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fef7e48d04f1a03d0f1d53f8b1a9a9e781fe0468c2c5f18f0b5e3f2833e1c7`  
		Last Modified: Fri, 10 Jun 2022 05:09:57 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.0-apache` - linux; mips64le

```console
$ docker pull wordpress@sha256:f3cf16d7aaca3438e693cf69c82799eaeef396f95d9df509215b447dd92c45b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190100742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84b184dbf1f0447ddd2203a224c6892358f0a4f3482d8fb92a6a51a4741e64e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:11:13 GMT
ADD file:f685a156b7ddafe7bafc6fad17cc36cc8a5d6d922fc1c425656ca92266d9a98e in / 
# Sat, 28 May 2022 01:11:18 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:30:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 03:30:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 03:32:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:32:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 03:32:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 03:46:37 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 03:46:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 03:47:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 03:47:45 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 03:47:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 03:47:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 03:47:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 03:48:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 05:44:55 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 28 May 2022 07:36:55 GMT
ENV PHP_VERSION=8.0.19
# Sat, 28 May 2022 07:36:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Sat, 28 May 2022 07:37:03 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Sat, 28 May 2022 07:37:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 07:37:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 07:51:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 07:51:23 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 28 May 2022 07:51:30 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 07:51:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 07:51:37 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 May 2022 07:51:40 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 May 2022 07:51:44 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 07:51:47 GMT
EXPOSE 80
# Sat, 28 May 2022 07:51:51 GMT
CMD ["apache2-foreground"]
# Mon, 30 May 2022 06:41:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 30 May 2022 06:48:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Mon, 30 May 2022 06:49:00 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 30 May 2022 06:49:07 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Mon, 30 May 2022 06:49:15 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Mon, 30 May 2022 06:49:32 GMT
RUN set -eux; 	version='6.0'; 	sha1='7a5a6d0591771e730b05c49d0c3fc134624d0491'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Mon, 30 May 2022 06:49:37 GMT
VOLUME [/var/www/html]
# Mon, 30 May 2022 06:49:41 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Mon, 30 May 2022 06:49:45 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Mon, 30 May 2022 06:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 30 May 2022 06:49:54 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:fdea7139ce36b557a23c4b9c4255387b175f851ed0c51e1e7d78dd301c0e4da8`  
		Last Modified: Sat, 28 May 2022 01:21:35 GMT  
		Size: 29.6 MB (29641237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48ffa812cba4145b49cbbc61824a577807dfbea2e248d5216b5b1fa5d6d81b5`  
		Last Modified: Sat, 28 May 2022 10:42:22 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ee5523dfa904c61988aab187090bf4bdb8ce8a4c4b8fa903a0ae6bc67d00cc`  
		Last Modified: Sat, 28 May 2022 10:43:14 GMT  
		Size: 71.8 MB (71812105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85368acf1e84d74f279250b786757fc0fad630ccedb2cf42c99422aee2bd1097`  
		Last Modified: Sat, 28 May 2022 10:42:21 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c3d2a738e63dfed168edc3c29258832be93684258d02b06a2b24e4e6aa434`  
		Last Modified: Sat, 28 May 2022 10:44:17 GMT  
		Size: 18.9 MB (18933116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66edaf522933dedc6d868e8f08ca79a936b873e00d232920dc4c3401c31eb0b`  
		Last Modified: Sat, 28 May 2022 10:44:04 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbae8f5d7ec49c8d7b9e972935e1d7dce5fddc80dc90a2cc4852c0f4ef42974`  
		Last Modified: Sat, 28 May 2022 10:44:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b0b729ba5bb518eb4d6a82bb500c48d25c76e55d1d45a975fa05cf6aafe821`  
		Last Modified: Sat, 28 May 2022 10:53:56 GMT  
		Size: 10.9 MB (10901429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469411f9706ebba69564748fc85d33f03741fa9bbd99dff1c9c202fa0a224ff4`  
		Last Modified: Sat, 28 May 2022 10:53:51 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b521d558854d3f07d645cfb739eb68ba1d3250b6eba9b81d7943c226ecb42865`  
		Last Modified: Sat, 28 May 2022 10:53:59 GMT  
		Size: 9.9 MB (9917188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbbe758331974908f82717c032847bbf7ca6cc8b787c3aefa55eec500e7fc5d`  
		Last Modified: Sat, 28 May 2022 10:53:51 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98e6115650123ef3f55dbb1b71a1c5a8c6092c63683d7bd999f26af7228362b`  
		Last Modified: Sat, 28 May 2022 10:53:51 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6094f03f66c33a3ba10d1e290e7d14bef44812cb855ddc295283a3e822fd4a`  
		Last Modified: Sat, 28 May 2022 10:53:51 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9905557a6d583c4dcd694d41b064b5bc1aca05ae9f8d52a65d1076808cbd1a`  
		Last Modified: Mon, 30 May 2022 07:21:23 GMT  
		Size: 18.8 MB (18798424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c70f7e37aa428854c74839b8520cd610638f8937bbf29bb14a62c6e609fe2601`  
		Last Modified: Mon, 30 May 2022 07:21:15 GMT  
		Size: 9.1 MB (9077925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c857ea8cbb90d8cc221585491d78473390a3075b03ffd6d6f647d558ae1140`  
		Last Modified: Mon, 30 May 2022 07:21:08 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195ebe46d93efbb4a045a5b748250e6236b59408c725699d24be6c12ae1c05ac`  
		Last Modified: Mon, 30 May 2022 07:21:06 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab8fc5e6f0f6c54b46417d424781ab415985c150bde41fb5a27b64a772efd63`  
		Last Modified: Mon, 30 May 2022 07:21:06 GMT  
		Size: 19.5 KB (19503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0458089d25e4ac5ff48206c28eb10fd7603665db05b3befe02aceba2d9346a31`  
		Last Modified: Mon, 30 May 2022 07:21:20 GMT  
		Size: 21.0 MB (20989503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6598608b6f5cc331ace6ebff6f57a7e2b9a553ffda1867e4294d04195b48bdb`  
		Last Modified: Mon, 30 May 2022 07:21:06 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78e2c1f213f0fada0c4317739f33eb1442455768e8995adc849358f94f4efca1`  
		Last Modified: Mon, 30 May 2022 07:21:06 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.0-apache` - linux; ppc64le

```console
$ docker pull wordpress@sha256:bdaa217f3aa37eff80d10ef18334350a9142df7e34aaf110fd1eff44ff32af9a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.3 MB (216336110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7597a75e48c5a5899481d90611a73f1c0a4d8fd457606414811c1f41d1bcac53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 01:22:54 GMT
ADD file:64e264b12eed99d87380e38f36bfecd62b9bb1e5460f0242cfbc5dc76c212ead in / 
# Sat, 28 May 2022 01:22:59 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:22:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 07:22:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 07:24:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:24:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 07:24:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 07:31:54 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 07:31:58 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 07:33:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 07:33:47 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 07:33:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 07:34:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 07:34:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 07:34:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 08:33:15 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 28 May 2022 09:21:17 GMT
ENV PHP_VERSION=8.0.19
# Sat, 28 May 2022 09:21:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Sat, 28 May 2022 09:21:22 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Sat, 28 May 2022 09:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 09:22:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 09:27:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 09:27:56 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 28 May 2022 09:28:02 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 09:28:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 09:28:07 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 May 2022 09:28:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 28 May 2022 09:28:11 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 09:28:13 GMT
EXPOSE 80
# Sat, 28 May 2022 09:28:15 GMT
CMD ["apache2-foreground"]
# Sun, 29 May 2022 12:04:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 12:11:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Sun, 29 May 2022 12:11:42 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 May 2022 12:11:55 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sun, 29 May 2022 12:12:05 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Sun, 29 May 2022 12:12:18 GMT
RUN set -eux; 	version='6.0'; 	sha1='7a5a6d0591771e730b05c49d0c3fc134624d0491'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Sun, 29 May 2022 12:12:21 GMT
VOLUME [/var/www/html]
# Sun, 29 May 2022 12:12:23 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Sun, 29 May 2022 12:12:24 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Sun, 29 May 2022 12:12:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sun, 29 May 2022 12:12:30 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:893e245a8f6219935016f2dd4422ec4b7fdab43d98ba29c024ec0d9ce57794ba`  
		Last Modified: Sat, 28 May 2022 01:32:28 GMT  
		Size: 35.3 MB (35286698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d642c3f5450a6405bbf9bc2437851b0fead8c5637c2187c3d0138aa4c80ebf`  
		Last Modified: Sat, 28 May 2022 10:59:01 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84dd41b6c195f84ab156bcf8fb6794ba7e3f25a1e949fc8dc500f0fd4caa4d3c`  
		Last Modified: Sat, 28 May 2022 10:59:18 GMT  
		Size: 86.6 MB (86628797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79723c6985ec0cb8d1a54a87d5714b293a1e9dbe5567d6d4997e28bdc5912ae`  
		Last Modified: Sat, 28 May 2022 10:59:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e0270a468d05d41f30ddf04051d086d4528a9b240c6d52b84f62b2691c1b9`  
		Last Modified: Sat, 28 May 2022 11:00:41 GMT  
		Size: 20.5 MB (20453663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caba973368705adc128b5c684f3d2221235aa63251fecf82373e06da2744d66d`  
		Last Modified: Sat, 28 May 2022 11:00:32 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffa81ec6ac60ca20f4c4555267b30d184806baed8e9526466f1fc6a38c2fb0c`  
		Last Modified: Sat, 28 May 2022 11:00:32 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e05963d2c767af668984500cbc05fadb10db92439293ecc05dcd340430d2924`  
		Last Modified: Sat, 28 May 2022 11:09:30 GMT  
		Size: 11.1 MB (11119131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402805e963cc17ffc7a22ee85d8b17d1e4e04a56d50c2d9567a2499a890b2313`  
		Last Modified: Sat, 28 May 2022 11:09:27 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7551a0f49532a0f59289f97836f0f57660e77caccfc036e1d5bb94d21902873`  
		Last Modified: Sat, 28 May 2022 11:09:29 GMT  
		Size: 11.1 MB (11137054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f7d03b3895b25210375120e9dd715650ee548d2a416f0d83c0479fe87762e5`  
		Last Modified: Sat, 28 May 2022 11:09:27 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00d47efb575ebf12caadadb3b2e8ae436fb3c9dfa475ceca5a349600378bccd`  
		Last Modified: Sat, 28 May 2022 11:09:27 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16af87430d56cb1b7678015327b650b1fd2f78e30e073a10062c6a06e171e02b`  
		Last Modified: Sat, 28 May 2022 11:09:27 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be01da2432f09c41ee71e23efc0fdfcd2b6e1e60ac256e2e108c770584929f4`  
		Last Modified: Sun, 29 May 2022 12:43:36 GMT  
		Size: 19.8 MB (19823716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80908622cdaa64a92bece428a29cdd14134b5ab365db733ea89368f871288b3e`  
		Last Modified: Sun, 29 May 2022 12:43:33 GMT  
		Size: 10.9 MB (10866970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10f8dd0bd7a5c1a857c0a70f48dc1a21226ab65c6827f16f769b1ea9858bc82`  
		Last Modified: Sun, 29 May 2022 12:43:30 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f974e20139eca301f92410b50ebaabc36cfb4ddec9cc42df0119b742c0ed02d6`  
		Last Modified: Sun, 29 May 2022 12:43:27 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e35399b19044466fb9f15c55ba6b8da3d83e2abd429f78fee812830de0211d3`  
		Last Modified: Sun, 29 May 2022 12:43:27 GMT  
		Size: 19.5 KB (19505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0fa08329b82769f2fdde7179e3bba9e252ba3e193ec623ed29025caed27be5`  
		Last Modified: Sun, 29 May 2022 12:43:30 GMT  
		Size: 21.0 MB (20990146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cef40a6a0d5d79959798d915e12466da91a195fb9fc9d6f7dbef45f4ce37d5`  
		Last Modified: Sun, 29 May 2022 12:43:27 GMT  
		Size: 2.3 KB (2342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a8bdea8df65d6edc701dbe5b45c3f403b220d4a515d720b610b923ec9c5139`  
		Last Modified: Sun, 29 May 2022 12:43:27 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.0-apache` - linux; s390x

```console
$ docker pull wordpress@sha256:eadd8abd014b06f1bd3b1c8a9b5eff0d356f754de156e48bb85003a9e0ddec45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.8 MB (190797482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b93169b36e61f8aacb4dedbb95072a366b2428b54ce91b820286ff6cfa501c5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 28 May 2022 00:43:00 GMT
ADD file:95dc6dcd4ebd15b42beaf935d91adafb0ea44a443bb44597bc1ff236e831ce18 in / 
# Sat, 28 May 2022 00:43:03 GMT
CMD ["bash"]
# Sat, 28 May 2022 16:09:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 16:10:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 16:10:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 16:10:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 16:10:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 16:16:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 28 May 2022 16:16:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 28 May 2022 16:17:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 28 May 2022 16:17:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 28 May 2022 16:17:23 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 28 May 2022 16:17:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 16:17:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 16:17:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 16:59:17 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 10 Jun 2022 01:05:42 GMT
ENV PHP_VERSION=8.0.20
# Fri, 10 Jun 2022 01:05:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.20.tar.xz.asc
# Fri, 10 Jun 2022 01:05:43 GMT
ENV PHP_SHA256=973fec765336ee01f47536a5db1c2eee98df9d34a41522b7b6c760159bf0a77b
# Fri, 10 Jun 2022 01:06:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 10 Jun 2022 01:06:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 01:10:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 01:10:18 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 10 Jun 2022 01:10:18 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 01:10:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 01:10:19 GMT
STOPSIGNAL SIGWINCH
# Fri, 10 Jun 2022 01:10:19 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 10 Jun 2022 01:10:19 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:10:19 GMT
EXPOSE 80
# Fri, 10 Jun 2022 01:10:19 GMT
CMD ["apache2-foreground"]
# Fri, 10 Jun 2022 05:15:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Jun 2022 05:16:48 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 10 Jun 2022 05:16:50 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Jun 2022 05:16:50 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 10 Jun 2022 05:16:51 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 10 Jun 2022 05:16:55 GMT
RUN set -eux; 	version='6.0'; 	sha1='7a5a6d0591771e730b05c49d0c3fc134624d0491'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 10 Jun 2022 05:16:56 GMT
VOLUME [/var/www/html]
# Fri, 10 Jun 2022 05:16:57 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Fri, 10 Jun 2022 05:16:57 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Fri, 10 Jun 2022 05:16:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Jun 2022 05:16:57 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f7bb6d2d11c3060ba2e66ba762e2aa10a0d1d361cfa6a806bcf26a64cc3a79aa`  
		Last Modified: Sat, 28 May 2022 00:49:46 GMT  
		Size: 29.7 MB (29655258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47e439a4381bc90946be2559c7afda81b0167e9737ff78feb342c01b2f71137`  
		Last Modified: Sat, 28 May 2022 19:04:47 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e731871658790a1839d3b135f76c62d3c42dcfe04bcd88e657460235dfdd56`  
		Last Modified: Sat, 28 May 2022 19:04:56 GMT  
		Size: 71.6 MB (71623152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4d70c4df3a2e37ece08f89d98c9e3864f9e96559baa39c6eca54cf9b6d109c`  
		Last Modified: Sat, 28 May 2022 19:04:47 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99e83e9582ec8219fdb45795c9b77a240131fe5ffda7107300bb96e9baaae2e`  
		Last Modified: Sat, 28 May 2022 19:05:44 GMT  
		Size: 19.1 MB (19053999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb19530daba1826ebe43f162fe297936828e76bdaa6ff42ee7ff78a8946b886b`  
		Last Modified: Sat, 28 May 2022 19:05:41 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18dfcdf8b0a326dff2523b3acca1fc469ea9c79274726e6e88c3a17a1e50963`  
		Last Modified: Sat, 28 May 2022 19:05:41 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982529954b9c5476aa1c45a21de21f88b30e068ff6d53b18f42de22aeb995bbc`  
		Last Modified: Fri, 10 Jun 2022 02:12:16 GMT  
		Size: 11.2 MB (11218047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2ac7483508dbcc5a82b66e3c9c38a21d21ffda04c8569d46e81e4889198f3c`  
		Last Modified: Fri, 10 Jun 2022 02:12:14 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:468c191b70230f37a84335a6139193ab5268156cbcfa5aba8b867a0abab6abb0`  
		Last Modified: Fri, 10 Jun 2022 02:12:16 GMT  
		Size: 9.9 MB (9922968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6110bc43ed84a9488f1c4657bf7b519d203a06c26332927763bab23b93b87db`  
		Last Modified: Fri, 10 Jun 2022 02:12:14 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6da79738ff4f5bdea04163b7d0b3f321b6132042969b658fb44f04a76ba418a`  
		Last Modified: Fri, 10 Jun 2022 02:12:14 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1b0fea0ce02bd1dc5c469e38748d883180b788a2b833b5d9c78de5a99fbfb1`  
		Last Modified: Fri, 10 Jun 2022 02:12:14 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1d14ade202fc9f9d5cb579a65664ed2e92c273c39f12ae4a1e94bbbd346e7e`  
		Last Modified: Fri, 10 Jun 2022 05:31:23 GMT  
		Size: 18.9 MB (18908533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c151743620bcfd4771ad9e2317e75a1c54a4c2527987a2805c01f72667247cc6`  
		Last Modified: Fri, 10 Jun 2022 05:31:21 GMT  
		Size: 9.4 MB (9395467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf5995200e5e032785317fcb5e160f86c1d1cbe32f2b27d4c210f51fdb6d388`  
		Last Modified: Fri, 10 Jun 2022 05:31:20 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3da4250b98d8f04421afaad13be738bba00f152cb31210d5b5a565e465d381`  
		Last Modified: Fri, 10 Jun 2022 05:31:18 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2217bc54bf5bc3ec22f831c0a55740e4f4fe3b8949a19aac7bef701f7a74da1b`  
		Last Modified: Fri, 10 Jun 2022 05:31:18 GMT  
		Size: 19.5 KB (19501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2684f6bb3610c2ed234964eaefb38e0acbf3b8f030465e1f4e22d30d30527924`  
		Last Modified: Fri, 10 Jun 2022 05:31:21 GMT  
		Size: 21.0 MB (20990139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48f0f93a4415023a02ed5620fa5b97f8d329c908109dddc79d5c76851a2d3f6`  
		Last Modified: Fri, 10 Jun 2022 05:31:18 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ecedfe95cc1c3887b28a08faf4f18d8410ac6e37ef3ec88cab47830c3ef1bf9`  
		Last Modified: Fri, 10 Jun 2022 05:31:18 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
