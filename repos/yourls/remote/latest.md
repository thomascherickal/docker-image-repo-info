## `yourls:latest`

```console
$ docker pull yourls@sha256:b7ed196ea16dca444a755c61443c0b7df3c2ef0bccd6785be31c598ff5cbbf6f
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

### `yourls:latest` - linux; amd64

```console
$ docker pull yourls@sha256:fb99091be0cdbf5fb93ac2e6df89fb8badadc2445c13e24b2834a043def7c737
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169815269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db00bb883dd3cc04fd0fde8eb1f3787b8382aa5ff93a61e6d048c68de2d04861`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 12:30:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 12:30:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 12:30:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 12:30:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 12:30:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 12:33:58 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 12:33:58 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 12:34:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 12:34:07 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 12:34:07 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 12:34:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 12:34:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 12:34:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 12:34:08 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 May 2022 13:00:59 GMT
ENV PHP_VERSION=8.1.5
# Wed, 11 May 2022 13:00:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.5.tar.xz.asc
# Wed, 11 May 2022 13:00:59 GMT
ENV PHP_SHA256=7647734b4dcecd56b7e4bd0bc55e54322fa3518299abcdc68eb557a7464a2e8a
# Wed, 11 May 2022 13:01:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 13:01:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 13:04:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 13:04:12 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 May 2022 13:04:13 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 13:04:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 13:04:13 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 May 2022 13:04:13 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 May 2022 13:04:13 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 13:04:13 GMT
EXPOSE 80
# Wed, 11 May 2022 13:04:13 GMT
CMD ["apache2-foreground"]
# Thu, 12 May 2022 04:18:02 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 12 May 2022 04:18:02 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 12 May 2022 04:18:02 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 12 May 2022 04:18:02 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 12 May 2022 04:18:02 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 12 May 2022 04:18:03 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 12 May 2022 04:18:03 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 12 May 2022 04:18:43 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 12 May 2022 04:18:43 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 04:18:44 GMT
RUN a2enmod rewrite expires
# Thu, 12 May 2022 04:18:44 GMT
ARG YOURLS_VERSION=1.9
# Thu, 12 May 2022 04:18:44 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 12 May 2022 04:18:44 GMT
LABEL org.opencontainers.image.version=1.9
# Thu, 12 May 2022 04:18:44 GMT
ENV YOURLS_VERSION=1.9
# Thu, 12 May 2022 04:18:44 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 12 May 2022 04:18:46 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 12 May 2022 04:18:46 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 12 May 2022 04:18:46 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 12 May 2022 04:18:47 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 12 May 2022 04:18:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 04:18:47 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd813a1b2cb8a76f5b4f268f422edd8f2cdea4c0354dd4762ea7b1d1e1c766de`  
		Last Modified: Wed, 11 May 2022 14:39:18 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cf7574573d0f63818130302247fc08e99f40a8c2b9b7be197cef5fe5006264`  
		Last Modified: Wed, 11 May 2022 14:39:31 GMT  
		Size: 91.6 MB (91601800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c27146d16e29ce547bb7328aca3930153a051520bbeb17e85b2548c164d71b`  
		Last Modified: Wed, 11 May 2022 14:39:18 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078f4450f949cf8479a92a7318d0596aa9a42aaf4a0b6770a30dee9d557430c3`  
		Last Modified: Wed, 11 May 2022 14:40:04 GMT  
		Size: 19.2 MB (19248594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f145e355bc44a3e4977431603bb5670c5a18d105dd8fbfda36c9e1d8500cfe8`  
		Last Modified: Wed, 11 May 2022 14:40:01 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc797cb9eeaeb3f771cd61108fec7f9846b4d2e12059cc4fb098774c4484a3c`  
		Last Modified: Wed, 11 May 2022 14:40:01 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64b282bc5121a2fd12095eab8e121e2c83973c815e94796731216ab93b8de07`  
		Last Modified: Wed, 11 May 2022 14:43:19 GMT  
		Size: 12.1 MB (12094359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99543e275b7195384c8ee700edc621ddc9c250e5f11bdae59c35df402573f485`  
		Last Modified: Wed, 11 May 2022 14:43:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ea612f371017c496b27b5a4787a6da91e0cca49b97ca84182380316c575e62`  
		Last Modified: Wed, 11 May 2022 14:43:18 GMT  
		Size: 11.0 MB (11025019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3cff1f668b12546f9386a9f0055e83de5bf0b4c30b2977326d4c73e729c6e2`  
		Last Modified: Wed, 11 May 2022 14:43:16 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacb7378c5bf4fba5bf4501cfa30b7f00fe4aec55c68e4d642750676bdd6d74c`  
		Last Modified: Wed, 11 May 2022 14:43:16 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c484c4329868b73a04b1d0314ea0aba36fbb3fe57e8d8767f97919067f1a8a97`  
		Last Modified: Wed, 11 May 2022 14:43:16 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566dc4711584a391f104f29a681c1e58e8b468d94c2808ee417a0975f01e240d`  
		Last Modified: Thu, 12 May 2022 04:19:57 GMT  
		Size: 511.5 KB (511506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f0b3b19ccf92adbe1b7c12aeb438e1e9b81deb5e00c85e5885f3cb83e42ba`  
		Last Modified: Thu, 12 May 2022 04:19:57 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:391f1a1624cbe049fb208a5870094d693ac9948f554e4131aa904d8494aa671d`  
		Last Modified: Thu, 12 May 2022 04:19:54 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987b53a7044cd19559cd5450a894451d3c6602e05061189deee9e6601589e968`  
		Last Modified: Thu, 12 May 2022 04:19:55 GMT  
		Size: 3.9 MB (3944332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a6911baad109eb07b30e9e674193183922cc3f07582167b72ba3bb5957e42d`  
		Last Modified: Thu, 12 May 2022 04:19:54 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d522d6884bec039b6f14ec01f786723a69301115e338cbf53746bb895781ba`  
		Last Modified: Thu, 12 May 2022 04:19:54 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ec500ded004749af29cd6a357e7e5a09c2c82de6dd7158deb3705d0337d2c4`  
		Last Modified: Thu, 12 May 2022 04:19:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; arm variant v5

```console
$ docker pull yourls@sha256:e729509f7c7ccf4554623e5b5de0c664d63a5e8ad4dfb30375f25711a2f9d234
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.4 MB (147400622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84371a6d850baf935de915347d98b795223fd126019c95e11af08bafd43318d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:50:34 GMT
ADD file:72357b75d7e4546f06abf4648ab600980e742a3017f36da3c7a6c086f2f5fb56 in / 
# Wed, 11 May 2022 00:50:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:01:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 09:01:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 09:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:02:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 09:02:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 09:08:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 09:08:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 09:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 09:08:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 09:08:28 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 09:08:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:08:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:08:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 09:08:30 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 May 2022 09:54:44 GMT
ENV PHP_VERSION=8.1.5
# Wed, 11 May 2022 09:54:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.5.tar.xz.asc
# Wed, 11 May 2022 09:54:45 GMT
ENV PHP_SHA256=7647734b4dcecd56b7e4bd0bc55e54322fa3518299abcdc68eb557a7464a2e8a
# Wed, 11 May 2022 09:55:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 09:55:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 10:00:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 10:00:23 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 May 2022 10:00:25 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 10:00:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 10:00:26 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 May 2022 10:00:26 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 May 2022 10:00:27 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 10:00:27 GMT
EXPOSE 80
# Wed, 11 May 2022 10:00:28 GMT
CMD ["apache2-foreground"]
# Thu, 12 May 2022 10:10:56 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 12 May 2022 10:10:57 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 12 May 2022 10:10:57 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 12 May 2022 10:10:58 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 12 May 2022 10:10:58 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 12 May 2022 10:10:58 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 12 May 2022 10:10:59 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 12 May 2022 10:12:02 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 12 May 2022 10:12:03 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 10:12:05 GMT
RUN a2enmod rewrite expires
# Thu, 12 May 2022 10:12:05 GMT
ARG YOURLS_VERSION=1.9
# Thu, 12 May 2022 10:12:05 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 12 May 2022 10:12:06 GMT
LABEL org.opencontainers.image.version=1.9
# Thu, 12 May 2022 10:12:06 GMT
ENV YOURLS_VERSION=1.9
# Thu, 12 May 2022 10:12:07 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 12 May 2022 10:12:11 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 12 May 2022 10:12:11 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 12 May 2022 10:12:12 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 12 May 2022 10:12:12 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 12 May 2022 10:12:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 10:12:13 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f7b69be15db1cb94a249f74b27edd4f5e5923a8701b026179a593f6888e897aa`  
		Last Modified: Wed, 11 May 2022 01:05:51 GMT  
		Size: 28.9 MB (28921122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2ff8b0532c87980261c55177d558e48990c19f64702896090e4a79e2493772`  
		Last Modified: Wed, 11 May 2022 12:55:39 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1566fe92ea5dc855b59bd00a5d07a309e42751c6913be13b05127b105588b1ab`  
		Last Modified: Wed, 11 May 2022 12:56:31 GMT  
		Size: 73.7 MB (73683798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa4ce106df6e3a09952012e2eb60204b4af3ea778df0eb37a9669fb59fc8a5f`  
		Last Modified: Wed, 11 May 2022 12:55:39 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f526d9160c51f75c6cf905f7dc968e7b02e076b4b3f54a171e1fc0044487b1ed`  
		Last Modified: Wed, 11 May 2022 12:57:19 GMT  
		Size: 18.5 MB (18545977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69af1625f8238b17d5b15e9cd14dfb0642c504e0cd4f579aa26edcb6b06852a3`  
		Last Modified: Wed, 11 May 2022 12:57:09 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d55c9a2d6b80faee3aeb823d120bccf7a0154c462494a3e0550e9be490ccd8`  
		Last Modified: Wed, 11 May 2022 12:57:09 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207e91e6346db90e6995e9c03b769971cb20524ee74f1444751f25fd57ee9b61`  
		Last Modified: Wed, 11 May 2022 13:02:48 GMT  
		Size: 12.1 MB (12092972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7ac1450282c9ec37594d493fc165bfd37c0548403b9026d6b0843dad072dbf`  
		Last Modified: Wed, 11 May 2022 13:02:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570300d28a01d5e546f18d251d25fefec61aa9bf9c1b681df752241604ef3780`  
		Last Modified: Wed, 11 May 2022 13:02:51 GMT  
		Size: 10.1 MB (10051417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05efb1685aaa697ff0b7a91fe0adf30e43f92aefcd5249bf2e74270e78b09e81`  
		Last Modified: Wed, 11 May 2022 13:02:43 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf924f483efc77035aa9bf17da93116178584988539e380d142bc57b7895d1ba`  
		Last Modified: Wed, 11 May 2022 13:02:43 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40782107e24b9c196e3b5b4475771fe0ba98166f2b179911d79dd3de483b4fce`  
		Last Modified: Wed, 11 May 2022 13:02:43 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c03502296ce79733ecb52c665b1966811f0f7becb0fee50662a3bf586c802df`  
		Last Modified: Thu, 12 May 2022 10:14:43 GMT  
		Size: 150.8 KB (150805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a888314507c551d625413b8cc07ebdcea45b7a516c4960f0d6e75b1ad529d1`  
		Last Modified: Thu, 12 May 2022 10:14:43 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276df41c7a46d745d3bdb1f541c48153c80273cab63d84dd8a75a1704d048594`  
		Last Modified: Thu, 12 May 2022 10:14:41 GMT  
		Size: 351.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4c1d2172fa0b648acad6d98c257f2b1f9a67ed5334ce565eb9957928d5013a`  
		Last Modified: Thu, 12 May 2022 10:14:44 GMT  
		Size: 3.9 MB (3944322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9beec4afd372255bcb7a207e3cc934cf01215e73dae086efaa706220cb49cb6d`  
		Last Modified: Thu, 12 May 2022 10:14:42 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b524230775f43a0c816ae950b808413173584b17ce210af89b4716b58d25af8`  
		Last Modified: Thu, 12 May 2022 10:14:41 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f87c2de8c571bd20eef459cdcfe07e71824df806fffcae9d70798dc77e2cce`  
		Last Modified: Thu, 12 May 2022 10:14:41 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; arm variant v7

```console
$ docker pull yourls@sha256:2b5d372616a18f00e8084d8a4a64fd400f5082b70cda93b9d4aebe96ec38bbea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139603440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9031360c30150fd70221c599f12227825f9167eef947f976663004f56217d45b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:49:07 GMT
ADD file:7c0451fffe8a520c2ab23048948d76bfe0dc0d90298c3d859279ccd8815b84f6 in / 
# Wed, 11 May 2022 01:49:08 GMT
CMD ["bash"]
# Wed, 11 May 2022 13:37:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 13:37:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 13:37:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 13:37:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 13:37:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 13:43:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 13:43:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 13:43:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 13:43:23 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 13:43:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 13:43:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 13:43:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 13:43:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 13:43:27 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 May 2022 14:26:39 GMT
ENV PHP_VERSION=8.1.5
# Wed, 11 May 2022 14:26:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.5.tar.xz.asc
# Wed, 11 May 2022 14:26:40 GMT
ENV PHP_SHA256=7647734b4dcecd56b7e4bd0bc55e54322fa3518299abcdc68eb557a7464a2e8a
# Wed, 11 May 2022 14:27:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 14:27:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 14:31:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 14:31:40 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 May 2022 14:31:42 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 14:31:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 14:31:43 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 May 2022 14:31:43 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 May 2022 14:31:44 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 14:31:44 GMT
EXPOSE 80
# Wed, 11 May 2022 14:31:44 GMT
CMD ["apache2-foreground"]
# Fri, 13 May 2022 03:39:05 GMT
LABEL org.opencontainers.image.title=YOURLS
# Fri, 13 May 2022 03:39:06 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Fri, 13 May 2022 03:39:06 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Fri, 13 May 2022 03:39:06 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Fri, 13 May 2022 03:39:07 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Fri, 13 May 2022 03:39:07 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Fri, 13 May 2022 03:39:08 GMT
LABEL org.opencontainers.image.licenses=MIT
# Fri, 13 May 2022 03:40:10 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Fri, 13 May 2022 03:40:11 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 13 May 2022 03:40:13 GMT
RUN a2enmod rewrite expires
# Fri, 13 May 2022 03:40:13 GMT
ARG YOURLS_VERSION=1.9
# Fri, 13 May 2022 03:40:14 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Fri, 13 May 2022 03:40:14 GMT
LABEL org.opencontainers.image.version=1.9
# Fri, 13 May 2022 03:40:14 GMT
ENV YOURLS_VERSION=1.9
# Fri, 13 May 2022 03:40:15 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Fri, 13 May 2022 03:40:19 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 13 May 2022 03:40:19 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Fri, 13 May 2022 03:40:20 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Fri, 13 May 2022 03:40:20 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Fri, 13 May 2022 03:40:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 May 2022 03:40:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1a9427b75b1c1db800cae7a9199bb4e508702e6761b17cc904d21441df43016c`  
		Last Modified: Wed, 11 May 2022 02:04:35 GMT  
		Size: 26.6 MB (26575672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0954e79492a980b9f2b5d48b790a35ab6a1c2ecf4930e9f13b753ed3929a89`  
		Last Modified: Wed, 11 May 2022 17:27:23 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8358c2337fd2fea1131efaae1584f9c388558f58e3e9656c3be2104eb52389`  
		Last Modified: Wed, 11 May 2022 17:28:06 GMT  
		Size: 69.3 MB (69316792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bd5bbec50e54eb7b4a5c1704f8ea26334c39b37b3c1337ffbd5646eb91854c`  
		Last Modified: Wed, 11 May 2022 17:27:23 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d79088b731d8ab13155fba86472c220dffdbfaadfec2f6e7af1592e6d5d0e8`  
		Last Modified: Wed, 11 May 2022 17:28:55 GMT  
		Size: 18.0 MB (17993556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be981561fdd07d9b5e8c9d8f7a821e2ba278d4a107d8c42fe0ecbc8f1ed568b`  
		Last Modified: Wed, 11 May 2022 17:28:44 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fdf33ccba4032a7fb0cd0d957accc85ea726fdbc3393e9f359ab07cf6005a3c`  
		Last Modified: Wed, 11 May 2022 17:28:44 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97965cbda4afdb3714f6c6bbe4ea5071325cc5224d0638a66979dc769dc23b9e`  
		Last Modified: Wed, 11 May 2022 17:34:50 GMT  
		Size: 12.1 MB (12093029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c8797db24df801cf0b532709a86ff2a312469eb8d4147e85927aed311bee9f3`  
		Last Modified: Wed, 11 May 2022 17:34:45 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf2c6f9bab99be0160a56294724f5f84052d353454f9d5127ab159d16d447fe`  
		Last Modified: Wed, 11 May 2022 17:34:52 GMT  
		Size: 9.5 MB (9531226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fee31192f6f7621367a12b73f3f89f77f84df9d67a68f624fb8613c91ac6a17`  
		Last Modified: Wed, 11 May 2022 17:34:45 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d8ae4b3794ec95e7a6a9698c0b649a9c5bfb85f357034fa3f314007176f938`  
		Last Modified: Wed, 11 May 2022 17:34:45 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36026ba04e83f9e86eb9a97a209ccf86b1a0d1d22529af69b778071ca3abb561`  
		Last Modified: Wed, 11 May 2022 17:34:45 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2abdc424db835995f9a2ee2c43c135d621abce65322d5ad9cf3a712ae96c9ea`  
		Last Modified: Fri, 13 May 2022 03:43:16 GMT  
		Size: 138.6 KB (138638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ac4e69ffbc53cb6ef885b769ca65374a126cef6798b3420428eecd45c24776`  
		Last Modified: Fri, 13 May 2022 03:43:16 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc326b0830b569991f0e0a26dd9c14af8819c4826a594628f606b64d936ee31`  
		Last Modified: Fri, 13 May 2022 03:43:14 GMT  
		Size: 349.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed024f5e164c496313fd9045da6440eeb1dbcfda3366db9a61231f8cf01330b`  
		Last Modified: Fri, 13 May 2022 03:43:18 GMT  
		Size: 3.9 MB (3944323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b230ff34f1181100aac14e7e27e9261d06396156e5e79bb49ee35191f26884a9`  
		Last Modified: Fri, 13 May 2022 03:43:14 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7dcbf17094ca65932d8a3890bd28644f5a460a3caeb7e31b364cac87def4626`  
		Last Modified: Fri, 13 May 2022 03:43:15 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e13f024b84aed4f833cba86a5eda5e29433ac8381c26a2fdc03703df73687b`  
		Last Modified: Fri, 13 May 2022 03:43:14 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:e3038df0823ce402f47abc1d520b8257a39ac1360c7b68cce791d9e52fbd3b50
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.4 MB (163447812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be280235653e90faa9d7b3151a07438aca13133211d24c29d38f7798c812996e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 05:09:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 05:09:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 05:10:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 05:10:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 05:10:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 05:14:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 05:14:27 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 05:14:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 05:14:36 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 05:14:37 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 05:14:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 05:14:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 05:14:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 05:14:41 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 May 2022 05:48:24 GMT
ENV PHP_VERSION=8.1.5
# Wed, 11 May 2022 05:48:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.5.tar.xz.asc
# Wed, 11 May 2022 05:48:26 GMT
ENV PHP_SHA256=7647734b4dcecd56b7e4bd0bc55e54322fa3518299abcdc68eb557a7464a2e8a
# Wed, 11 May 2022 05:48:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 05:48:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 05:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 05:52:19 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 May 2022 05:52:19 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 05:52:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 05:52:21 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 May 2022 05:52:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 May 2022 05:52:23 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 05:52:24 GMT
EXPOSE 80
# Wed, 11 May 2022 05:52:25 GMT
CMD ["apache2-foreground"]
# Wed, 11 May 2022 23:14:21 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 11 May 2022 23:14:22 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 11 May 2022 23:14:23 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 11 May 2022 23:14:24 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 11 May 2022 23:14:25 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 11 May 2022 23:14:26 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 11 May 2022 23:14:27 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 11 May 2022 23:15:41 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 11 May 2022 23:15:42 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 May 2022 23:15:43 GMT
RUN a2enmod rewrite expires
# Wed, 11 May 2022 23:15:44 GMT
ARG YOURLS_VERSION=1.9
# Wed, 11 May 2022 23:15:45 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Wed, 11 May 2022 23:15:46 GMT
LABEL org.opencontainers.image.version=1.9
# Wed, 11 May 2022 23:15:47 GMT
ENV YOURLS_VERSION=1.9
# Wed, 11 May 2022 23:15:48 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Wed, 11 May 2022 23:15:51 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 11 May 2022 23:15:52 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 11 May 2022 23:15:53 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 11 May 2022 23:15:54 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 11 May 2022 23:15:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 23:15:55 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad610f0f8b379f259a51b01495d1b006606e8320949fe72660f38e01cb489a5`  
		Last Modified: Wed, 11 May 2022 07:34:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8144c565ce19428ab5ed0e19ff493df33b73544363c34ebb7fe3e0db906ecec`  
		Last Modified: Wed, 11 May 2022 07:34:36 GMT  
		Size: 86.7 MB (86717272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d881248602f9812f673802e2b5968730890d16b900940453fe7cf887097f8630`  
		Last Modified: Wed, 11 May 2022 07:34:23 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08737d8f4766c7838fcb3e075fe5a3f2574355f0c8614cb5f061536ad54cae36`  
		Last Modified: Wed, 11 May 2022 07:35:12 GMT  
		Size: 18.9 MB (18943653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581b3736d6717151a7139e945e58ad4801c5a7c95603c075e4ca79ce77ac7027`  
		Last Modified: Wed, 11 May 2022 07:35:09 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d1b76adda2961f8cadf21ba7c5a4ec8ec0c10c47487ee91b30b74eba922350`  
		Last Modified: Wed, 11 May 2022 07:35:09 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95537678b4a07b1a1dfd5a6dc9f9ad92d942d28cbefbaaa4158f4277a9dc21b`  
		Last Modified: Wed, 11 May 2022 07:38:51 GMT  
		Size: 11.9 MB (11877118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2cf676007c89e956b48f5f162e014bcc5d54fd7c504fd2efac83403dc410be`  
		Last Modified: Wed, 11 May 2022 07:38:48 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f877047d2bf58869d7337db8209c2a1f993fb7f9426d1eb291687feb98a8156`  
		Last Modified: Wed, 11 May 2022 07:38:50 GMT  
		Size: 11.1 MB (11094374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d904c486a97063c6cd043c574662015c192efa593a4819aac3cb20156eef4d0`  
		Last Modified: Wed, 11 May 2022 07:38:48 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d343b473e9987549824bd1e8a194d3b2e2984819639a5d05d7ed91bcafe4236`  
		Last Modified: Wed, 11 May 2022 07:38:48 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feffd043bd85030e72b80d07e473a65da1da54cd74ac1ff78954f08bc9033445`  
		Last Modified: Wed, 11 May 2022 07:38:48 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92923437d9b59d0a4147f10281dae0ac512bccc824e0aa2fb1ca138b15444162`  
		Last Modified: Wed, 11 May 2022 23:18:16 GMT  
		Size: 795.4 KB (795352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c3584e6b97d7d5c085c4357bb902889b20efc59a3bc4c632adcb934e403876`  
		Last Modified: Wed, 11 May 2022 23:18:15 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602204350a5ddb7a208585ec230ed22ae3e353885c39f75b12b43f785496526b`  
		Last Modified: Wed, 11 May 2022 23:18:13 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0a2eb794e9dd92b936070b3930f6552120663cc6aa72a0883df96a47e9d6ea`  
		Last Modified: Wed, 11 May 2022 23:18:13 GMT  
		Size: 3.9 MB (3944286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e731dc84d5d8e6cca5f051580c25bb9df08b5fee87d448ca7e49297b511f2a`  
		Last Modified: Wed, 11 May 2022 23:18:12 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fad342d2fb8191f108e73c413a9178be949ea26d4e55a30ad935e30b37e5635`  
		Last Modified: Wed, 11 May 2022 23:18:13 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e33c02992692954a1af569ab65d77bd98316f67aba29802f0ffd8bc4d9a2d41`  
		Last Modified: Wed, 11 May 2022 23:18:13 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; 386

```console
$ docker pull yourls@sha256:6c9c7320a72ed3fade68e09e067baa116a30342c24932db6edeb6e4dd007409f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.0 MB (171972768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c285e821087c390264f15014ca5dad16cf13e192ca76e3efe5acf3a6a6538a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
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
# Wed, 11 May 2022 07:16:10 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 May 2022 07:42:20 GMT
ENV PHP_VERSION=8.1.5
# Wed, 11 May 2022 07:42:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.5.tar.xz.asc
# Wed, 11 May 2022 07:42:21 GMT
ENV PHP_SHA256=7647734b4dcecd56b7e4bd0bc55e54322fa3518299abcdc68eb557a7464a2e8a
# Wed, 11 May 2022 07:42:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 07:42:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 07:45:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 07:45:21 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 May 2022 07:45:21 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 07:45:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 07:45:23 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 May 2022 07:45:25 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 May 2022 07:45:25 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 07:45:26 GMT
EXPOSE 80
# Wed, 11 May 2022 07:45:27 GMT
CMD ["apache2-foreground"]
# Wed, 11 May 2022 18:25:42 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 11 May 2022 18:25:43 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 11 May 2022 18:25:44 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 11 May 2022 18:25:45 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 11 May 2022 18:25:46 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 11 May 2022 18:25:47 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 11 May 2022 18:25:48 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 11 May 2022 18:26:25 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 11 May 2022 18:26:25 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 May 2022 18:26:26 GMT
RUN a2enmod rewrite expires
# Wed, 11 May 2022 18:26:27 GMT
ARG YOURLS_VERSION=1.9
# Wed, 11 May 2022 18:26:28 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Wed, 11 May 2022 18:26:29 GMT
LABEL org.opencontainers.image.version=1.9
# Wed, 11 May 2022 18:26:30 GMT
ENV YOURLS_VERSION=1.9
# Wed, 11 May 2022 18:26:31 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Wed, 11 May 2022 18:26:34 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 11 May 2022 18:26:35 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 11 May 2022 18:26:36 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 11 May 2022 18:26:37 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 11 May 2022 18:26:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 18:26:38 GMT
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
	-	`sha256:43bad42296d71a98e5eaa9cd1b7fd77273708b27f3662b0bbf701d38fded151b`  
		Last Modified: Wed, 11 May 2022 09:28:43 GMT  
		Size: 11.9 MB (11877151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a000e22f47fd10e799e15cdee37062341c5913fffa8cd3b80a0fed10305118`  
		Last Modified: Wed, 11 May 2022 09:28:39 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b7676152207653fd95fb6b21deee4d26b64aefa9548d758f3f031acca2d3f5`  
		Last Modified: Wed, 11 May 2022 09:28:41 GMT  
		Size: 11.2 MB (11246671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5c92e35420cfd799165d5508637af937800c52dbaf8668e256ab3239fed48c`  
		Last Modified: Wed, 11 May 2022 09:28:39 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6082b8911b04af7f8dedb86f25184f4dcfec5ff378df6530981765a18375a2`  
		Last Modified: Wed, 11 May 2022 09:28:39 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77c80178d6ef33f34fe68f62223307c4db45c6a5ab69293440438ab138f9778`  
		Last Modified: Wed, 11 May 2022 09:28:39 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7444effa5cd3b071fdc1fb40277ce8d9c37f87f9531d8c4a2fda995b565ec1`  
		Last Modified: Wed, 11 May 2022 18:28:20 GMT  
		Size: 492.3 KB (492276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b13b92d5fcf35bfa09dfb8d32f7ae6811bbd46a501ff4fe77f2a7b61351de4`  
		Last Modified: Wed, 11 May 2022 18:28:19 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95908305f679f9c774485be5be4e4a2dabb146fa54ef89f21c2330aa0742c3e7`  
		Last Modified: Wed, 11 May 2022 18:28:17 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f6505e680fc44e379110c022b96abbbbf296d045453ec320cacc521d6ecc46`  
		Last Modified: Wed, 11 May 2022 18:28:18 GMT  
		Size: 3.9 MB (3944286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e00429444ff73b7fd6be93d326a6a2eade8e622b0fc963c91efd3e28c366f7`  
		Last Modified: Wed, 11 May 2022 18:28:17 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e609c430e1d422855dd32e705c278ce292d2ed1c369048a0b758490f607a3423`  
		Last Modified: Wed, 11 May 2022 18:28:17 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5bfbc589483d75cabc03387dcd181e059d252c9510372fd1fac9a0512d2ccf4`  
		Last Modified: Wed, 11 May 2022 18:28:17 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; mips64le

```console
$ docker pull yourls@sha256:74a84cf99217ca43705235bef43535f186ceb5c859fe6b4be882245afae1869d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.5 MB (146538426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f34f82fcce6d2a8ec546dd736b6a131c1b670fa43defa11fd10f398dc2e3dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
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
# Thu, 21 Apr 2022 18:16:53 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 21 Apr 2022 18:16:56 GMT
ENV PHP_VERSION=8.1.5
# Thu, 21 Apr 2022 18:17:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.5.tar.xz.asc
# Thu, 21 Apr 2022 18:17:03 GMT
ENV PHP_SHA256=7647734b4dcecd56b7e4bd0bc55e54322fa3518299abcdc68eb557a7464a2e8a
# Thu, 21 Apr 2022 18:17:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Apr 2022 18:17:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Apr 2022 18:31:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Apr 2022 18:31:28 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 21 Apr 2022 18:31:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Apr 2022 18:31:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Apr 2022 18:31:43 GMT
STOPSIGNAL SIGWINCH
# Thu, 21 Apr 2022 18:31:46 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 21 Apr 2022 18:31:50 GMT
WORKDIR /var/www/html
# Thu, 21 Apr 2022 18:31:53 GMT
EXPOSE 80
# Thu, 21 Apr 2022 18:31:57 GMT
CMD ["apache2-foreground"]
# Wed, 27 Apr 2022 19:12:56 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 27 Apr 2022 19:13:00 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 27 Apr 2022 19:13:03 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 27 Apr 2022 19:13:07 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 27 Apr 2022 19:13:10 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 27 Apr 2022 19:13:14 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 27 Apr 2022 19:13:17 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 27 Apr 2022 19:14:24 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 27 Apr 2022 19:14:30 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 27 Apr 2022 19:14:36 GMT
RUN a2enmod rewrite expires
# Wed, 27 Apr 2022 19:14:40 GMT
ARG YOURLS_VERSION=1.9
# Wed, 27 Apr 2022 19:14:43 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Wed, 27 Apr 2022 19:14:47 GMT
LABEL org.opencontainers.image.version=1.9
# Wed, 27 Apr 2022 19:14:50 GMT
ENV YOURLS_VERSION=1.9
# Wed, 27 Apr 2022 19:14:54 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Wed, 27 Apr 2022 19:15:03 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 27 Apr 2022 19:15:07 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 27 Apr 2022 19:15:10 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 27 Apr 2022 19:15:13 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 27 Apr 2022 19:15:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 27 Apr 2022 19:15:20 GMT
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
	-	`sha256:1a876d7ed0fcfd6feb2a3df147651519de45db250c2e3ca5b8edd8cc80fce62c`  
		Last Modified: Thu, 21 Apr 2022 23:18:51 GMT  
		Size: 11.9 MB (11875997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fe787c565708ccf02669752fc31de39bf958494376783c571ae8c3234e3299`  
		Last Modified: Thu, 21 Apr 2022 23:18:45 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127678e78d99855c59c6e56b27852aea6c6f5485dffabf1a0f9b18344a9191b2`  
		Last Modified: Thu, 21 Apr 2022 23:18:54 GMT  
		Size: 10.2 MB (10174504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bfd7e2e3760673fe441614ecc890858504a9eec4559369aca8a273d3a2aaa4`  
		Last Modified: Thu, 21 Apr 2022 23:18:45 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad79edbf0332e320979b340a3c08845ef0ed392bc76c3b31650bfa544c939f3`  
		Last Modified: Thu, 21 Apr 2022 23:18:45 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e361881892cf6c9c57772d7687449e8042a2fab4521cde2805e88eca3a12ed3`  
		Last Modified: Thu, 21 Apr 2022 23:18:45 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e722772824df4c8fc7008a12c642d7af0d8700a596b1d8ea4b8e41a2e70757c1`  
		Last Modified: Wed, 27 Apr 2022 19:18:20 GMT  
		Size: 149.1 KB (149121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973ee82f05db050cd11233d0a2014bd3a4a661b643dd3c34ef0ca6a6261bb507`  
		Last Modified: Wed, 27 Apr 2022 19:18:20 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4504a0f323ed10101b4bda790ebb1ed8cddfb01a05e585d30382e9f252cdb8`  
		Last Modified: Wed, 27 Apr 2022 19:18:17 GMT  
		Size: 352.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbc075cedd728ff788caca24a05a5dda542e85a09c0f11e327fa7408c1f6562`  
		Last Modified: Wed, 27 Apr 2022 19:18:21 GMT  
		Size: 3.9 MB (3944285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2d7f469c00010c52396bef3b07267dfe84d2f6fb6ba479b8b7a547334f3a9e`  
		Last Modified: Wed, 27 Apr 2022 19:18:17 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ad8502ad13f3c9a50f8df93ad3291c759e84aa9c35112363ac59cf9f00abc`  
		Last Modified: Wed, 27 Apr 2022 19:18:18 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6f7b1a25b0e9ebb04281f97abed8f06805bdb55733fd1e7aca026bfbf16ab8`  
		Last Modified: Wed, 27 Apr 2022 19:18:17 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; ppc64le

```console
$ docker pull yourls@sha256:2d9846b5e2006cab1ba48310618082d6c03d856191c2742a6707f842cd6ad09c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.0 MB (170018822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1d5bf3e976e571efabfa3b6143c57c9030fe70b65ad175c3c2999775a709a9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 01:32:29 GMT
ADD file:1e94716789ec21981460f74be38a668bc212bd804c1d41cecf90036a5bccac5a in / 
# Wed, 11 May 2022 01:32:34 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:46:05 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 15:46:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 15:47:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:47:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 15:47:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 15:54:47 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 15:54:52 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 15:56:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 15:56:38 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 15:56:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 15:56:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 15:56:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 15:56:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 15:56:57 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 May 2022 16:53:31 GMT
ENV PHP_VERSION=8.1.5
# Wed, 11 May 2022 16:53:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.5.tar.xz.asc
# Wed, 11 May 2022 16:53:40 GMT
ENV PHP_SHA256=7647734b4dcecd56b7e4bd0bc55e54322fa3518299abcdc68eb557a7464a2e8a
# Wed, 11 May 2022 16:54:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 16:54:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 17:00:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 17:00:43 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 May 2022 17:00:49 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 17:00:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 17:00:54 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 May 2022 17:00:56 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 May 2022 17:00:59 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 17:01:03 GMT
EXPOSE 80
# Wed, 11 May 2022 17:01:06 GMT
CMD ["apache2-foreground"]
# Thu, 12 May 2022 19:25:11 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 12 May 2022 19:25:13 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 12 May 2022 19:25:17 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 12 May 2022 19:25:19 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 12 May 2022 19:25:21 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 12 May 2022 19:25:24 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 12 May 2022 19:25:27 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 12 May 2022 19:26:14 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 12 May 2022 19:26:22 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 19:26:31 GMT
RUN a2enmod rewrite expires
# Thu, 12 May 2022 19:26:33 GMT
ARG YOURLS_VERSION=1.9
# Thu, 12 May 2022 19:26:36 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 12 May 2022 19:26:43 GMT
LABEL org.opencontainers.image.version=1.9
# Thu, 12 May 2022 19:26:49 GMT
ENV YOURLS_VERSION=1.9
# Thu, 12 May 2022 19:26:55 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 12 May 2022 19:27:05 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 12 May 2022 19:27:07 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 12 May 2022 19:27:10 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 12 May 2022 19:27:15 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Thu, 12 May 2022 19:27:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 12 May 2022 19:27:26 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:2533109ed11eefd6415e0370d6d7a3ea879b582b1887c98b819a598ad18fca24`  
		Last Modified: Wed, 11 May 2022 01:43:03 GMT  
		Size: 35.3 MB (35286467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371e62d3e51f3d14be9514e014a0c47381c71b4980f7df69274dfe7a3483d992`  
		Last Modified: Wed, 11 May 2022 20:00:12 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c36644b7fcb22a6d1cb83c25dc22b2cab2ad5b9afa4d1b019470f2c528781a`  
		Last Modified: Wed, 11 May 2022 20:01:07 GMT  
		Size: 86.6 MB (86626256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50fa70cc25099f203f1f6f9fe00d78b44559eb7b466c1477de32a4175b4af28`  
		Last Modified: Wed, 11 May 2022 20:00:12 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d70967b312bd4eb2894b309be2ad6881a7ca7080f3d9a921e9eb8f29615d9b66`  
		Last Modified: Wed, 11 May 2022 20:02:04 GMT  
		Size: 20.5 MB (20454041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab32495907fcbeca0a4d661d516a5a933fc681d838582ef13808f19f7b49d729`  
		Last Modified: Wed, 11 May 2022 20:01:47 GMT  
		Size: 480.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1e99f4e92b93fb786e7a2f3a13af0b7e83b9ebbbbde7ba4bc745add7baade2`  
		Last Modified: Wed, 11 May 2022 20:01:47 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fcedcce69eb93f36f1b19343954190e52c8eb787f4a07ad50482b198af9890`  
		Last Modified: Wed, 11 May 2022 20:07:24 GMT  
		Size: 12.1 MB (12094591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e789cc6f87598addc116cee399768788428a8e575f005feffaea96aaa9219c`  
		Last Modified: Wed, 11 May 2022 20:07:19 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4576c6236346bf67a942fe6bcac986ad9e5587a63594f6b63c27f91b22a6b223`  
		Last Modified: Wed, 11 May 2022 20:07:22 GMT  
		Size: 11.4 MB (11419040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ac9e467ee9ffcc29e1202fd350c63f6ae37e7b53cc8d11f11ba08ddb6b74f`  
		Last Modified: Wed, 11 May 2022 20:07:20 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3defbc02fb6060f3499a20f3eed78571d04b8ec64dae75a55a4d9316435d6e2`  
		Last Modified: Wed, 11 May 2022 20:07:19 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e74eadccae102eb2ca11def608bf01b65429e91f666c56e2d9cc2b29ebf05b1`  
		Last Modified: Wed, 11 May 2022 20:07:19 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b021a227db87ce999f67c46a725d32d5def088464b58ca4b1a3603b880f4fa1`  
		Last Modified: Thu, 12 May 2022 19:30:21 GMT  
		Size: 183.9 KB (183904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad787e459d6fdf51c096bfb5167a98dcb65e8ed9e0faba93046420b210573819`  
		Last Modified: Thu, 12 May 2022 19:30:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b63913428753df5285d00fa282916c08c82af6d648caafe823fb9a136f5b9f5`  
		Last Modified: Thu, 12 May 2022 19:30:17 GMT  
		Size: 347.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b793aa273810af5784fd27f6925b773b850a817bf445ab7e04d1fc9fe8a921`  
		Last Modified: Thu, 12 May 2022 19:30:18 GMT  
		Size: 3.9 MB (3944325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31c6d6dcfb2e009b48197b4429e0f31fc0dd675a9dc87b3d119d4e992efe60a`  
		Last Modified: Thu, 12 May 2022 19:30:17 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2555cdf8f09ed61772a056ed939389ba04e0ea1ece1755dcbba151a82baf2c37`  
		Last Modified: Thu, 12 May 2022 19:30:17 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c484dc6f33691c62e5e46e9516cb743ea88e7a1319dfae93bf3720c96aa4bbbb`  
		Last Modified: Thu, 12 May 2022 19:30:17 GMT  
		Size: 334.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:latest` - linux; s390x

```console
$ docker pull yourls@sha256:37f44a200a5cb46c53397abac3150f953244960cc6d28f342b0bd90fde7acd12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.7 MB (146699113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0594faa4de301ededd2293db900300dbe964ba1aab7b9299cb5e80bc048d2980`
-	Entrypoint: `["docker-entrypoint.sh"]`
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
# Wed, 11 May 2022 09:03:33 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 11 May 2022 09:25:27 GMT
ENV PHP_VERSION=8.1.5
# Wed, 11 May 2022 09:25:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.5.tar.xz.asc
# Wed, 11 May 2022 09:25:28 GMT
ENV PHP_SHA256=7647734b4dcecd56b7e4bd0bc55e54322fa3518299abcdc68eb557a7464a2e8a
# Wed, 11 May 2022 09:25:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 09:25:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 09:28:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 09:28:03 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 May 2022 09:28:04 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 09:28:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 09:28:04 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 May 2022 09:28:04 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 May 2022 09:28:04 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 09:28:05 GMT
EXPOSE 80
# Wed, 11 May 2022 09:28:05 GMT
CMD ["apache2-foreground"]
# Wed, 11 May 2022 19:45:33 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 11 May 2022 19:45:34 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 11 May 2022 19:45:34 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 11 May 2022 19:45:34 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 11 May 2022 19:45:34 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 11 May 2022 19:45:34 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 11 May 2022 19:45:34 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 11 May 2022 19:45:46 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 11 May 2022 19:45:47 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 May 2022 19:45:48 GMT
RUN a2enmod rewrite expires
# Wed, 11 May 2022 19:45:48 GMT
ARG YOURLS_VERSION=1.9
# Wed, 11 May 2022 19:45:48 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Wed, 11 May 2022 19:45:48 GMT
LABEL org.opencontainers.image.version=1.9
# Wed, 11 May 2022 19:45:48 GMT
ENV YOURLS_VERSION=1.9
# Wed, 11 May 2022 19:45:48 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Wed, 11 May 2022 19:45:50 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 11 May 2022 19:45:50 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 11 May 2022 19:45:50 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 11 May 2022 19:45:51 GMT
COPY file:5b7ff05d0c98ad759c4bec0ef8a7ce74cae42e95b42564b55f43b341c2c3e3f5 in /usr/src/yourls/ 
# Wed, 11 May 2022 19:45:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 19:45:51 GMT
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
	-	`sha256:d866976891c51cb0c6649d17aa9c116f93085c70a9a161a5c47e549e57cff0e9`  
		Last Modified: Wed, 11 May 2022 10:57:29 GMT  
		Size: 12.1 MB (12093343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a09c59c384c5559238fbf42306d28349ccf03817cf428d6c6876e91b53acd92`  
		Last Modified: Wed, 11 May 2022 10:57:27 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f335ecad248c43bd854a7c55363af2997d918e6d3ba4d86a221f6d11af94543`  
		Last Modified: Wed, 11 May 2022 10:57:29 GMT  
		Size: 10.2 MB (10162058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc47c4b447bcb4f19944d11639ee8cde1190c4b37d592126b92662f80cf63518`  
		Last Modified: Wed, 11 May 2022 10:57:27 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4874a6ca8c29b1bf5b606998e8001059f95d389859dc48e90bbce5712b937099`  
		Last Modified: Wed, 11 May 2022 10:57:27 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc16c05613992ae9c6300697664137cd48a007534a137b5f726971e308ba960b`  
		Last Modified: Wed, 11 May 2022 10:57:27 GMT  
		Size: 890.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb477d2548de0af6f8de0199035223e3f718e4bf4cdceae09719dcaabcccb6f`  
		Last Modified: Wed, 11 May 2022 19:46:54 GMT  
		Size: 158.3 KB (158300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84acc571ca2b7970ef3664f2f8f481a18a0f65a0602a90d4f6b68b6ee466ec3b`  
		Last Modified: Wed, 11 May 2022 19:46:54 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d49a1b78d95974f59f3b3e72b7dad5c700fa3f94b4c385d3e521a10831755a`  
		Last Modified: Wed, 11 May 2022 19:46:53 GMT  
		Size: 348.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f14f63420da78870d88e9cbd546cbc30b7c9df6b10d71ec789cd50f79055a2`  
		Last Modified: Wed, 11 May 2022 19:46:53 GMT  
		Size: 3.9 MB (3944330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0944d992916143b3c4dca7bb882ecfe0dd7e884265d5c64a927df702cd66da24`  
		Last Modified: Wed, 11 May 2022 19:46:53 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638eb1d930eecd7dcc8996afc9308a3d34487f31dd23be8d4cfe66d40e5d8629`  
		Last Modified: Wed, 11 May 2022 19:46:53 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41dc5af283c678b61dd00151e72c1a671e90d4a4fd5ad761735cf9d6c7a0b087`  
		Last Modified: Wed, 11 May 2022 19:46:53 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
