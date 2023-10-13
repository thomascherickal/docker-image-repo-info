## `wordpress:php8.1-fpm`

```console
$ docker pull wordpress@sha256:daaab0f6733e3ef60dd5b3b6e74b98e734112a5e20908a394e60bef6afef986f
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

### `wordpress:php8.1-fpm` - linux; amd64

```console
$ docker pull wordpress@sha256:eb953c90d793f6cb372e6cd807539f3876eb2011b25514e9f6d86caf2029b323
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.7 MB (252678837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff32de0daecedaaa09d4815ac1297b979357b3669368abed24862bfdc37caf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:50 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Wed, 11 Oct 2023 18:34:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:35:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 03:35:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 03:36:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:36:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 03:36:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 03:36:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:36:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 03:36:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 04:33:44 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 12 Oct 2023 04:33:44 GMT
ENV PHP_VERSION=8.1.24
# Thu, 12 Oct 2023 04:33:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Thu, 12 Oct 2023 04:33:45 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Thu, 12 Oct 2023 04:34:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 04:34:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 04:45:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 04:45:02 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 12 Oct 2023 04:45:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 04:45:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 04:45:02 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 04:45:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 12 Oct 2023 04:45:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 12 Oct 2023 04:45:03 GMT
EXPOSE 9000
# Thu, 12 Oct 2023 04:45:03 GMT
CMD ["php-fpm"]
# Thu, 12 Oct 2023 19:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 19:17:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 19:17:28 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 19:17:28 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 19:17:32 GMT
RUN set -eux; 	version='6.3.1'; 	sha1='052777aef40e7f627c63c8a26eefe37b843a44df'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 12 Oct 2023 19:17:32 GMT
VOLUME [/var/www/html]
# Thu, 12 Oct 2023 19:17:32 GMT
COPY --chown=www-data:www-datafile:d38fd3c0db552e13465e83c5d7bbd85c7c3d036bf1285495988cc4ab2ffaf7f5 in /usr/src/wordpress/ 
# Thu, 12 Oct 2023 19:17:32 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 12 Oct 2023 19:17:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 19:17:33 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ad076dff2ee9b3f3f22002a0376585f329a1520f17968ed711ec81aac8c56e`  
		Last Modified: Thu, 12 Oct 2023 05:31:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d17b5cade1b79810ab26afa4e1c16926954b1bdbe90c6bb584a6d56d0e0da26`  
		Last Modified: Thu, 12 Oct 2023 05:31:34 GMT  
		Size: 104.4 MB (104352887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d71c28a645649b1de350bae417729f630041edea705feac3f1b231a45e7def23`  
		Last Modified: Thu, 12 Oct 2023 05:31:19 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a209902cf37c4f214fd0ee889fc3a8bd7896fa7cc66bc5ba5c9a748f4e761e`  
		Last Modified: Thu, 12 Oct 2023 05:38:00 GMT  
		Size: 12.1 MB (12108896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d352b19c53d03b7b5b89cd7c9a2bfe7d2b783dc5b387b68de24c9e263f98d714`  
		Last Modified: Thu, 12 Oct 2023 05:37:58 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4c2b2c7de1922216a7893a6b098c0850d6495fb797a834b55bd2c211491057`  
		Last Modified: Thu, 12 Oct 2023 05:38:46 GMT  
		Size: 27.5 MB (27527796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ca885ef9f374d174a3cdc1ef9c39399b428f95b1ffb6d59acb2b10a443d615`  
		Last Modified: Thu, 12 Oct 2023 05:38:41 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815861d69716108ed21fdcf6beb63cc7ac1a9b2d6fd02e240c698ba87b52031`  
		Last Modified: Thu, 12 Oct 2023 05:38:41 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e6a63ff199855db7231907d27a8e27eb65159d3b6722693acd0f8dfd81031c`  
		Last Modified: Thu, 12 Oct 2023 05:38:41 GMT  
		Size: 8.9 KB (8876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c16de38a09ade54875b43d3e4d92386c26cdc9aa200ce55f51a0f29b0d40d21`  
		Last Modified: Thu, 12 Oct 2023 19:25:38 GMT  
		Size: 26.4 MB (26381274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f333f0d817c909fdddcddcaae10bfea8f00f1e5b051fba950eef78f049c3a3`  
		Last Modified: Thu, 12 Oct 2023 19:25:38 GMT  
		Size: 29.9 MB (29867181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf6f639681f2a1393d6f5b85709c49d1ee0c050af6778ea1780ac7a0e50749d`  
		Last Modified: Thu, 12 Oct 2023 19:25:31 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce4ac3692742aacad9436f06b310c3a26e6392ad14fbe597fc4f8773fc09364`  
		Last Modified: Thu, 12 Oct 2023 19:25:31 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc801923e714f063e79e1eeeab12e9a53459e1528435403b94be6701025f46d`  
		Last Modified: Thu, 12 Oct 2023 19:25:35 GMT  
		Size: 23.3 MB (23273532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8be6ca3711ad064363d199662ede2e9345402c2c9e9bffc024aa2a87cb2326`  
		Last Modified: Thu, 12 Oct 2023 19:25:31 GMT  
		Size: 2.4 KB (2350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bdfa2c3e020b7d926ac7952216d3c6c79f55070065369870f36ce0514bdaa52`  
		Last Modified: Thu, 12 Oct 2023 19:25:31 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:3fc0a875dc06a7a6a86efb4f44ea5d35f2e5ed32c395700d55d2b63b3bc3a345
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.8 MB (222838785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1c57a8c489b05a7722dd872ed744a8b5dc7cdadcede39af1e79d019f6ba39a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:43 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Wed, 11 Oct 2023 17:37:43 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:28:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Oct 2023 22:28:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Oct 2023 22:29:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:29:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Oct 2023 22:29:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 11 Oct 2023 22:29:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:29:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:29:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Oct 2023 23:17:53 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Oct 2023 23:17:53 GMT
ENV PHP_VERSION=8.1.24
# Wed, 11 Oct 2023 23:17:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Wed, 11 Oct 2023 23:17:54 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Wed, 11 Oct 2023 23:18:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Oct 2023 23:18:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Oct 2023 23:28:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Oct 2023 23:28:07 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Oct 2023 23:28:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Oct 2023 23:28:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Oct 2023 23:28:10 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 23:28:11 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Oct 2023 23:28:11 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Oct 2023 23:28:11 GMT
EXPOSE 9000
# Wed, 11 Oct 2023 23:28:12 GMT
CMD ["php-fpm"]
# Thu, 12 Oct 2023 09:27:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 09:29:09 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 09:29:10 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 09:29:10 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 09:29:14 GMT
RUN set -eux; 	version='6.3.1'; 	sha1='052777aef40e7f627c63c8a26eefe37b843a44df'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 12 Oct 2023 09:29:15 GMT
VOLUME [/var/www/html]
# Thu, 12 Oct 2023 09:29:15 GMT
COPY --chown=www-data:www-datafile:d38fd3c0db552e13465e83c5d7bbd85c7c3d036bf1285495988cc4ab2ffaf7f5 in /usr/src/wordpress/ 
# Thu, 12 Oct 2023 09:29:15 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 12 Oct 2023 09:29:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 09:29:15 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fa8e4917e1fc4cdb2f4419c1699100cf74e6c3305d6ad5cd40293a3fa5359e`  
		Last Modified: Thu, 12 Oct 2023 00:15:01 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9847054fe5d49949a4aaa7ef1f8aa389ff4037632f0d72987225d45fe7f89f40`  
		Last Modified: Thu, 12 Oct 2023 00:15:22 GMT  
		Size: 82.0 MB (82047969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e50907e19eead2a289407a27937238c3dafc48371525244545ba41940e5fd53`  
		Last Modified: Thu, 12 Oct 2023 00:15:01 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61400fd1d96d3296a327f58f8e289d100e31df0018142fcb66ecaec71d1a3d9`  
		Last Modified: Thu, 12 Oct 2023 00:21:48 GMT  
		Size: 12.1 MB (12107139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d0b507d7c7dc163c403387c9237418bd0e7244e9fec6c88817b210594b1dcc`  
		Last Modified: Thu, 12 Oct 2023 00:21:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe58df0b4f2d9102b8b81d9dd2c16bc714450edabfeb17b574b2f32bfadc069b`  
		Last Modified: Thu, 12 Oct 2023 00:22:42 GMT  
		Size: 26.0 MB (26006599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42eda00730796533f747001aba9be32ceff360997d0f507db7c8401cd7f03f8a`  
		Last Modified: Thu, 12 Oct 2023 00:22:36 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b569269117b5280e4c07c9e9ba04febc065a30df6dc3bd12dc9b1c4a48a20986`  
		Last Modified: Thu, 12 Oct 2023 00:22:36 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b49ad22626c76c87ab31f09f442c668d9bab373dbad0a6fe394db444f1058`  
		Last Modified: Thu, 12 Oct 2023 00:22:36 GMT  
		Size: 8.9 KB (8882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af7ba7a21fcbb8445c8aa1b7b3363e68171fff74e44970b69f8f3a5a48ba86e`  
		Last Modified: Thu, 12 Oct 2023 09:37:04 GMT  
		Size: 25.8 MB (25825363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f41c9c60100222965075f221d3c39ebe421bac68f2a5acfa1ad87bf218dceeda`  
		Last Modified: Thu, 12 Oct 2023 09:37:04 GMT  
		Size: 26.6 MB (26638625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b688c3b370a65cdb6f8df255f12917f265f2cc74cf5d94bc2ecfa52a4744bd`  
		Last Modified: Thu, 12 Oct 2023 09:36:58 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884de74c2f4278d3632f33032488f44c80b28607f3e890773b6aee21dd0fc886`  
		Last Modified: Thu, 12 Oct 2023 09:36:58 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdda2d98c8acb50c1733be147d8f7fd23b5b35b7929bca1f5ad50d58b8bf6f81`  
		Last Modified: Thu, 12 Oct 2023 09:37:02 GMT  
		Size: 23.3 MB (23273529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf094377d33dc6750b04704b5a66ca306fe935dd9005ef579d174b81e45e2d10`  
		Last Modified: Thu, 12 Oct 2023 09:36:58 GMT  
		Size: 2.3 KB (2348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c33570b4f0fe8cb79c041c49a23f33d1fac2df401fd1a88653355286fb9e5f`  
		Last Modified: Thu, 12 Oct 2023 09:36:58 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:d5f71d44d5f9dfb246cca4423207c03c4686f82697aa4fc8056ba23656691bc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.8 MB (211775295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d87870177b818323fe474465a87e6c23f91cc1812e38373e38d8831cd133c8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:11 GMT
ADD file:da08fed31a161a2210fd920a1b5e43aa3f4199985cdeaa0d5d24c0a0f19044aa in / 
# Wed, 11 Oct 2023 17:42:11 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:16:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Oct 2023 19:16:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Oct 2023 19:17:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:17:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Oct 2023 19:17:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 11 Oct 2023 19:17:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 19:17:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 19:17:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Oct 2023 20:12:59 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Oct 2023 20:12:59 GMT
ENV PHP_VERSION=8.1.24
# Wed, 11 Oct 2023 20:12:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Wed, 11 Oct 2023 20:13:00 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Wed, 11 Oct 2023 20:13:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Oct 2023 20:13:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:30:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Oct 2023 20:30:09 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Oct 2023 20:30:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Oct 2023 20:30:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Oct 2023 20:30:09 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 20:30:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Oct 2023 20:30:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Oct 2023 20:30:10 GMT
EXPOSE 9000
# Wed, 11 Oct 2023 20:30:10 GMT
CMD ["php-fpm"]
# Thu, 12 Oct 2023 06:48:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 06:50:07 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 06:50:08 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 06:50:08 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 06:50:12 GMT
RUN set -eux; 	version='6.3.1'; 	sha1='052777aef40e7f627c63c8a26eefe37b843a44df'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 12 Oct 2023 06:50:12 GMT
VOLUME [/var/www/html]
# Thu, 12 Oct 2023 06:50:12 GMT
COPY --chown=www-data:www-datafile:d38fd3c0db552e13465e83c5d7bbd85c7c3d036bf1285495988cc4ab2ffaf7f5 in /usr/src/wordpress/ 
# Thu, 12 Oct 2023 06:50:13 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 12 Oct 2023 06:50:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 06:50:13 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2f11c34abc7b59f09b58bb6e2cf54f260f4b4142ecf8023a114e281ea4b532d1`  
		Last Modified: Wed, 11 Oct 2023 17:46:22 GMT  
		Size: 24.7 MB (24748925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60addccf9d45f8daddb0238754bdf613af58ed3f2c5188649b3584d91c9e9407`  
		Last Modified: Wed, 11 Oct 2023 21:24:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c247348c790b796698137345a99a4f5afebbbc24ce9dbd9bedc07f017f41c5`  
		Last Modified: Wed, 11 Oct 2023 21:24:53 GMT  
		Size: 76.2 MB (76225741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7baba4d60838c07f3fc636e38e6c4a4066ff85ee42d4af6676c0030b30e7234`  
		Last Modified: Wed, 11 Oct 2023 21:24:41 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e92f55e874bee822e7d912a9caec430f1f2f90e235b78d782938f51883ae35`  
		Last Modified: Wed, 11 Oct 2023 21:31:49 GMT  
		Size: 12.1 MB (12107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b22f23ffb2165653d0a8f9a9b04eb03ce936e2d6c6ed00cb8a5f44855c080f2`  
		Last Modified: Wed, 11 Oct 2023 21:31:48 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee484a0eee7262bdc0bb97499eb2cf3194231f738e40cb72c32bb828035a5c42`  
		Last Modified: Wed, 11 Oct 2023 21:32:49 GMT  
		Size: 25.1 MB (25149361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b300b16a3999ec7bc00d04108d4d47235d148cf045be42fe7199c630f1b81c1f`  
		Last Modified: Wed, 11 Oct 2023 21:32:45 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca69a930a5a76e258d21b394d28ec45dcd85e63897ec797553e8d698d8bab9b`  
		Last Modified: Wed, 11 Oct 2023 21:32:45 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c35ab087ff540d26cba8fbecd17f46b556c51bd0a1551a0bf183c3ee4546f55`  
		Last Modified: Wed, 11 Oct 2023 21:32:45 GMT  
		Size: 8.9 KB (8883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f06970f9058a51f013e322499a31207053f5fe06b1a58f6641292e4e71ff732`  
		Last Modified: Thu, 12 Oct 2023 06:58:53 GMT  
		Size: 25.2 MB (25171969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e299ab06ce4b10f8492a40c8451081f2ac4a4c6db86ddf10bc97f72c408864e0`  
		Last Modified: Thu, 12 Oct 2023 06:58:53 GMT  
		Size: 25.1 MB (25081206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e00a6f9dec76756191ede8f6faa1f9b2c2dbd32f0ae318a41d759a7af5d16da`  
		Last Modified: Thu, 12 Oct 2023 06:58:44 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ce6be337f0be3cecdd3c71ff8e5cb585d2415caafc24ddbe05e6a7028be2ce`  
		Last Modified: Thu, 12 Oct 2023 06:58:44 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f491e62fc745ec28044b07364cac9544fc3a74d853157528ce45b52d2714dd3`  
		Last Modified: Thu, 12 Oct 2023 06:58:50 GMT  
		Size: 23.3 MB (23273548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0313ae7b55a1ffaed99080689c28ff5d83254701fc75936d52a525d2b336f6e`  
		Last Modified: Thu, 12 Oct 2023 06:58:44 GMT  
		Size: 2.3 KB (2347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d0594534f8d6d590c924e502bc2a76fabd5cf05973b05d0e97960f92e02001`  
		Last Modified: Thu, 12 Oct 2023 06:58:44 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:6e0bce958685a7c46bd9c15b33fb693d13899d045948c1aae45aa4527d38d2d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.0 MB (243990156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54797586766d9e9b8dedf629c02340a641239ad93029adcd4c15f0d997d577c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:51 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Wed, 11 Oct 2023 18:24:51 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 08:13:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 08:13:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 08:13:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 08:13:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 08:13:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 08:13:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 08:13:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 08:13:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 09:10:14 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 12 Oct 2023 09:10:14 GMT
ENV PHP_VERSION=8.1.24
# Thu, 12 Oct 2023 09:10:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Thu, 12 Oct 2023 09:10:14 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Thu, 12 Oct 2023 09:10:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 09:10:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 09:21:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 09:21:11 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 12 Oct 2023 09:21:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 09:21:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 09:21:12 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 09:21:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 12 Oct 2023 09:21:13 GMT
STOPSIGNAL SIGQUIT
# Thu, 12 Oct 2023 09:21:13 GMT
EXPOSE 9000
# Thu, 12 Oct 2023 09:21:13 GMT
CMD ["php-fpm"]
# Thu, 12 Oct 2023 19:16:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 19:17:50 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 19:17:51 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 19:17:51 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 19:17:54 GMT
RUN set -eux; 	version='6.3.1'; 	sha1='052777aef40e7f627c63c8a26eefe37b843a44df'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 12 Oct 2023 19:17:54 GMT
VOLUME [/var/www/html]
# Thu, 12 Oct 2023 19:17:55 GMT
COPY --chown=www-data:www-datafile:d38fd3c0db552e13465e83c5d7bbd85c7c3d036bf1285495988cc4ab2ffaf7f5 in /usr/src/wordpress/ 
# Thu, 12 Oct 2023 19:17:55 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 12 Oct 2023 19:17:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 19:17:55 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6db690faaae693fface34a50bfe91ec722f16596447dee7df8fb412cac50de`  
		Last Modified: Thu, 12 Oct 2023 09:58:06 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52439f351543dbca787c3477a8a818967bcedc1c39976df5f1abf6ccf6b1270`  
		Last Modified: Thu, 12 Oct 2023 09:58:16 GMT  
		Size: 98.1 MB (98136069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b2675dd3270d646cc9609f7620fb3ee1b137cf246173d31b605f21c9162fb00`  
		Last Modified: Thu, 12 Oct 2023 09:58:05 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e96021cab685ff53d7eae57ebb615c0609b73d405a98bf255cbb28886020fe`  
		Last Modified: Thu, 12 Oct 2023 10:04:24 GMT  
		Size: 12.1 MB (12108667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c800d9b766b849ca7daa6b5774756547a89a5a1a1ae4a86d87e50b4047efe1c`  
		Last Modified: Thu, 12 Oct 2023 10:04:22 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076db76845c8c39337919654f3cbdbb3e0361982219a0c554f585ec743fef4b5`  
		Last Modified: Thu, 12 Oct 2023 10:05:08 GMT  
		Size: 27.5 MB (27475547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b363fca4e4d1e2c55658875e9454ec970714e85c72ed67d85452fd7e11cb24ae`  
		Last Modified: Thu, 12 Oct 2023 10:05:05 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27aecd533999d8cf2090018a641844fe34563b06eaae6fe39cd4bdb8d0f73fb2`  
		Last Modified: Thu, 12 Oct 2023 10:05:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb1129d5543a2b14b49c744f3404a2c1551fc5ae54dc6b97abf5c32a8f0a11d`  
		Last Modified: Thu, 12 Oct 2023 10:05:05 GMT  
		Size: 8.9 KB (8885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3c68657cb0baf435dc47054e1d14e53b40e6556c7a860edc91813ac7fd374e`  
		Last Modified: Thu, 12 Oct 2023 19:25:33 GMT  
		Size: 26.3 MB (26293389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e71e741da9d1b1562a4867306e389fbf161c514e31e4031cfae1b3cea54082`  
		Last Modified: Thu, 12 Oct 2023 19:25:33 GMT  
		Size: 27.5 MB (27506245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6f0d0aa6de9c27962073595adf3b88b63cb9d5af1720ae3de7edaf4e86ad29`  
		Last Modified: Thu, 12 Oct 2023 19:25:27 GMT  
		Size: 365.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f79ed1e3552bf05712edaec98a1d7671b6b5f223deea776517c406a6e536910`  
		Last Modified: Thu, 12 Oct 2023 19:25:27 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a2f2b7d01214346c0da57ad99a6b4d682c187947b331a4670a6cd78b68e60b`  
		Last Modified: Thu, 12 Oct 2023 19:25:30 GMT  
		Size: 23.3 MB (23273532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1032765b60aaed7c20dc268f0363d8a746e5478275d5f9a9495556d9a45493fc`  
		Last Modified: Thu, 12 Oct 2023 19:25:27 GMT  
		Size: 2.3 KB (2347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1030079a3597e836fc9fbfc081192759c2944c953973ae76bb6b0c069c100910`  
		Last Modified: Thu, 12 Oct 2023 19:25:27 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm` - linux; 386

```console
$ docker pull wordpress@sha256:afad421e7a01205786d32108bfadcfff52d9a584f55f3e692c5553e34474fcc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.2 MB (251203295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46d8400b394c41f0ada98df1a3f940c3dd1f418adedccfd5679cb85bc375996`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:42 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Wed, 11 Oct 2023 17:40:42 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 05:20:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 05:20:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 05:21:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 05:21:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 05:21:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 05:21:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 05:21:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 05:21:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 06:55:49 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 12 Oct 2023 06:55:49 GMT
ENV PHP_VERSION=8.1.24
# Thu, 12 Oct 2023 06:55:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Thu, 12 Oct 2023 06:55:49 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Thu, 12 Oct 2023 06:56:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 06:56:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 07:14:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 07:14:28 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 12 Oct 2023 07:14:29 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 07:14:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 07:14:29 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 07:14:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 12 Oct 2023 07:14:30 GMT
STOPSIGNAL SIGQUIT
# Thu, 12 Oct 2023 07:14:30 GMT
EXPOSE 9000
# Thu, 12 Oct 2023 07:14:30 GMT
CMD ["php-fpm"]
# Thu, 12 Oct 2023 19:02:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 19:03:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 12 Oct 2023 19:03:39 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 Oct 2023 19:03:40 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 12 Oct 2023 19:03:44 GMT
RUN set -eux; 	version='6.3.1'; 	sha1='052777aef40e7f627c63c8a26eefe37b843a44df'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 12 Oct 2023 19:03:44 GMT
VOLUME [/var/www/html]
# Thu, 12 Oct 2023 19:03:44 GMT
COPY --chown=www-data:www-datafile:d38fd3c0db552e13465e83c5d7bbd85c7c3d036bf1285495988cc4ab2ffaf7f5 in /usr/src/wordpress/ 
# Thu, 12 Oct 2023 19:03:45 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 12 Oct 2023 19:03:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 Oct 2023 19:03:45 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a685497e319a2b6b2b724f94202c87562da480b7886e87b5bf18e1482d4c5d2`  
		Last Modified: Thu, 12 Oct 2023 08:25:29 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dea9e9f22b3e1d15c62435915faf772b929100a57d639bd083ef64a01437dd6`  
		Last Modified: Thu, 12 Oct 2023 08:25:52 GMT  
		Size: 101.5 MB (101531380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b416265171fa34df6124c5f53f38a6409255b6a3f8381d94a020e02eade87a9d`  
		Last Modified: Thu, 12 Oct 2023 08:25:29 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3da9519b7098ebd8df028789fce7f1602e56990b701ccc1b3ad5af49290ccd8`  
		Last Modified: Thu, 12 Oct 2023 08:32:50 GMT  
		Size: 12.1 MB (12108189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c3eb11b1873e25494b0bfa54b907bf482a26a43d9e2beda42aae440eadd847`  
		Last Modified: Thu, 12 Oct 2023 08:32:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da97911b00ac7c27410eb6879e667500da370bd0cd8e36f3addad29df637a60c`  
		Last Modified: Thu, 12 Oct 2023 08:33:41 GMT  
		Size: 28.0 MB (28038517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ac03e70999cf74ef3d7aada8c567ab352abc6e60ed9532594270280ecb8099`  
		Last Modified: Thu, 12 Oct 2023 08:33:35 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a686ee650abf5ce27d02606e429c5c19d0758d403352f78a8e0961fb2c19aa41`  
		Last Modified: Thu, 12 Oct 2023 08:33:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac65bcf661489ef083dcd1545018a71715c22e7770a307b5bb5d71c0c95b1a`  
		Last Modified: Thu, 12 Oct 2023 08:33:35 GMT  
		Size: 8.9 KB (8881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f20e940f2ac6d50ea2877d583adec6c18f5db407cb76455721972e436c2943`  
		Last Modified: Thu, 12 Oct 2023 19:13:03 GMT  
		Size: 26.8 MB (26837258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ebc9b6b370bb5e54c9707ca87f86be6207051694b5f017bcc0dccb03babf73`  
		Last Modified: Thu, 12 Oct 2023 19:13:05 GMT  
		Size: 29.2 MB (29232901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ea897ec339d5e9fb90630c9efe4807a51addb7b7cfe775a2e925203c828823`  
		Last Modified: Thu, 12 Oct 2023 19:12:54 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d52e1998eaf77ace4077801c9bd8dd3390dfeadce35b2a82e50ec80d226d2a3`  
		Last Modified: Thu, 12 Oct 2023 19:12:54 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ec1115938b8c9b86f9cb182771af95eeff6686c1924c2d377f1b3c55a7db6c`  
		Last Modified: Thu, 12 Oct 2023 19:13:00 GMT  
		Size: 23.3 MB (23273528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c024073a981a854b1a5d301e17793226437f6b9052d4e83bf5292a1e6ecd0aa`  
		Last Modified: Thu, 12 Oct 2023 19:12:54 GMT  
		Size: 2.3 KB (2347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee167c6ab8acb58829a90cc5c51fd65aeabee2ee34728eb70fe7b0938cfc217c`  
		Last Modified: Thu, 12 Oct 2023 19:12:54 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm` - linux; mips64le

```console
$ docker pull wordpress@sha256:dc53b87b6bd685c24a9ae1bcb32a53587166741bacc2795da6c7b40a7477fa61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.6 MB (224570200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4df4ddcc90b28b62d0dbe94b781e23ff30de623b332e9692a3612f6138707fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 20 Sep 2023 03:10:01 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Wed, 20 Sep 2023 03:10:05 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:07:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 10:07:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 10:09:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:09:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 10:09:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 10:09:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 10:09:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 10:09:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 16:19:15 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 30 Sep 2023 05:54:13 GMT
ENV PHP_VERSION=8.1.24
# Sat, 30 Sep 2023 05:54:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 30 Sep 2023 05:54:20 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 30 Sep 2023 05:55:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 30 Sep 2023 05:55:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 30 Sep 2023 06:41:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 30 Sep 2023 06:41:30 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 30 Sep 2023 06:41:36 GMT
RUN docker-php-ext-enable sodium
# Sat, 30 Sep 2023 06:41:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 30 Sep 2023 06:41:43 GMT
WORKDIR /var/www/html
# Sat, 30 Sep 2023 06:41:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 30 Sep 2023 06:41:52 GMT
STOPSIGNAL SIGQUIT
# Sat, 30 Sep 2023 06:41:55 GMT
EXPOSE 9000
# Sat, 30 Sep 2023 06:41:59 GMT
CMD ["php-fpm"]
# Sat, 30 Sep 2023 13:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Sep 2023 13:19:19 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Sat, 30 Sep 2023 13:19:27 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 30 Sep 2023 13:19:33 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 30 Sep 2023 13:19:52 GMT
RUN set -eux; 	version='6.3.1'; 	sha1='052777aef40e7f627c63c8a26eefe37b843a44df'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Sat, 30 Sep 2023 13:19:57 GMT
VOLUME [/var/www/html]
# Sat, 30 Sep 2023 13:20:01 GMT
COPY --chown=www-data:www-datafile:d38fd3c0db552e13465e83c5d7bbd85c7c3d036bf1285495988cc4ab2ffaf7f5 in /usr/src/wordpress/ 
# Sat, 30 Sep 2023 13:20:06 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Sat, 30 Sep 2023 13:20:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Sep 2023 13:20:15 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13be0169bbca45d04b6865d960fa18b85165b8512d8b6586743bc395e961aae5`  
		Last Modified: Wed, 20 Sep 2023 21:18:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78fa1c50adc35b8a5d3ed371ce4ecc5fdd6ddd827aac2af4c9f5dcc0295f4f4`  
		Last Modified: Wed, 20 Sep 2023 21:19:51 GMT  
		Size: 80.7 MB (80671000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a2620da2ab8ff2c4c00daed91ea144d334623c7de2d739f7e905cee010fa21`  
		Last Modified: Wed, 20 Sep 2023 21:18:54 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbfc95f25e64860cd1d8d8d3986bd6b9f501d9e13649b930f66f224ee5b8d2f`  
		Last Modified: Sat, 30 Sep 2023 08:05:47 GMT  
		Size: 11.9 MB (11900677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd744e71fb29b892c84b8b3a314f6672384f6108cdde20c6f4e1ab4371e8985`  
		Last Modified: Sat, 30 Sep 2023 08:05:44 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a696e8b3493c223c9f536c8035738eba2b29a475c616447678e16ac7348b07b4`  
		Last Modified: Sat, 30 Sep 2023 08:07:12 GMT  
		Size: 26.4 MB (26414382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c25bcbb527f3dd802cf12f08b746662632d23549f30893f580d4a04a9b9b7eda`  
		Last Modified: Sat, 30 Sep 2023 08:06:56 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:300cb06283683578c9d52a725041644a2ec72109664ec060518798cbc9f6f667`  
		Last Modified: Sat, 30 Sep 2023 08:06:56 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85acac0c63e11bd9bcdeecb7ea52671f6968e8d53fb7027a075fde0604f80ed8`  
		Last Modified: Sat, 30 Sep 2023 08:06:56 GMT  
		Size: 8.9 KB (8889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e058241ae76f7e74c6c8cfbdcbcb35ac9de95febeb49c0c5034f41d22d4e031`  
		Last Modified: Sat, 30 Sep 2023 13:46:29 GMT  
		Size: 26.2 MB (26152279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afc45a5cb1fb3c89b0b213aafa851e33bf2b645cbc2e8cb8777d65fa8622b6d`  
		Last Modified: Sat, 30 Sep 2023 13:46:31 GMT  
		Size: 27.0 MB (27019152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31254b373a978ace8a8a2c6fdd482a172d9d7668619f507aeefff74cc21a11f4`  
		Last Modified: Sat, 30 Sep 2023 13:46:07 GMT  
		Size: 364.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc468ffb5e56d9c6d6e522129e084a00a0167b922d8d824a3046193e476d2e0`  
		Last Modified: Sat, 30 Sep 2023 13:46:07 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaab8f1a72043390c2a7672f8535fa19e979c608cbd6ef398278d2678cffd4a`  
		Last Modified: Sat, 30 Sep 2023 13:46:23 GMT  
		Size: 23.3 MB (23273662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c41c34b24d0877d6b983ee9c4f226bc1d509a091c8fc105eceaa3dfa3e5c45`  
		Last Modified: Sat, 30 Sep 2023 13:46:07 GMT  
		Size: 2.3 KB (2347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dacc8457db12ce7af33b99618b340aa7f69dddc3a4d6b0f78829d666a3c1ae`  
		Last Modified: Sat, 30 Sep 2023 13:46:07 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm` - linux; ppc64le

```console
$ docker pull wordpress@sha256:96589dbe8898ae4ab34307b735e76a44ce985613316a6d3571649af21a71c6c4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.8 MB (257787643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d58a5fbe1748cd7a6fed4f8f8d6ee013c2a5a447bb467db3d6b41d69ebf98d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:19 GMT
ADD file:53c83bdd58e7c4003ae769596cc2f8e6b72c0bbb854dbe7f006a39f273848b1b in / 
# Wed, 11 Oct 2023 17:44:21 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:23:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Oct 2023 22:23:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Oct 2023 22:24:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:24:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Oct 2023 22:24:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 11 Oct 2023 22:24:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:24:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:24:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Oct 2023 23:45:23 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 Oct 2023 23:45:23 GMT
ENV PHP_VERSION=8.1.24
# Wed, 11 Oct 2023 23:45:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Wed, 11 Oct 2023 23:45:24 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Wed, 11 Oct 2023 23:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Oct 2023 23:45:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Oct 2023 23:59:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Oct 2023 23:59:40 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 Oct 2023 23:59:42 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Oct 2023 23:59:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Oct 2023 23:59:43 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 23:59:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 11 Oct 2023 23:59:45 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 Oct 2023 23:59:46 GMT
EXPOSE 9000
# Wed, 11 Oct 2023 23:59:46 GMT
CMD ["php-fpm"]
# Fri, 13 Oct 2023 00:01:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:04:29 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 13 Oct 2023 00:04:32 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 13 Oct 2023 00:04:34 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 13 Oct 2023 00:04:40 GMT
RUN set -eux; 	version='6.3.1'; 	sha1='052777aef40e7f627c63c8a26eefe37b843a44df'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Fri, 13 Oct 2023 00:04:42 GMT
VOLUME [/var/www/html]
# Fri, 13 Oct 2023 00:04:44 GMT
COPY --chown=www-data:www-datafile:d38fd3c0db552e13465e83c5d7bbd85c7c3d036bf1285495988cc4ab2ffaf7f5 in /usr/src/wordpress/ 
# Fri, 13 Oct 2023 00:04:45 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Fri, 13 Oct 2023 00:04:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 00:04:46 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:54813908ce8a5d8a81f2db88ad0366eb5266484c7c402e5e93ef26e764f7a0e2`  
		Last Modified: Wed, 11 Oct 2023 17:49:58 GMT  
		Size: 33.1 MB (33141653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d8a2a1403465e0fb9e91eabac1bc00df3d7d73951dbddf4ff0219372b680a7`  
		Last Modified: Thu, 12 Oct 2023 00:43:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db7b4f878b38fa5b9844ee0de75b17ee2fdb556df06a8dbf408cbf719c1a8e2`  
		Last Modified: Thu, 12 Oct 2023 00:44:04 GMT  
		Size: 103.3 MB (103321394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7530e1e6052f1efc267c9e5b1baa9a7fa2128027e0ec3178d4a6f2c24db07320`  
		Last Modified: Thu, 12 Oct 2023 00:43:37 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5600200a05c64619b8db9288eaa79505d1ab2770d0b134ecb9d59e0dedc059c5`  
		Last Modified: Thu, 12 Oct 2023 00:51:42 GMT  
		Size: 12.1 MB (12108375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4868fd9efd5c8e3f7a81a5d9ed52f3f2acb882e99f6d331edba135fd7734556e`  
		Last Modified: Thu, 12 Oct 2023 00:51:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a26881ba2b8cffdaa1d0247de7afbdeae529d4ded40a9b994d36261862332c`  
		Last Modified: Thu, 12 Oct 2023 00:52:41 GMT  
		Size: 28.5 MB (28543979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0f8d53a49908187ab6048be851b8b84c8f521f54b1dabbc30bf044b7056468`  
		Last Modified: Thu, 12 Oct 2023 00:52:33 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10d165efce7d9aee83ebed5b837aca19257e2453d9e26a5533ff9b320752933`  
		Last Modified: Thu, 12 Oct 2023 00:52:33 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3140df1df9fabda90e70f34dd5b7b7ebb40c4ae288f1b728606d2ebce1d9a7c7`  
		Last Modified: Thu, 12 Oct 2023 00:52:33 GMT  
		Size: 8.9 KB (8884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e45767c8ba2caf0c5cbe233f53cc34e53c842215265a39d9f00adab3d79b468d`  
		Last Modified: Fri, 13 Oct 2023 00:17:37 GMT  
		Size: 27.5 MB (27482459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652afb0cc1e95faf9ee80da6d9ab8f7ce9f6d1de69c9cf5ac6b729397f101f65`  
		Last Modified: Fri, 13 Oct 2023 00:17:38 GMT  
		Size: 29.9 MB (29898844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f419c893578c5964d02c89e103a930928153b99deec0438555ed01d47cb30a8`  
		Last Modified: Fri, 13 Oct 2023 00:17:30 GMT  
		Size: 363.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be591ab1827ca67a58b31c13dba9897838f74cb52810d1eab32bb75eceedb93`  
		Last Modified: Fri, 13 Oct 2023 00:17:31 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369d4964208fbb349d7bac2f04b4b0c1d9053198c2a8c0a82738aec3bc491d6b`  
		Last Modified: Fri, 13 Oct 2023 00:17:34 GMT  
		Size: 23.3 MB (23273528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147b8f0cf08b80f9e083f27e64068fc7fafdd7109705824c14e916b74f47ffe1`  
		Last Modified: Fri, 13 Oct 2023 00:17:30 GMT  
		Size: 2.3 KB (2348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32bb1eae5a7e00791e7459a8913fa6b1324fa68bca29995e2cd4428fbe2beb99`  
		Last Modified: Fri, 13 Oct 2023 00:17:31 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm` - linux; s390x

```console
$ docker pull wordpress@sha256:564f98340281b409d227fdc9c2832807be9da18918a2dfdee9e96b765c627d1c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.9 MB (222853150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401cc7d97799ee0a27aacbdc095fe966460b521662ec5a0635dae086c3f21c4e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:28 GMT
ADD file:b85ed0ed01200dd3626d66cf5205d989fc48e61b3dd3498f777ee72d91e64870 in / 
# Wed, 11 Oct 2023 17:50:30 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 09:47:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 12 Oct 2023 09:47:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 12 Oct 2023 09:48:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 09:48:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 12 Oct 2023 09:48:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 12 Oct 2023 09:48:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 09:48:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 12 Oct 2023 09:48:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 12 Oct 2023 10:34:58 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 12 Oct 2023 10:34:58 GMT
ENV PHP_VERSION=8.1.24
# Thu, 12 Oct 2023 10:34:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Thu, 12 Oct 2023 10:34:59 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Thu, 12 Oct 2023 10:35:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Oct 2023 10:35:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 10:43:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 10:43:15 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 12 Oct 2023 10:43:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 10:43:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 10:43:16 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 10:43:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 12 Oct 2023 10:43:16 GMT
STOPSIGNAL SIGQUIT
# Thu, 12 Oct 2023 10:43:17 GMT
EXPOSE 9000
# Thu, 12 Oct 2023 10:43:17 GMT
CMD ["php-fpm"]
# Fri, 13 Oct 2023 04:53:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 04:55:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libicu-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$extDir"/*.so 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 13 Oct 2023 04:55:30 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 13 Oct 2023 04:55:30 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 13 Oct 2023 04:55:35 GMT
RUN set -eux; 	version='6.3.1'; 	sha1='052777aef40e7f627c63c8a26eefe37b843a44df'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Fri, 13 Oct 2023 04:55:37 GMT
VOLUME [/var/www/html]
# Fri, 13 Oct 2023 04:55:37 GMT
COPY --chown=www-data:www-datafile:d38fd3c0db552e13465e83c5d7bbd85c7c3d036bf1285495988cc4ab2ffaf7f5 in /usr/src/wordpress/ 
# Fri, 13 Oct 2023 04:55:37 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Fri, 13 Oct 2023 04:55:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Oct 2023 04:55:38 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f270c1bb05fa46b165ce3680225dc9fa5bbfe4d69420a467350e80f692c78eb2`  
		Last Modified: Wed, 11 Oct 2023 17:56:03 GMT  
		Size: 27.5 MB (27512850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59099b3e94e78acfd6adc8820c2a313798026d8c737c60d48fbf605d1e5df9d`  
		Last Modified: Thu, 12 Oct 2023 11:10:08 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484bad2504e3e0824ec41110608fa975b667ce65bd9ce53f0897723c641d392f`  
		Last Modified: Thu, 12 Oct 2023 11:10:18 GMT  
		Size: 80.8 MB (80818715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:942fbd6ab4e770ca930aa91a3eaa2b9590459e4692028fd2c12dc9c29d989539`  
		Last Modified: Thu, 12 Oct 2023 11:10:07 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c653880e794814ee81ee18458a37254c35c9ec46de8de5ae219d8fb56908057e`  
		Last Modified: Thu, 12 Oct 2023 11:29:36 GMT  
		Size: 12.1 MB (12107482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b7ffab77716660a0f449141d360beee14bb3743872ad0fd46ff08ef3109f80`  
		Last Modified: Thu, 12 Oct 2023 11:29:34 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0fc8ebe25dcea789252f9731f21291857e87441eff85db3cf8d3f16402f3e5`  
		Last Modified: Thu, 12 Oct 2023 11:32:15 GMT  
		Size: 26.5 MB (26471378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5f1bd904115d3962a6a12187bce41b7c9cd15757713a0e3fed26e587940400`  
		Last Modified: Thu, 12 Oct 2023 11:32:11 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff64c78c099fdd8bc3dd082979a700ac81a6091960538ca5e471073f15ac6ee4`  
		Last Modified: Thu, 12 Oct 2023 11:32:11 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33e83dc7d031debc7af009e98fe79f775df027e8bc2618d1d6297afbeff8302`  
		Last Modified: Thu, 12 Oct 2023 11:32:11 GMT  
		Size: 8.9 KB (8884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff895c2994b85484dc685b4417f45245ef3f931f529c953c66ab599853a26ff8`  
		Last Modified: Fri, 13 Oct 2023 05:04:29 GMT  
		Size: 26.0 MB (26020516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475253865d2b3e4b09840f48d8a22530d617f316f07ea7a559dbdb04f1cabc89`  
		Last Modified: Fri, 13 Oct 2023 05:04:29 GMT  
		Size: 26.6 MB (26631248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f2db9bd1dc269ea4ae1e6088b5d44641d88d5280584a251e9d2ae6c9bf6e52`  
		Last Modified: Fri, 13 Oct 2023 05:04:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2ea9acd748a0766b85590d38491d06a49c0d82f148019e525ecbb7d184af39`  
		Last Modified: Fri, 13 Oct 2023 05:04:24 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f8344013eb9231d3d9f84b80113aca46d633ac85c55fb45064253768b13c75`  
		Last Modified: Fri, 13 Oct 2023 05:04:27 GMT  
		Size: 23.3 MB (23273546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3927967fc90f5acd8dbbed948193c649541de3ba364d9816fd4d85f1173519c`  
		Last Modified: Fri, 13 Oct 2023 05:04:24 GMT  
		Size: 2.3 KB (2349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a247cc892317b40ee8b9082f2ffcbea046c3d8e08bef641e7c5cacc29d5081d9`  
		Last Modified: Fri, 13 Oct 2023 05:04:24 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
