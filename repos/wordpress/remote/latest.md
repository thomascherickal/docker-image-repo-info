## `wordpress:latest`

```console
$ docker pull wordpress@sha256:d99da8858fc8c19ade40a059af332c805e0ee92f777995a10e0de82f015b3db1
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

### `wordpress:latest` - linux; amd64

```console
$ docker pull wordpress@sha256:699b44ae55bbf1ee577d0ddcbda4891ee1723088f7c413187abf74f86966e7b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.2 MB (188208909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c47f1587bb103310dce926f543bbb6f7c8078753566a3c669e2f6bcdc2c85a04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 11 Dec 2020 02:06:10 GMT
ADD file:3a7bff4e139bcacc5831fd70a035c130a91b5da001dd91c08b2acd635c7064e8 in / 
# Fri, 11 Dec 2020 02:06:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 07:15:52 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 07:15:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 07:16:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 07:16:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 07:16:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 07:25:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 11 Dec 2020 07:25:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 11 Dec 2020 07:25:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 11 Dec 2020 07:25:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 11 Dec 2020 07:25:59 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 11 Dec 2020 07:25:59 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 11 Dec 2020 07:25:59 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 11 Dec 2020 07:26:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 07:26:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 07:26:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 08:20:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:23:59 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:23:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:24:00 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:24:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jan 2021 17:24:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:27:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 17:27:06 GMT
COPY multi:dc714d093d9a94baf082b278964398d495faeef837d3357693090c43ebfb6fb4 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:27:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 17:27:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 17:27:07 GMT
STOPSIGNAL SIGWINCH
# Thu, 07 Jan 2021 17:27:07 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:27:08 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 17:27:08 GMT
EXPOSE 80
# Thu, 07 Jan 2021 17:27:08 GMT
CMD ["apache2-foreground"]
# Fri, 08 Jan 2021 00:20:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 00:22:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 00:22:13 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 08 Jan 2021 00:22:14 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 08 Jan 2021 00:22:15 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 08 Jan 2021 00:22:24 GMT
RUN set -eux; 	version='5.6'; 	sha1='db8b75bfc9de27490434b365c12fd805ca6784ce'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 08 Jan 2021 00:22:24 GMT
VOLUME [/var/www/html]
# Fri, 08 Jan 2021 00:22:25 GMT
COPY file:21c61c8c5411c6f288a3a044c8f9622540460def171cd20ff6e83aa721350821 in /usr/local/bin/ 
# Fri, 08 Jan 2021 00:22:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Jan 2021 00:22:25 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6ec7b7d162b24bd6df88abde89ceb6d7bbc2be927f025c9dd061af2b0c328cfe`  
		Last Modified: Fri, 11 Dec 2020 02:12:26 GMT  
		Size: 27.1 MB (27099295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db606474d60ce31604505c7d6dad9a66cb42f3818fca738832db2f2091cf89c9`  
		Last Modified: Fri, 11 Dec 2020 12:04:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb30f0cd8e0ff78b5eecdc2d9365a50441ad83c5db5f1e87942d6426237fa56`  
		Last Modified: Fri, 11 Dec 2020 12:04:17 GMT  
		Size: 76.7 MB (76652169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb2e805159413e5278b859f7fbb86ddfc99e667cb705d5d5aec0a7c8ffcf1b5`  
		Last Modified: Fri, 11 Dec 2020 12:04:00 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c761b44e2ccbff3f10b254b21bb00a52dfd26919ad9e3f7efcd569196e6c26b`  
		Last Modified: Fri, 11 Dec 2020 12:04:46 GMT  
		Size: 18.7 MB (18678264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2199db96575122fd559c29b619a2773fe9069e0266312a6369ac95f4464b1dd`  
		Last Modified: Fri, 11 Dec 2020 12:04:42 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a9381eea8f93068e8043f18ea59b709c07256e2f90962931a1433fbdf5e79`  
		Last Modified: Fri, 11 Dec 2020 12:04:40 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f0689715a35c9729fe1b9ef2979d9b52830b4ee23a2fbbfe7956413307c2e5`  
		Last Modified: Thu, 07 Jan 2021 20:29:55 GMT  
		Size: 10.7 MB (10664655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6cc018dd458111427b637b37fec610eb011ad61616091c0bbf7d14ba54ced0`  
		Last Modified: Thu, 07 Jan 2021 20:29:54 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052299cf2d767f7ec4092cd723fc3b9d85975385d3347229b569f5f9428adac5`  
		Last Modified: Thu, 07 Jan 2021 20:29:54 GMT  
		Size: 13.8 MB (13830470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee83da709c8837204eaf072be1528f4b3d1c9ef5fd2ee1af9bd4e818a0aa44b7`  
		Last Modified: Thu, 07 Jan 2021 20:29:53 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b10df91e6d088efaf8c6eeee0b52da35a4700c85cc145f4135dcd65d6611e6f`  
		Last Modified: Thu, 07 Jan 2021 20:29:53 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2eb858e27d81408bb396428a4230e49dda55781fdd8160d6b9e911f77a2542b`  
		Last Modified: Thu, 07 Jan 2021 20:29:53 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6269830d5ad26b8ebf468c835cfd26d1a8cb05b1e80e6fa2782bc5bc16d6f7d`  
		Last Modified: Fri, 08 Jan 2021 00:34:51 GMT  
		Size: 16.7 MB (16704744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228a0fa8a95f67f24ee7ab16476021f477b1e9a0f43fed076b1870de01d6b5df`  
		Last Modified: Fri, 08 Jan 2021 00:34:49 GMT  
		Size: 9.3 MB (9282756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f7abe863327e0a690269977b526713a8c0d140011ff134366248e18a7ce011`  
		Last Modified: Fri, 08 Jan 2021 00:34:44 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d3e1e4145ff26f09b149b4e5f4dec26eeeba1e034e56e0dbb9eaf7eb7c0bb`  
		Last Modified: Fri, 08 Jan 2021 00:34:44 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75d27a32f14ef51bdc4475b41df652eea8a2f3cf928dc3bdbf22025af7c0eb9`  
		Last Modified: Fri, 08 Jan 2021 00:34:44 GMT  
		Size: 19.5 KB (19473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c632295f58ef1b57efd83f40be84ead6e4e725ed3f9d34f62a5ed45ab5d96fc`  
		Last Modified: Fri, 08 Jan 2021 00:35:01 GMT  
		Size: 15.3 MB (15267063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84352e3067919d20304875150a2e707a731833a52f013b3a5611ba85f188f1fe`  
		Last Modified: Fri, 08 Jan 2021 00:34:44 GMT  
		Size: 4.0 KB (3965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:latest` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:d289a6537b555cd23b65e413c7e97e5ef2b8bad18c1978d2afc321522ac6576c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.0 MB (164979727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70409d128c88d3108188a8da2c2f69341c0028f7a4803fd1895bdd46167975a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 07:13:03 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 07:13:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 07:13:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 07:13:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 07:13:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 07:18:17 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 11 Dec 2020 07:18:18 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 11 Dec 2020 07:18:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 11 Dec 2020 07:18:45 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 11 Dec 2020 07:18:48 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 11 Dec 2020 07:18:48 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 11 Dec 2020 07:18:49 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 11 Dec 2020 07:18:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 07:18:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 07:18:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 07:38:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:53:22 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:53:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:53:24 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:53:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jan 2021 17:53:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:57:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 17:57:29 GMT
COPY multi:dc714d093d9a94baf082b278964398d495faeef837d3357693090c43ebfb6fb4 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:57:32 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 17:57:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 17:57:35 GMT
STOPSIGNAL SIGWINCH
# Thu, 07 Jan 2021 17:57:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:57:38 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 17:57:39 GMT
EXPOSE 80
# Thu, 07 Jan 2021 17:57:40 GMT
CMD ["apache2-foreground"]
# Thu, 07 Jan 2021 21:44:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 00:05:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 00:05:54 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 08 Jan 2021 00:05:57 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 08 Jan 2021 00:06:00 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 08 Jan 2021 00:06:09 GMT
RUN set -eux; 	version='5.6'; 	sha1='db8b75bfc9de27490434b365c12fd805ca6784ce'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 08 Jan 2021 00:06:11 GMT
VOLUME [/var/www/html]
# Fri, 08 Jan 2021 00:06:12 GMT
COPY file:21c61c8c5411c6f288a3a044c8f9622540460def171cd20ff6e83aa721350821 in /usr/local/bin/ 
# Fri, 08 Jan 2021 00:06:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Jan 2021 00:06:16 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed9b2f20ffb0bcade877c21585737821b1abdd1b29ec2742ef3d8bc1a8a71b2`  
		Last Modified: Fri, 11 Dec 2020 09:10:11 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086596dbe8ce93733486082312fbe0cffefc063795aa2ae18459ce018c64bd`  
		Last Modified: Fri, 11 Dec 2020 09:10:30 GMT  
		Size: 58.8 MB (58801419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5a47fff6f79bd0fed3070e2cbe30a88324dcd19c6597080333fabbf9adf49d`  
		Last Modified: Fri, 11 Dec 2020 09:10:09 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4517107dffe6fc5dcbf76387b03c5f0f2ced48e2b48178cd9b615f3a2b13bc8`  
		Last Modified: Fri, 11 Dec 2020 09:11:08 GMT  
		Size: 18.0 MB (18026228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d52419e1d1b4bfe2b0d4c2c5225b6fd7fe59bba8acb8b28c697658bfb7365c`  
		Last Modified: Fri, 11 Dec 2020 09:11:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca7d691aeaf537d2c7d897bb473aec13e1f708157f08c95460271ad428a1011`  
		Last Modified: Fri, 11 Dec 2020 09:11:03 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e4b6fedeea5fad8ab65b767d8093337929f321898dd151faa6a48b54319afe`  
		Last Modified: Thu, 07 Jan 2021 18:49:28 GMT  
		Size: 10.7 MB (10662660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3d337e99c74a984c1db333dd2e72e9489ec6f1122f0bd5b473dbcbaf34fd2d`  
		Last Modified: Thu, 07 Jan 2021 18:49:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3949502f795417b8431271829b112a6fb4d9bc710b72e1a93da5aa956716027`  
		Last Modified: Thu, 07 Jan 2021 18:49:28 GMT  
		Size: 12.9 MB (12905361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d15a67dc4c9ad4aff1e88139aa9c5a627cf4465fc7585a0550048f583b885e`  
		Last Modified: Thu, 07 Jan 2021 18:49:23 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f1841d90a908f7e1c91156840681e00572e2d6421ec5ef85882d0eb383898e`  
		Last Modified: Thu, 07 Jan 2021 18:49:23 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36b340b040d9c6ed5f14c19b98c3d84a5ed083c8e6c1f119ddb40391e496eef`  
		Last Modified: Thu, 07 Jan 2021 18:49:23 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85aad139d3b3dc0a451426cf22880e2e3135a09fb9d0d42d5e44588b6a73e9df`  
		Last Modified: Thu, 07 Jan 2021 21:54:35 GMT  
		Size: 16.3 MB (16283203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c618f3a335a79c8924c179f5e24fcc24224aba79e0f22162fd5ecb06d80432f`  
		Last Modified: Fri, 08 Jan 2021 00:18:11 GMT  
		Size: 8.2 MB (8160664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd62f7d138f97e906ec3a35a74889916cd9627acd5bf1cf7c99ac031a6c0cef`  
		Last Modified: Fri, 08 Jan 2021 00:18:06 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3defc02c7d2bd1ceece67a4d2f7ebec218c6ca80c3307f3a5321591b81ac3a58`  
		Last Modified: Fri, 08 Jan 2021 00:18:06 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fa443a2baaf315adcc963a59071a3cb1e4fe3c86068b94f06468d6b72506e6`  
		Last Modified: Fri, 08 Jan 2021 00:18:07 GMT  
		Size: 19.5 KB (19476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0460c070c20c6d2b5d481e618a9b6a95f2c54aceb1b7756b4cca320251980eae`  
		Last Modified: Fri, 08 Jan 2021 00:18:12 GMT  
		Size: 15.3 MB (15267121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74ecfd53e42e19ddf4fdb3016859a6d5c0b500100db1ec529c041b483771c2c`  
		Last Modified: Fri, 08 Jan 2021 00:18:06 GMT  
		Size: 4.0 KB (3964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:latest` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:edb9fc07a9288f1084a7f1b3303897da86ced3095f4c9aa53868b53d8f3891d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161051822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d54e96329815a24640a75084972a604e5102757ee46c44c897abd48fdd72fe39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 11 Dec 2020 02:23:37 GMT
ADD file:75ca842ac2d6e9f6617bb3df280af1e4c9619c9805fd5e00c1c3d6b8b4e3d802 in / 
# Fri, 11 Dec 2020 02:23:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:45:55 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 06:45:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 06:47:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 06:47:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 06:47:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 06:50:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 11 Dec 2020 06:50:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 11 Dec 2020 06:51:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 11 Dec 2020 06:51:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 11 Dec 2020 06:51:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 11 Dec 2020 06:51:18 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 11 Dec 2020 06:51:19 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 11 Dec 2020 06:51:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 06:51:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 06:51:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 07:16:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:11:20 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:11:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:11:22 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:11:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jan 2021 17:11:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:14:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 17:14:03 GMT
COPY multi:dc714d093d9a94baf082b278964398d495faeef837d3357693090c43ebfb6fb4 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:14:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 17:14:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 17:14:06 GMT
STOPSIGNAL SIGWINCH
# Thu, 07 Jan 2021 17:14:07 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:14:08 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 17:14:08 GMT
EXPOSE 80
# Thu, 07 Jan 2021 17:14:09 GMT
CMD ["apache2-foreground"]
# Thu, 07 Jan 2021 22:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 00:56:58 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 00:57:05 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 08 Jan 2021 00:57:08 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 08 Jan 2021 00:57:11 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 08 Jan 2021 00:57:18 GMT
RUN set -eux; 	version='5.6'; 	sha1='db8b75bfc9de27490434b365c12fd805ca6784ce'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 08 Jan 2021 00:57:21 GMT
VOLUME [/var/www/html]
# Fri, 08 Jan 2021 00:57:22 GMT
COPY file:21c61c8c5411c6f288a3a044c8f9622540460def171cd20ff6e83aa721350821 in /usr/local/bin/ 
# Fri, 08 Jan 2021 00:57:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Jan 2021 00:57:24 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c06905228d4fc5a5c840a70e2e6ced56596a8bc73abc69e6a1867bbb6f7ae7e7`  
		Last Modified: Fri, 11 Dec 2020 02:33:07 GMT  
		Size: 22.7 MB (22707662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff29bbfe5a8a35c816e943e30889f192df4e12d1b4c03a36540c0e4d40bcf3e8`  
		Last Modified: Fri, 11 Dec 2020 09:16:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01e4ef0e8e22e1ca2287988849c31e36c883039c399efe7cc63b9bfe617dfa7`  
		Last Modified: Fri, 11 Dec 2020 09:16:35 GMT  
		Size: 59.5 MB (59508954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c032054d75502633be18567f6e069e007d492b2bcb340991656015ae61b9e28`  
		Last Modified: Fri, 11 Dec 2020 09:16:15 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd024b01ae978f65f5eca3f392865e98a1d1d7f75d63595bb70730417f7dd0ac`  
		Last Modified: Fri, 11 Dec 2020 09:17:13 GMT  
		Size: 17.5 MB (17481707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bb823d44c0ee717bb9f076d7046d1b990d85d3ce4c6a35e760fc4b75618228`  
		Last Modified: Fri, 11 Dec 2020 09:17:09 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f96022462b744f8f7af417b0189d26064f72fb6c3f25565ccfb590e0c38af87e`  
		Last Modified: Fri, 11 Dec 2020 09:17:09 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beef19ca306c7e021f3931136d2f3945928be7f2ebe0f3e62038ba72da3ecfe2`  
		Last Modified: Thu, 07 Jan 2021 18:40:16 GMT  
		Size: 10.7 MB (10662630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72909301bfcfd6cfae4b77ae3fa04e78a9285e5c0020cc46e4eb17ee9d9c9151`  
		Last Modified: Thu, 07 Jan 2021 18:40:11 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71deec2d9842937739fa068018836a495a3ac975cb75ac6dc09474d726843837`  
		Last Modified: Thu, 07 Jan 2021 18:40:17 GMT  
		Size: 12.2 MB (12206364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e17c256d6751afe6c9c78cb7680df1dbb16507e6ca7ffd4a287497dae914eda`  
		Last Modified: Thu, 07 Jan 2021 18:40:13 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b53c168b188e6768c2ce0e10d70911761bfc54c2b28a734538b37125514c1a`  
		Last Modified: Thu, 07 Jan 2021 18:40:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c6a816e8e89759ce5de261fa5e50202f42843a7947812a2e99fa81f3411e77`  
		Last Modified: Thu, 07 Jan 2021 18:40:11 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:099af3f51e7271a4e44f5753ba3ab0794f4f0ef381278234f4d2e3f5447270e4`  
		Last Modified: Thu, 07 Jan 2021 22:58:10 GMT  
		Size: 15.9 MB (15857443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d6d8bf2258088de13ca5f1892469ce3fcd4a1a544e544b7c46533158979afdc`  
		Last Modified: Fri, 08 Jan 2021 01:13:52 GMT  
		Size: 7.3 MB (7330337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9637b167e1d55a72ed03d0e2f18037fd4e366d3e208e7dc0a06ffa2e063896d4`  
		Last Modified: Fri, 08 Jan 2021 01:13:49 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29d58b0b8ef95e2bb04cb0ecf16e1797a37fc92ff0597f14c5240b515209def`  
		Last Modified: Fri, 08 Jan 2021 01:13:49 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b046e9a8873768f2e3e7f56a9c890f061532cf5828b30cb7e900790fbb194662`  
		Last Modified: Fri, 08 Jan 2021 01:13:48 GMT  
		Size: 19.5 KB (19479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ddf528adc82d7ec92dc77bce5ab295c067af67d396c78995045482d4a43b7c`  
		Last Modified: Fri, 08 Jan 2021 01:13:55 GMT  
		Size: 15.3 MB (15267122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84c57854e5b5cace5c16525e1ad4899b4f1083f0838c10daeccd4cbef7cc3a1`  
		Last Modified: Fri, 08 Jan 2021 01:13:52 GMT  
		Size: 4.0 KB (3964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:latest` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:81150120ab9aa447e1e28d972852788e39035c7c1f5e3bcc43782d19eba0a30b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178703064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa391b024db56ce37d0102cae5a593e54b8942042fa30984989ddfa385a7908c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 11 Dec 2020 02:45:53 GMT
ADD file:a5a2f039c00bc638b88cefdff4c3cd1865b4d415bf80c4fe6b496d975af7cc1f in / 
# Fri, 11 Dec 2020 02:45:57 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 09:33:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 09:33:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 09:33:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 09:33:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 09:33:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 09:37:52 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 11 Dec 2020 09:37:53 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 11 Dec 2020 09:38:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 11 Dec 2020 09:38:19 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 11 Dec 2020 09:38:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 11 Dec 2020 09:38:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 11 Dec 2020 09:38:23 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 11 Dec 2020 09:38:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 09:38:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 09:38:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 10:05:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:49:54 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:49:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:49:57 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:50:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jan 2021 17:50:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:54:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 17:54:13 GMT
COPY multi:dc714d093d9a94baf082b278964398d495faeef837d3357693090c43ebfb6fb4 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:54:16 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 17:54:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 17:54:19 GMT
STOPSIGNAL SIGWINCH
# Thu, 07 Jan 2021 17:54:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:54:22 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 17:54:23 GMT
EXPOSE 80
# Thu, 07 Jan 2021 17:54:24 GMT
CMD ["apache2-foreground"]
# Thu, 07 Jan 2021 23:23:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 01:17:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 01:17:31 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 08 Jan 2021 01:17:33 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 08 Jan 2021 01:17:36 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 08 Jan 2021 01:17:41 GMT
RUN set -eux; 	version='5.6'; 	sha1='db8b75bfc9de27490434b365c12fd805ca6784ce'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 08 Jan 2021 01:17:43 GMT
VOLUME [/var/www/html]
# Fri, 08 Jan 2021 01:17:44 GMT
COPY file:21c61c8c5411c6f288a3a044c8f9622540460def171cd20ff6e83aa721350821 in /usr/local/bin/ 
# Fri, 08 Jan 2021 01:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Jan 2021 01:17:45 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c9648d7fcbb6d597cf33916d8fcd207fde8ec05d764b4480d4f3e884e142a902`  
		Last Modified: Fri, 11 Dec 2020 02:53:14 GMT  
		Size: 25.9 MB (25856191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88cecc04e76783f0006b9fed72be749e834825383e941e16de2565a0e4a8cc3`  
		Last Modified: Fri, 11 Dec 2020 11:57:47 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30eb7a300f132babe7d5ed65f9e81a1fdd4542ecf70ac29a91bc290484dbc5e5`  
		Last Modified: Fri, 11 Dec 2020 11:58:04 GMT  
		Size: 70.3 MB (70338279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c17a0a78e91d3ac0ec4a0c0566f57580154ead8d8967258efe94989d86cd05bd`  
		Last Modified: Fri, 11 Dec 2020 11:57:46 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d436d7bb0262f042a9554b5c54b25bc1d19cabbb9435747672c34d12f8dc1d0`  
		Last Modified: Fri, 11 Dec 2020 11:58:40 GMT  
		Size: 18.6 MB (18579888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5543a36f8eed548f436944bf39a2e918115fc9b30b54416c1081566f25716010`  
		Last Modified: Fri, 11 Dec 2020 11:58:35 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28135fd83ed1ac66e6f4288fabe4c84616cfe420e8e6808ba92d052771325ab4`  
		Last Modified: Fri, 11 Dec 2020 11:58:35 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf988abef866f04f29a3c0774107ddc1b04e93dcf63185d136eb21efc3a786`  
		Last Modified: Thu, 07 Jan 2021 19:31:00 GMT  
		Size: 10.7 MB (10663420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97375a43613218ba66a34e88eb91b851147488fc46327656a3364e6b4f4a0b5a`  
		Last Modified: Thu, 07 Jan 2021 19:30:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03791a4fe0b1d90a6cff01a973e0d558a2b0438d1b49c863914544c9037da77d`  
		Last Modified: Thu, 07 Jan 2021 19:31:00 GMT  
		Size: 13.6 MB (13609261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b7dd6f6dd70fc500653b8f9b95b8e3ca49abf3dd1d21b2662f499aefb31b1e`  
		Last Modified: Thu, 07 Jan 2021 19:30:56 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcce015f0dad73aaa4ff93a2a747e1b3b88fff1bd1c8c10ed0ae8d54962ef91`  
		Last Modified: Thu, 07 Jan 2021 19:30:56 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a251d7e17037f4e3f45a3d9d15860b5fcbd5d098cb993cdac80cb75d0f7d46`  
		Last Modified: Thu, 07 Jan 2021 19:30:56 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e09e777f40864d8219c1558b19be9ed7d6283cfa7c512d50b695d56dce03bea`  
		Last Modified: Thu, 07 Jan 2021 23:37:34 GMT  
		Size: 16.7 MB (16659592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c31cd5290aff75f79ae8fe92d180f7490f7cb59ffc1f7576b2205a8693867a`  
		Last Modified: Fri, 08 Jan 2021 01:36:06 GMT  
		Size: 7.7 MB (7699691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4ae4455ab89cc6e15f82f5bd2171ed2cb746e139386f097c960d2702d7da09`  
		Last Modified: Fri, 08 Jan 2021 01:36:00 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221f760a2058b9eb683bd30efbfdfb564a617f122d7c32f8f3df4cffc4d7a49d`  
		Last Modified: Fri, 08 Jan 2021 01:35:59 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65c96d85b550d10b7cd597773428d22bc4664283d4d134131131a37a2587821`  
		Last Modified: Fri, 08 Jan 2021 01:36:01 GMT  
		Size: 19.5 KB (19481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c290bbc5d83b10e60ea0b88f10ccbb71c120edad7b14db89c7d0a060b6314e3`  
		Last Modified: Fri, 08 Jan 2021 01:36:04 GMT  
		Size: 15.3 MB (15267125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d88989c7224f8022c4eb102424ed2bf6e40f2d4200a829ae75649062e26a1d`  
		Last Modified: Fri, 08 Jan 2021 01:36:01 GMT  
		Size: 4.0 KB (3963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:latest` - linux; 386

```console
$ docker pull wordpress@sha256:65e7e75f63846bb8d66b1e310f3cb629c61bd76638bf40e8020aa0e381f5fcc9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.8 MB (193763589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05af2b47d880433b3e96251440c6c7e5ce2ffe206ca37dedffdd67e0fd7695e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:a0879774b23f70c4db7f7b04736cca142beb0b22e93f5952364ca990a1675552 in / 
# Fri, 11 Dec 2020 02:03:08 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 06:00:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 06:00:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 06:01:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 06:01:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 06:01:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 06:07:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 11 Dec 2020 06:07:52 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 11 Dec 2020 06:08:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 11 Dec 2020 06:08:04 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 11 Dec 2020 06:08:05 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 11 Dec 2020 06:08:05 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 11 Dec 2020 06:08:05 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 11 Dec 2020 06:08:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 06:08:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 06:08:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 06:53:35 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:46:27 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:46:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:46:27 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:46:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jan 2021 17:46:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:52:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 17:52:23 GMT
COPY multi:dc714d093d9a94baf082b278964398d495faeef837d3357693090c43ebfb6fb4 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:52:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 17:52:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 17:52:24 GMT
STOPSIGNAL SIGWINCH
# Thu, 07 Jan 2021 17:52:24 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:52:25 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 17:52:25 GMT
EXPOSE 80
# Thu, 07 Jan 2021 17:52:25 GMT
CMD ["apache2-foreground"]
# Fri, 08 Jan 2021 00:39:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 00:40:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 00:40:53 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 08 Jan 2021 00:40:54 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 08 Jan 2021 00:40:55 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 08 Jan 2021 00:40:58 GMT
RUN set -eux; 	version='5.6'; 	sha1='db8b75bfc9de27490434b365c12fd805ca6784ce'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 08 Jan 2021 00:40:58 GMT
VOLUME [/var/www/html]
# Fri, 08 Jan 2021 00:40:58 GMT
COPY file:21c61c8c5411c6f288a3a044c8f9622540460def171cd20ff6e83aa721350821 in /usr/local/bin/ 
# Fri, 08 Jan 2021 00:40:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Jan 2021 00:40:59 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:cfec07a090788e68b692f30d34e11dc7af0f1c8112fbc846e8e40e24faf882d7`  
		Last Modified: Fri, 11 Dec 2020 02:09:41 GMT  
		Size: 27.8 MB (27757584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3c4afa53a59b083552d0b7595929265478f679a53088d91b97259460181159`  
		Last Modified: Fri, 11 Dec 2020 10:57:07 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8850c4c63c4455c5a9d68a8eb2fa7e2ed0a3e55da10d297894d128630a0a92`  
		Last Modified: Fri, 11 Dec 2020 10:57:33 GMT  
		Size: 81.2 MB (81196971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a53bd58246139a0a491b0e968bcac9a28e25cecbf8b243f7708f0a3ec37982`  
		Last Modified: Fri, 11 Dec 2020 10:57:06 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7a035a817d1767a780511f3cf12afa35f2f805747b61c6015ac8df6a19277b`  
		Last Modified: Fri, 11 Dec 2020 10:58:12 GMT  
		Size: 19.1 MB (19113575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e746d98cd779a9701ad7ae79a579d9d4c5dd81e50e18286995afc8e704de10d3`  
		Last Modified: Fri, 11 Dec 2020 10:58:07 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e7e181023ff3e02d359fba760e5b4ee20096f39fe53f97c6fce0fd3592a9437`  
		Last Modified: Fri, 11 Dec 2020 10:58:05 GMT  
		Size: 488.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9796f742178c9187370eac7509c4d4ce1f6a72263b3e49f8091bdaeb6af5fc5`  
		Last Modified: Thu, 07 Jan 2021 21:11:56 GMT  
		Size: 10.7 MB (10663949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6a6f330c43cda5e6aa28b1fb68bc995bbe81efb686c1c393851974d0cd1f9b`  
		Last Modified: Thu, 07 Jan 2021 21:11:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ef78ef390a29a30ba760cf4aaaa595a3f8e1bde1a4f907a9107eddc7a99b17`  
		Last Modified: Thu, 07 Jan 2021 21:12:02 GMT  
		Size: 14.2 MB (14155155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ceced1ed8ad8d5b25dfd0045c881af6c20d784bbfe9fe8fe9a43a41c27186e`  
		Last Modified: Thu, 07 Jan 2021 21:11:52 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22837edf0483dc4633fc71cb4287079699ced39bcbce59459d78de7fa374390e`  
		Last Modified: Thu, 07 Jan 2021 21:11:52 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849aefafa93d5f7a540ac4f93dc9c585d9e584dffc13bdaa08f0060015ec5259`  
		Last Modified: Thu, 07 Jan 2021 21:11:51 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaea7be005dc4a0416f84219664d9e7dce06d66f8b01a60d6ac43484f18f82c`  
		Last Modified: Fri, 08 Jan 2021 00:53:16 GMT  
		Size: 17.0 MB (17023960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8393a1ba5ab6eb66270e5cbf6bb207b4b17f584d971f68ea9583a6a20f2de327`  
		Last Modified: Fri, 08 Jan 2021 00:53:14 GMT  
		Size: 8.6 MB (8555844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e027e6725198b4b5891f0fc53aae305fc02966194132073c834854bb80d7080`  
		Last Modified: Fri, 08 Jan 2021 00:53:08 GMT  
		Size: 372.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fc489f12e9298191567c82bd65fd3a522cdeec6b9e1edbde93a88d780c85c7`  
		Last Modified: Fri, 08 Jan 2021 00:53:08 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ea38726ae0cd8a81f0fb22ca7eb681aafa5829b8c8a790a6da1f10e0240ff8`  
		Last Modified: Fri, 08 Jan 2021 00:53:08 GMT  
		Size: 19.5 KB (19471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c216e698f367d7d4edadf97ea08ee13638c5d4edeb084818cd8e08b27c4c6b11`  
		Last Modified: Fri, 08 Jan 2021 00:53:15 GMT  
		Size: 15.3 MB (15267069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd2c8b88a3893ae8b73878c1b6866172d113e33b6a35fc899fd1abfb95f6953`  
		Last Modified: Fri, 08 Jan 2021 00:53:08 GMT  
		Size: 4.0 KB (3966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:latest` - linux; mips64le

```console
$ docker pull wordpress@sha256:d930520ed93b17fd2f1c7ff38f3b05caff434f753b42a482f8e590c5304e4b4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.1 MB (169131431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8205075d9378ea3d3f78bea72fbd796fe67d16136bf952a9ef828aea390db049`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 04:25:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 04:25:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 04:26:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 04:26:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 04:26:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 04:39:30 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 11 Dec 2020 04:39:31 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 11 Dec 2020 04:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 11 Dec 2020 04:39:59 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 11 Dec 2020 04:40:01 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 11 Dec 2020 04:40:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 11 Dec 2020 04:40:02 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 11 Dec 2020 04:40:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 04:40:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 04:40:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 05:33:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:18:44 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:18:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:18:44 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:19:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jan 2021 17:19:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:26:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 17:26:56 GMT
COPY multi:dc714d093d9a94baf082b278964398d495faeef837d3357693090c43ebfb6fb4 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:26:58 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 17:26:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 17:26:59 GMT
STOPSIGNAL SIGWINCH
# Thu, 07 Jan 2021 17:26:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:27:00 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 17:27:00 GMT
EXPOSE 80
# Thu, 07 Jan 2021 17:27:00 GMT
CMD ["apache2-foreground"]
# Thu, 07 Jan 2021 21:52:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Jan 2021 23:44:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Jan 2021 23:44:42 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 07 Jan 2021 23:44:44 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Jan 2021 23:44:46 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Thu, 07 Jan 2021 23:44:55 GMT
RUN set -eux; 	version='5.6'; 	sha1='db8b75bfc9de27490434b365c12fd805ca6784ce'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 07 Jan 2021 23:44:55 GMT
VOLUME [/var/www/html]
# Thu, 07 Jan 2021 23:44:56 GMT
COPY file:21c61c8c5411c6f288a3a044c8f9622540460def171cd20ff6e83aa721350821 in /usr/local/bin/ 
# Thu, 07 Jan 2021 23:44:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Jan 2021 23:44:57 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b3d5e3fa447bed7791080d575c40219a0b0de0c2e5ead844514214998183e0`  
		Last Modified: Fri, 11 Dec 2020 06:59:42 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1851d26f0412137a20989be3bda0a0351df126006d6402dc3ded381e8c9869`  
		Last Modified: Fri, 11 Dec 2020 07:00:41 GMT  
		Size: 61.4 MB (61389791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abb65a130446f126e756b4748232dd20e059e4dfb57760a20063aad1e3ce00b`  
		Last Modified: Fri, 11 Dec 2020 06:59:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bfa578a2de0f7a16274f8531a53a1a27c5816f11cdb897425c8693e33909d9`  
		Last Modified: Fri, 11 Dec 2020 07:01:51 GMT  
		Size: 18.6 MB (18611403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00625263f216799b9bf53ae68502784b0346b27422c4c94a555aa7f6ca74a1db`  
		Last Modified: Fri, 11 Dec 2020 07:01:38 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5bc3b6b4ecace07f24d6cc7b90035a7951dbdc28b7ce79fa982597df9e07d6`  
		Last Modified: Fri, 11 Dec 2020 07:01:39 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712bf878e7f3e93b89b3d92a58e600b90c1e043c918abc3bd8bdae7846b617c3`  
		Last Modified: Thu, 07 Jan 2021 18:42:23 GMT  
		Size: 10.7 MB (10661663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9de9e24906691d18e1f4fd581fee10cb37cb72a3a9284afb39285b1d043bbec`  
		Last Modified: Thu, 07 Jan 2021 18:42:15 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f8d33609df1b332cbc6c1c6157f8d28af146440874a2dfe4e053c0b50e01553`  
		Last Modified: Thu, 07 Jan 2021 18:42:24 GMT  
		Size: 13.1 MB (13133859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf226bc5525c37f9c7485cf27a019bed638523cba8422e0af3b237853473bfd4`  
		Last Modified: Thu, 07 Jan 2021 18:42:14 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1e984c3d711e4168842b3c9abf0d9fc18e746bc6d86f44fd3f30e4a9ef9f14`  
		Last Modified: Thu, 07 Jan 2021 18:42:15 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1535d2313631d2aa95465d3912c5c50d5cda79878a7dddaefd5c923557ad70b2`  
		Last Modified: Thu, 07 Jan 2021 18:42:15 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751bf4764fe0ea02e0503870c3ba61c0088e6a4289902b07d94a632426c8530c`  
		Last Modified: Thu, 07 Jan 2021 22:03:26 GMT  
		Size: 16.5 MB (16527885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1941cbd0388d7b2ee601e71addfc812d836d05d0f5d64f03f1dbf973f00a4c9`  
		Last Modified: Thu, 07 Jan 2021 23:57:26 GMT  
		Size: 7.7 MB (7740373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430e3b45e1f30398abf933c399c338c922613277f9a5cd4453f18c3f3eb2ecec`  
		Last Modified: Thu, 07 Jan 2021 23:57:19 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760b6d18fb7696754f194cf134b234413f6bc146265c7d2aaccf0500dd01be04`  
		Last Modified: Thu, 07 Jan 2021 23:57:17 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44182d8556c859ecc8ea9276379efac9dec905489ce763e03de240d680fd9fa`  
		Last Modified: Thu, 07 Jan 2021 23:57:17 GMT  
		Size: 19.5 KB (19487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5f26806751cab97e8006f4d913bf92ac3f99772e7bd16006d842213283f7bb`  
		Last Modified: Thu, 07 Jan 2021 23:57:29 GMT  
		Size: 15.3 MB (15267079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dce77d1678a3d6bc9577bea46542213884e484b48dfabd3b5e9911a3f74d9d`  
		Last Modified: Thu, 07 Jan 2021 23:57:17 GMT  
		Size: 4.0 KB (3962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:latest` - linux; ppc64le

```console
$ docker pull wordpress@sha256:6e0d7e273febeb6bdadf42e80b74c9827f63105d0338f35199e2d3f5220b34a5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.0 MB (200013394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4589ca676da61392de84eafa495fc4cf2eb3cece32bc91c1a11e2d36ede013dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 11 Dec 2020 03:34:02 GMT
ADD file:eca1a7737bd5e84ff883c4c284c0cd22492145d9cd7ae3b8e7b490e3d8e5aefb in / 
# Fri, 11 Dec 2020 03:34:11 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 09:35:26 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 09:35:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 09:37:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 09:37:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 09:37:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 09:43:36 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 11 Dec 2020 09:43:38 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 11 Dec 2020 09:44:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 11 Dec 2020 09:44:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 11 Dec 2020 09:44:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 11 Dec 2020 09:45:00 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 11 Dec 2020 09:45:02 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 11 Dec 2020 09:45:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 09:45:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 09:45:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 10:26:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 11 Dec 2020 10:26:40 GMT
ENV PHP_VERSION=7.4.13
# Fri, 11 Dec 2020 10:26:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Fri, 11 Dec 2020 10:26:49 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Fri, 11 Dec 2020 10:27:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 10:27:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:33:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Dec 2020 10:33:22 GMT
COPY multi:dc714d093d9a94baf082b278964398d495faeef837d3357693090c43ebfb6fb4 in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:33:35 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Dec 2020 10:33:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Dec 2020 10:33:43 GMT
STOPSIGNAL SIGWINCH
# Fri, 11 Dec 2020 10:33:44 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:33:49 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 10:33:52 GMT
EXPOSE 80
# Fri, 11 Dec 2020 10:33:56 GMT
CMD ["apache2-foreground"]
# Sat, 12 Dec 2020 00:31:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 00:41:08 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 12 Dec 2020 00:41:16 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 12 Dec 2020 00:41:34 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 12 Dec 2020 00:41:49 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Sat, 12 Dec 2020 00:41:55 GMT
ENV WORDPRESS_VERSION=5.6
# Sat, 12 Dec 2020 00:42:04 GMT
ENV WORDPRESS_SHA1=db8b75bfc9de27490434b365c12fd805ca6784ce
# Sat, 12 Dec 2020 00:42:18 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Sat, 12 Dec 2020 00:42:23 GMT
VOLUME [/var/www/html]
# Sat, 12 Dec 2020 00:42:25 GMT
COPY file:f56966eeac957656aead5cb65d1531bfe029ddac03ee3ffefdafd2f0d4252925 in /usr/local/bin/ 
# Sat, 12 Dec 2020 00:42:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 00:42:38 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c0f0648876332890be87a9f32ec4ad2a939e805be3152ab991a923f7dec2b35d`  
		Last Modified: Fri, 11 Dec 2020 03:41:39 GMT  
		Size: 30.5 MB (30524717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5b99ad441d88921297aa0d8c7e2939c5e9612193590ff93145ebd13672ca87`  
		Last Modified: Fri, 11 Dec 2020 12:43:40 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a1c0581b0c2819f18cd9c840a6d32586aa9de3889e54251a3327b0b77c3cb5`  
		Last Modified: Fri, 11 Dec 2020 12:43:59 GMT  
		Size: 82.3 MB (82259915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5dbb5ac2103376300e56e95cc3ccd22e74917a509747b1dd2049869642692e`  
		Last Modified: Fri, 11 Dec 2020 12:43:39 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca1cc816ea84b3a6ebd801a1e953d4afae51890cc4615b4689a104267b7d7de`  
		Last Modified: Fri, 11 Dec 2020 12:44:56 GMT  
		Size: 19.8 MB (19817738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492dff1cd8cb5ef532e553a18fbb10193b386b2a3fd13799a01c79bf8fecf327`  
		Last Modified: Fri, 11 Dec 2020 12:44:51 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659212e8c9d5e16eb1fdfeeb59b411bb6589a67dc62c2fb00f0d03a261fa3175`  
		Last Modified: Fri, 11 Dec 2020 12:44:50 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c6b5d4e9e40496bd0c1d40d4f1b9dee341b0f3c52fef28d3f01038dcf7a11e`  
		Last Modified: Fri, 11 Dec 2020 12:48:53 GMT  
		Size: 10.7 MB (10656965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7421d9d5dca38b058e905e86132f5b9133e21623698afda0c6bfeb536e2ae45`  
		Last Modified: Fri, 11 Dec 2020 12:48:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02b1b224d31f7f15e7974fd2dddf7c5cf64b013adb4f6057d5e4646478b26dfe`  
		Last Modified: Fri, 11 Dec 2020 12:48:53 GMT  
		Size: 14.9 MB (14864506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97074e63f275db45910b6aa94631937936cfe93c6a5dd21866b61753ade0ccfb`  
		Last Modified: Fri, 11 Dec 2020 12:48:49 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90a241fc5d4c79b9be86ce26ad46ad97603301d0a051502f1e926c65236fdc3`  
		Last Modified: Fri, 11 Dec 2020 12:48:48 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5eaff212d5f055f2710510929eca23918bdc85e473ac73fc459a47d594e7ee`  
		Last Modified: Fri, 11 Dec 2020 12:48:49 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636872622a2d792f4450505211c5ab4a3cb1f6be55e01169021775ae20fe6b9d`  
		Last Modified: Sat, 12 Dec 2020 01:10:59 GMT  
		Size: 17.5 MB (17475666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6065fe49a7a73f23b9581227cd41c8a2ada64328a083f960767591140336b08`  
		Last Modified: Sat, 12 Dec 2020 01:10:57 GMT  
		Size: 9.1 MB (9117115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88281687595334e8f7a8d9dcdab94b76b53bd30bdf89056b267ad38f3f796880`  
		Last Modified: Sat, 12 Dec 2020 01:10:52 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274279b9fd813c1cad34d5e287c767289e41e24eff115d49a3cc65382ba2bf98`  
		Last Modified: Sat, 12 Dec 2020 01:10:52 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e149da962dad83bd6d07e3878c26071fad32fec2bdd9a8ee820abbedca283f`  
		Last Modified: Sat, 12 Dec 2020 01:10:52 GMT  
		Size: 19.5 KB (19481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaf62cc23133bb2bfda45a028a5b9cd0ceaa98b0f3b98fa900f19363d3e98ff`  
		Last Modified: Sat, 12 Dec 2020 01:10:56 GMT  
		Size: 15.3 MB (15266955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f249c4a751edd130e39b646a673e962b93ca575de951c64d6ea76a513746d5`  
		Last Modified: Sat, 12 Dec 2020 01:10:52 GMT  
		Size: 4.2 KB (4156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:latest` - linux; s390x

```console
$ docker pull wordpress@sha256:fc7c64aeefc909fe5fc39d65f9f25a4e8cb06379e48702fe1090e955299dde6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172402068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cf454fa08bf94180f03bd3b83c147f03cad7919c20933ac4c56190726f9f4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 11:11:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 11 Dec 2020 11:11:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 11 Dec 2020 11:12:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 11:12:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 11:12:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 11:16:43 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 11 Dec 2020 11:16:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 11 Dec 2020 11:17:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 11 Dec 2020 11:17:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 11 Dec 2020 11:17:05 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 11 Dec 2020 11:17:05 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 11 Dec 2020 11:17:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 11 Dec 2020 11:17:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 11:17:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 11:17:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 11:47:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:47:59 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:48:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:48:00 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:48:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 07 Jan 2021 17:48:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:49:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 17:49:52 GMT
COPY multi:dc714d093d9a94baf082b278964398d495faeef837d3357693090c43ebfb6fb4 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:49:53 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 17:49:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 17:49:53 GMT
STOPSIGNAL SIGWINCH
# Thu, 07 Jan 2021 17:49:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:49:53 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 17:49:54 GMT
EXPOSE 80
# Thu, 07 Jan 2021 17:49:54 GMT
CMD ["apache2-foreground"]
# Thu, 07 Jan 2021 21:35:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 00:03:33 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 08 Jan 2021 00:03:35 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 08 Jan 2021 00:03:36 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 08 Jan 2021 00:03:37 GMT
RUN set -eux; 	a2enmod rewrite expires; 		a2enmod remoteip; 	{ 		echo 'RemoteIPHeader X-Forwarded-For'; 		echo 'RemoteIPTrustedProxy 10.0.0.0/8'; 		echo 'RemoteIPTrustedProxy 172.16.0.0/12'; 		echo 'RemoteIPTrustedProxy 192.168.0.0/16'; 		echo 'RemoteIPTrustedProxy 169.254.0.0/16'; 		echo 'RemoteIPTrustedProxy 127.0.0.0/8'; 	} > /etc/apache2/conf-available/remoteip.conf; 	a2enconf remoteip; 	find /etc/apache2 -type f -name '*.conf' -exec sed -ri 's/([[:space:]]*LogFormat[[:space:]]+"[^"]*)%h([^"]*")/\1%a\2/g' '{}' +
# Fri, 08 Jan 2021 00:03:40 GMT
RUN set -eux; 	version='5.6'; 	sha1='db8b75bfc9de27490434b365c12fd805ca6784ce'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 08 Jan 2021 00:03:42 GMT
VOLUME [/var/www/html]
# Fri, 08 Jan 2021 00:03:42 GMT
COPY file:21c61c8c5411c6f288a3a044c8f9622540460def171cd20ff6e83aa721350821 in /usr/local/bin/ 
# Fri, 08 Jan 2021 00:03:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 Jan 2021 00:03:42 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e848b987a55bcc9612a0ff983cfffc62ac173eb600e57e1f26d2f62d666fdf`  
		Last Modified: Fri, 11 Dec 2020 13:46:08 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aeb6ec9142dee6d014f57c94fb0a215e2d28aa691b8568428e5e462d17ebd92`  
		Last Modified: Fri, 11 Dec 2020 13:46:19 GMT  
		Size: 64.7 MB (64707189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd418c632e5e527db12983ceffec6fb69c3ae70b420bb36ce3f0bc2f72b76bee`  
		Last Modified: Fri, 11 Dec 2020 13:46:08 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c27fa8d6c033bb6eb8edfe95328683591c0a4f6da22496bef5bcc6820050f55`  
		Last Modified: Fri, 11 Dec 2020 13:46:55 GMT  
		Size: 18.5 MB (18524998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d2f7c3fe697fb3c5d37183a5ba4ec1ec85713bc8312d43e83ce67082f0bc04`  
		Last Modified: Fri, 11 Dec 2020 13:46:51 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c28aa1ab7bf0ca80b41f2d404a96e514e6595bd1646ac7104bd8aba3b3cccc`  
		Last Modified: Fri, 11 Dec 2020 13:46:52 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c342efa75ad5be74cdb95f46802267856b3a4471ae021a5da19875345772e1af`  
		Last Modified: Thu, 07 Jan 2021 18:50:06 GMT  
		Size: 10.7 MB (10662886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bedf473093386e0511b8fce724fca41f6d0e6f8f72b1c76cce9d1edf7c7f74`  
		Last Modified: Thu, 07 Jan 2021 18:50:04 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff1d68c43c5ae02d53c082be52d3b6861eabe12380666700443b42f83e6cd76`  
		Last Modified: Thu, 07 Jan 2021 18:50:05 GMT  
		Size: 13.0 MB (13032635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c84a08605e3764c6e6cdd1b4327ac93ef4b6f4324879e20085ef868ddf249f8d`  
		Last Modified: Thu, 07 Jan 2021 18:50:03 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef6e005b3b02b42afde8c181b36e28873491d1e1464a1e6f8a618bcfa76a766`  
		Last Modified: Thu, 07 Jan 2021 18:50:03 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7847797b3e3ed5210ada3de2191ce288662772c770e092088a9f1c70d1426085`  
		Last Modified: Thu, 07 Jan 2021 18:50:04 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a428bcb60f08358ae399b275b442edd30c15fad3ad42f53ff3a50d68201733b9`  
		Last Modified: Thu, 07 Jan 2021 21:42:19 GMT  
		Size: 16.6 MB (16618466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe64da1da9dc3c665371bfe4a9e24f4fc63ca4949e4da7c94fc2e324300f2c5`  
		Last Modified: Fri, 08 Jan 2021 00:12:07 GMT  
		Size: 7.8 MB (7845222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070eb442e6a03a5fc53af489201eef92fc9b9fcec48dc33484c53a46733d08db`  
		Last Modified: Fri, 08 Jan 2021 00:12:06 GMT  
		Size: 376.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebf384c33841a2a6c6c8dacb4aa5427475dfcbb8b1a386df4cd9e035e9e1994`  
		Last Modified: Fri, 08 Jan 2021 00:12:05 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6c062feff2ab11239054331a3b7d1f627b53aa6c315373ac922f458e4796fa`  
		Last Modified: Fri, 08 Jan 2021 00:12:05 GMT  
		Size: 19.5 KB (19472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67db48a3846d1e1ead2abeaff22bda05743a6619c5e5d5108d91ae284502c6f`  
		Last Modified: Fri, 08 Jan 2021 00:12:07 GMT  
		Size: 15.3 MB (15267115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389a4a8e3a417f30c6d10dfdab2c3d5d49fb6682b7373aa3ea07aded689241cb`  
		Last Modified: Fri, 08 Jan 2021 00:12:04 GMT  
		Size: 4.0 KB (3963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
