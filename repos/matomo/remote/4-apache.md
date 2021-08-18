## `matomo:4-apache`

```console
$ docker pull matomo@sha256:8c93118c7f2cb90a42d09445ecfa0b537a1d41315a1424ed5c60bbccba2ec304
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

### `matomo:4-apache` - linux; amd64

```console
$ docker pull matomo@sha256:74c5a254ad1e52825facc149b980f17ef052a57bc245932e89b3e9f2faa64676
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.8 MB (165803088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da919fcd72a378d954df36104328ed0a877809b7b477a165c625cb990bd20af`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 12:15:20 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 12:15:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 12:15:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 12:15:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 12:15:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 12:23:01 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 17 Aug 2021 12:23:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 17 Aug 2021 12:23:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 17 Aug 2021 12:23:17 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 17 Aug 2021 12:23:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 17 Aug 2021 12:23:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 17 Aug 2021 12:23:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 17 Aug 2021 12:23:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 12:23:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 12:23:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Aug 2021 13:06:51 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 17 Aug 2021 13:06:51 GMT
ENV PHP_VERSION=7.4.22
# Tue, 17 Aug 2021 13:06:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.22.tar.xz.asc
# Tue, 17 Aug 2021 13:06:51 GMT
ENV PHP_SHA256=8e078cd7d2f49ac3fcff902490a5bb1addc885e7e3b0d8dd068f42c68297bde8
# Tue, 17 Aug 2021 13:07:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 13:07:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Aug 2021 13:09:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 17 Aug 2021 13:09:57 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 17 Aug 2021 13:09:58 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Aug 2021 13:09:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Aug 2021 13:09:58 GMT
STOPSIGNAL SIGWINCH
# Tue, 17 Aug 2021 13:09:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 17 Aug 2021 13:09:59 GMT
WORKDIR /var/www/html
# Tue, 17 Aug 2021 13:09:59 GMT
EXPOSE 80
# Tue, 17 Aug 2021 13:09:59 GMT
CMD ["apache2-foreground"]
# Wed, 18 Aug 2021 10:47:37 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 18 Aug 2021 10:48:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 10:48:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 18 Aug 2021 10:48:56 GMT
ENV MATOMO_VERSION=4.4.1
# Wed, 18 Aug 2021 10:50:19 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 10:50:19 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 18 Aug 2021 10:50:20 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Wed, 18 Aug 2021 10:50:20 GMT
VOLUME [/var/www/html]
# Wed, 18 Aug 2021 10:50:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 10:50:20 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4909824c2d9e8528562a0eeab6573b4553f598555dd0a29f6f3fb2c28f6e4f2`  
		Last Modified: Tue, 17 Aug 2021 14:14:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d250e5f539524d16c1024cbbc0ba50cbde53f2ffce91a99088af37712f9e89`  
		Last Modified: Tue, 17 Aug 2021 14:14:48 GMT  
		Size: 76.7 MB (76680781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb8ea4156ce7c000260f63ef26989a499cb20b8aea4f2d8a4cd0da0e79903b07`  
		Last Modified: Tue, 17 Aug 2021 14:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dff16f247612bdc649a6812c73ab44e71286a2037692fcb3a88c559d6b16603`  
		Last Modified: Tue, 17 Aug 2021 14:15:26 GMT  
		Size: 18.7 MB (18679463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a0e426f4978a362f05bfda76c1e18b1eaa725ca2d83355858a5da5c25f86f4`  
		Last Modified: Tue, 17 Aug 2021 14:15:21 GMT  
		Size: 485.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9b16cc5ea2fde828ecbd14ed17ddbf0e857873da06c49f677d75d555e1072a`  
		Last Modified: Tue, 17 Aug 2021 14:15:21 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa5bbe2d919ce010baa79710a3c63f76631c706f0adc56e3e04544f4ca3992b`  
		Last Modified: Tue, 17 Aug 2021 14:20:39 GMT  
		Size: 10.7 MB (10686722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5956e724a764e45b618cfb7be0a4c1dbd8211fd40e13395a04e5ddd2fdd492`  
		Last Modified: Tue, 17 Aug 2021 14:20:36 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38db6370a0c58ac36fcc77bb3d235d188498d9b225529546ea9b57ee8752b6da`  
		Last Modified: Tue, 17 Aug 2021 14:20:39 GMT  
		Size: 13.8 MB (13843056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a3b12ead431d3fc8e3bb0d6ad8473cbb157d240fef3c2844eca84d73a7563c`  
		Last Modified: Tue, 17 Aug 2021 14:20:36 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed367d0ca8e25a65c95959c990509b1f93c6c58ac311e341a3bd2742d09a7858`  
		Last Modified: Tue, 17 Aug 2021 14:20:36 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d3ce2320a1d20419b4a8aea1d6819d2528d1b1f54cb831d69609782dac90a3`  
		Last Modified: Tue, 17 Aug 2021 14:20:36 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235790c26192d459f15513c3a053ce679c06103e15c6ddaeba73fbdadf28f828`  
		Last Modified: Wed, 18 Aug 2021 10:53:05 GMT  
		Size: 3.2 MB (3186513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6302a35a617215439e953a5929ed7d8ad2e7625647648a30db5d24cf7d5ca951`  
		Last Modified: Wed, 18 Aug 2021 10:53:04 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c091fb0c6dd2ac1015d8d5d8e72a333261768ddb08482f6c6bc9ae2bfc639a`  
		Last Modified: Wed, 18 Aug 2021 10:53:07 GMT  
		Size: 15.6 MB (15574310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86410109abd0e089f0188ee9380a2aba251041cd8c261b4aec4707033e8e15ad`  
		Last Modified: Wed, 18 Aug 2021 10:53:04 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8d3396354ec4fd5781bb26a897b5782426d2271dca8e208de99e65032bae69`  
		Last Modified: Wed, 18 Aug 2021 10:53:04 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-apache` - linux; arm variant v5

```console
$ docker pull matomo@sha256:2d591e8cc66a6d5ee31f9e178b66b040a4929da15d121ed5857b356f1fc6ec9f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.2 MB (163194049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449f58d655fffd7786ac5d4afff94957f77995404dce1aef86fe08f50b53e83c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 17 Aug 2021 01:55:48 GMT
ADD file:9ab41fbe9b84c147eb71d451b4d31f27a0eb362bb6d14ee3ba6279d67ae25531 in / 
# Tue, 17 Aug 2021 01:55:49 GMT
CMD ["bash"]
# Wed, 18 Aug 2021 08:33:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Aug 2021 08:33:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Aug 2021 08:34:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 08:34:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Aug 2021 08:34:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Aug 2021 08:40:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 18 Aug 2021 08:40:09 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 18 Aug 2021 08:40:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 18 Aug 2021 08:40:36 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 18 Aug 2021 08:40:38 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 18 Aug 2021 08:40:38 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 18 Aug 2021 08:40:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 18 Aug 2021 08:40:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Aug 2021 08:40:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Aug 2021 08:40:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Aug 2021 09:25:44 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 18 Aug 2021 09:25:44 GMT
ENV PHP_VERSION=7.4.22
# Wed, 18 Aug 2021 09:25:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.22.tar.xz.asc
# Wed, 18 Aug 2021 09:25:45 GMT
ENV PHP_SHA256=8e078cd7d2f49ac3fcff902490a5bb1addc885e7e3b0d8dd068f42c68297bde8
# Wed, 18 Aug 2021 09:26:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 09:26:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Aug 2021 09:30:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Aug 2021 09:30:11 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Wed, 18 Aug 2021 09:30:13 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Aug 2021 09:30:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Aug 2021 09:30:14 GMT
STOPSIGNAL SIGWINCH
# Wed, 18 Aug 2021 09:30:14 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 18 Aug 2021 09:30:15 GMT
WORKDIR /var/www/html
# Wed, 18 Aug 2021 09:30:15 GMT
EXPOSE 80
# Wed, 18 Aug 2021 09:30:16 GMT
CMD ["apache2-foreground"]
# Wed, 18 Aug 2021 13:10:59 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 18 Aug 2021 13:14:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 13:14:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 18 Aug 2021 13:14:46 GMT
ENV MATOMO_VERSION=4.4.1
# Wed, 18 Aug 2021 13:15:20 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 13:15:22 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 18 Aug 2021 13:15:22 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Wed, 18 Aug 2021 13:15:23 GMT
VOLUME [/var/www/html]
# Wed, 18 Aug 2021 13:15:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 13:15:23 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:91b48139ec3e0280b0a9be84b502b3d6394149000106be38ac11a1c31b59d956`  
		Last Modified: Tue, 17 Aug 2021 02:11:08 GMT  
		Size: 28.9 MB (28904169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa2796fe1de11330173a65d9c79bd200115ed2bbe4a010226c01033778d8c3f`  
		Last Modified: Wed, 18 Aug 2021 10:15:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb10f22b0293b7ff792f98dc678a22c7b6f3eca97496bef4e50daece21e0ee80`  
		Last Modified: Wed, 18 Aug 2021 10:16:19 GMT  
		Size: 73.7 MB (73670748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ea0ba062254d8e5013c25abe70301cc348d021f0813a2d82181961a2b48c50`  
		Last Modified: Wed, 18 Aug 2021 10:15:31 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5008017b2ff93a998b2ed04b0d3cddabd0df1d59bee90c66e9ed6d6af66859`  
		Last Modified: Wed, 18 Aug 2021 10:17:17 GMT  
		Size: 18.5 MB (18523066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adc384e97a58bed5588c04e8f1b38dda571fb3abd02f78859396a4f88d84af3`  
		Last Modified: Wed, 18 Aug 2021 10:17:06 GMT  
		Size: 484.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c856b3f94fae66ce8d19e9722a35d944808ee96f5532cfae449a690c448f2317`  
		Last Modified: Wed, 18 Aug 2021 10:17:05 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d474b1becd484c2659712028760453283f97bfeee095eab48b5ce705c15c2df`  
		Last Modified: Wed, 18 Aug 2021 10:25:06 GMT  
		Size: 10.7 MB (10687597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c5e9c0f2634f974739f3ab97502e3c12d6127219cd92813df796bf9305b57d`  
		Last Modified: Wed, 18 Aug 2021 10:25:01 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed27f55db5465955ab4a87c8aa067c7e4f4b59cd191da72d0403306e76f6ca3`  
		Last Modified: Wed, 18 Aug 2021 10:25:11 GMT  
		Size: 13.0 MB (12978273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9d77fd4e33d3e1d23958f3f70a1376e1ba843e89d16a05545186a8ef373586`  
		Last Modified: Wed, 18 Aug 2021 10:25:01 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67dc463e76543cc8a26cdff08a709ed8d5b758413d5c2501957bcae6e348164d`  
		Last Modified: Wed, 18 Aug 2021 10:25:02 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7145b1d5a71a169462799b21b7e49af868e4fd194109125d479e9552e0463ab3`  
		Last Modified: Wed, 18 Aug 2021 10:25:01 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32da2ed3f6e71a9b4f1069ed2cb8bdcd64d23b8518a6d9d81f814578726ed3dd`  
		Last Modified: Wed, 18 Aug 2021 13:21:18 GMT  
		Size: 2.8 MB (2846235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ea3b813064f2d017603aee7e0bddd0a794e02e1a018fdfad77a223ce69ffaf`  
		Last Modified: Wed, 18 Aug 2021 13:21:16 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e845678c83254f7dacdf024c09ba9199697fbcfce2b57001b8c50c4e4da4c6c`  
		Last Modified: Wed, 18 Aug 2021 13:21:31 GMT  
		Size: 15.6 MB (15577692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b9ccd2eaa4d344768578254552b9b1b4c59403cd15f4e229c778d288f7272e`  
		Last Modified: Wed, 18 Aug 2021 13:21:16 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11295ac948b805082bd67d42d3d93d2172ad77e40d2080738966dd6476a2bb0`  
		Last Modified: Wed, 18 Aug 2021 13:21:16 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-apache` - linux; arm variant v7

```console
$ docker pull matomo@sha256:772c3ca983d9986dcab8dfa054a96bc00b82b94842ce394c941e397484904374
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141099816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:036e9161be774c93d0bbc9422ab4b6d8800967da15be38a098200435830b38aa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:36:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 22 Jul 2021 14:36:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 22 Jul 2021 14:37:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:37:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Jul 2021 14:37:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Jul 2021 14:42:39 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 22 Jul 2021 14:42:39 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 22 Jul 2021 14:43:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 22 Jul 2021 14:43:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 22 Jul 2021 14:43:04 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 22 Jul 2021 14:43:05 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 22 Jul 2021 14:43:05 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 22 Jul 2021 14:43:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 14:43:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 14:43:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Jul 2021 15:26:05 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Jul 2021 00:40:19 GMT
ENV PHP_VERSION=7.4.22
# Fri, 30 Jul 2021 00:40:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.22.tar.xz.asc
# Fri, 30 Jul 2021 00:40:20 GMT
ENV PHP_SHA256=8e078cd7d2f49ac3fcff902490a5bb1addc885e7e3b0d8dd068f42c68297bde8
# Fri, 30 Jul 2021 00:40:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 30 Jul 2021 00:40:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Jul 2021 00:44:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Jul 2021 00:44:33 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 30 Jul 2021 00:44:35 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Jul 2021 00:44:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Jul 2021 00:44:36 GMT
STOPSIGNAL SIGWINCH
# Fri, 30 Jul 2021 00:44:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 30 Jul 2021 00:44:37 GMT
WORKDIR /var/www/html
# Fri, 30 Jul 2021 00:44:37 GMT
EXPOSE 80
# Fri, 30 Jul 2021 00:44:37 GMT
CMD ["apache2-foreground"]
# Fri, 30 Jul 2021 05:28:21 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 30 Jul 2021 05:31:57 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 30 Jul 2021 05:31:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 02 Aug 2021 21:32:37 GMT
ENV MATOMO_VERSION=4.4.1
# Mon, 02 Aug 2021 21:33:10 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Aug 2021 21:33:11 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Mon, 02 Aug 2021 21:33:12 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Mon, 02 Aug 2021 21:33:12 GMT
VOLUME [/var/www/html]
# Mon, 02 Aug 2021 21:33:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 02 Aug 2021 21:33:13 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a6f750d4cc5b551e031499e5ced2f4e1692c17f980e3f3e9761851b1387df6`  
		Last Modified: Thu, 22 Jul 2021 16:43:33 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f840bf7e69f6fe9bd4011a2183f851a5cc6fc624d56bc9b46591cd2e53e0a944`  
		Last Modified: Thu, 22 Jul 2021 16:44:11 GMT  
		Size: 59.5 MB (59513541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee71535876e5795780f7bfcbfe8f27f77aa6f23604c136eca44283630cee1f2e`  
		Last Modified: Thu, 22 Jul 2021 16:43:33 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321c322abb00aaa1a1a9361dcc1b844d07f4a778a2740fda143e67b56903c197`  
		Last Modified: Thu, 22 Jul 2021 16:45:03 GMT  
		Size: 17.5 MB (17481720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b52be569cf1523c6fbe4bac9eb505e674557de2cb5e9225816da32d8412d43`  
		Last Modified: Thu, 22 Jul 2021 16:44:53 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6740a92d88c8a3cd252177314eb2726ed2630987afbdb2aa24475b31394a4ff7`  
		Last Modified: Thu, 22 Jul 2021 16:44:53 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4d688217fda9b0b98d360dff1ac30ce43b81a1bbfb24a6912c1e6b96110925`  
		Last Modified: Fri, 30 Jul 2021 01:51:27 GMT  
		Size: 10.7 MB (10684812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948d3097f492b6365352ccd497a20686898389fa04935977f3084a74b4c6ca4e`  
		Last Modified: Fri, 30 Jul 2021 01:51:22 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd12d0c11aff22c6de4ba9080094a52d465b7fd2f246bd058f2b99d68846d584`  
		Last Modified: Fri, 30 Jul 2021 01:51:30 GMT  
		Size: 12.2 MB (12225041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c10b70269fea247b479d05137fcfaa96208b77cc56f6db005715a1c3192630b`  
		Last Modified: Fri, 30 Jul 2021 01:51:22 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b18229b01945980566d61dbf04b99eb20438cf37fa4362cab3153448547a0e`  
		Last Modified: Fri, 30 Jul 2021 01:51:22 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09190746c068a9430fb61968bf10d6895b32c157d3207bdcf7198216fa8f472`  
		Last Modified: Fri, 30 Jul 2021 01:51:22 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccef7150610e783ad4bfc59e49725cda1e51a7ea3d24ea537c3fc6c80d917ee`  
		Last Modified: Fri, 30 Jul 2021 05:42:19 GMT  
		Size: 2.9 MB (2869772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802d22a1d2661ee4dbf45c893fe04cf6a3e45ca922ade34177e2e76048e89997`  
		Last Modified: Fri, 30 Jul 2021 05:42:17 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcec0e9835a6b234fb6ff013b9f4fef913f11e0ccae51cb334c21a30a86c9d89`  
		Last Modified: Mon, 02 Aug 2021 21:36:18 GMT  
		Size: 15.6 MB (15572695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2afef3bcd2e38c28afd7ebe7a8bb8a2fb386fd7298cd9f05d47657528bcf24`  
		Last Modified: Mon, 02 Aug 2021 21:36:02 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b32b9faa1f8e9241970c79e58d6a7aa581bc898137a711bf69fbea0ff6e4a4`  
		Last Modified: Mon, 02 Aug 2021 21:36:02 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-apache` - linux; arm64 variant v8

```console
$ docker pull matomo@sha256:9d40883eea0db5e023069bf3f35d07150f604a01fbc6e28201642d3b04957dec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **179.0 MB (179007281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5fbd669123dfc45875b980a80c1f684d8cc76304afed5ef99f7057e953945a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:04 GMT
ADD file:0a42d4a201f0ac7889187c3212fbdfc2747f31f36e690d59c22eec50fe542614 in / 
# Tue, 17 Aug 2021 01:46:05 GMT
CMD ["bash"]
# Wed, 18 Aug 2021 08:36:51 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 18 Aug 2021 08:36:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 18 Aug 2021 08:37:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 08:37:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 18 Aug 2021 08:37:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 18 Aug 2021 08:44:53 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 18 Aug 2021 08:44:53 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 18 Aug 2021 08:45:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 18 Aug 2021 08:45:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 18 Aug 2021 08:45:02 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 18 Aug 2021 08:45:02 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 18 Aug 2021 08:45:02 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 18 Aug 2021 08:45:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Aug 2021 08:45:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 18 Aug 2021 08:45:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Aug 2021 09:22:46 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 18 Aug 2021 09:22:46 GMT
ENV PHP_VERSION=7.4.22
# Wed, 18 Aug 2021 09:22:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.22.tar.xz.asc
# Wed, 18 Aug 2021 09:22:47 GMT
ENV PHP_SHA256=8e078cd7d2f49ac3fcff902490a5bb1addc885e7e3b0d8dd068f42c68297bde8
# Wed, 18 Aug 2021 09:23:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 09:23:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Aug 2021 09:25:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Aug 2021 09:25:28 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Wed, 18 Aug 2021 09:25:29 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Aug 2021 09:25:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Aug 2021 09:25:29 GMT
STOPSIGNAL SIGWINCH
# Wed, 18 Aug 2021 09:25:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 18 Aug 2021 09:25:30 GMT
WORKDIR /var/www/html
# Wed, 18 Aug 2021 09:25:30 GMT
EXPOSE 80
# Wed, 18 Aug 2021 09:25:30 GMT
CMD ["apache2-foreground"]
# Wed, 18 Aug 2021 17:40:47 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 18 Aug 2021 17:42:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 17:42:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 18 Aug 2021 17:42:04 GMT
ENV MATOMO_VERSION=4.4.1
# Wed, 18 Aug 2021 17:42:18 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 17:42:19 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 18 Aug 2021 17:42:19 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Wed, 18 Aug 2021 17:42:19 GMT
VOLUME [/var/www/html]
# Wed, 18 Aug 2021 17:42:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 17:42:20 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3716b9f3c2f9e7592f5b47c2e6e13e64132071620c7551e0aa3c5c248e106139`  
		Last Modified: Tue, 17 Aug 2021 01:53:29 GMT  
		Size: 30.0 MB (30048801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d866415d3ee37964a1368090e3c4aa263a48fd0596d75470d756470d733cd00`  
		Last Modified: Wed, 18 Aug 2021 10:00:40 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb031746844ed5917dd3fa8bcff68ca0473331bbaec575ef0d3dff53734d697`  
		Last Modified: Wed, 18 Aug 2021 10:00:54 GMT  
		Size: 86.9 MB (86921080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea9475b4efc00fba612481a916aadd4bc40f01a083b01782899c9f7715ca7b6`  
		Last Modified: Wed, 18 Aug 2021 10:00:39 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767477a4f5e70bffb50c946aa1fc4197beaa701d16c3fef70875896d90af90ff`  
		Last Modified: Wed, 18 Aug 2021 10:01:35 GMT  
		Size: 19.1 MB (19140098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e70956f9cd7382de463766d83f66dc5e6e508007d5789d102844fd61c7bba2`  
		Last Modified: Wed, 18 Aug 2021 10:01:32 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b033e02310007952146912558e123a95d512137579f209dca9419885b3d9cc31`  
		Last Modified: Wed, 18 Aug 2021 10:01:32 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca732bf83a660f6283e8c047b6aeb46e7b44d0fd114880aa55faaa5281629c`  
		Last Modified: Wed, 18 Aug 2021 10:08:03 GMT  
		Size: 10.7 MB (10688066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536d7c15ec5104c8a267a5a57630089b53df768f9f95addfa1c29acaf18e4242`  
		Last Modified: Wed, 18 Aug 2021 10:07:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38391707d72ca8754724d4025d00e6f065bcc2989bb4fe840ab698a199d05f53`  
		Last Modified: Wed, 18 Aug 2021 10:08:02 GMT  
		Size: 13.6 MB (13641231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ce64ec83f885972999eadae5337ee9c4156abcd9b50933aea26d9e1a887a3b4`  
		Last Modified: Wed, 18 Aug 2021 10:07:59 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783e21b616779e87c3b4f5d72301b0ff7806053093d38751141d065f49ccfc94`  
		Last Modified: Wed, 18 Aug 2021 10:07:59 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54709a2fdc517c2c0a009d1670f79b05728e0a0cc7583af0a8505bb3d55e7c53`  
		Last Modified: Wed, 18 Aug 2021 10:07:59 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d101f889c295e1404346c1b7c3948a682c847d9962c69bf6f24852088401ffcd`  
		Last Modified: Wed, 18 Aug 2021 17:44:52 GMT  
		Size: 3.0 MB (2983512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60eeb14208ef1fb9182e49efe5870e32a7550d07baec18396716f06a6bdc8a36`  
		Last Modified: Wed, 18 Aug 2021 17:44:51 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa05ec7f75f8cf4d1518a5ff1d4971dee4bdaf5c960ecdc740e5b39048052fd`  
		Last Modified: Wed, 18 Aug 2021 17:44:55 GMT  
		Size: 15.6 MB (15578240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700e1d3ab831132aee896d2c251c585f4fd9b27edc7a521c73f6d876f075ed7d`  
		Last Modified: Wed, 18 Aug 2021 17:44:51 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b270b8cab62d20f3dbad30e40144fd044a7ebe15ef5ff92ca8961c3f2344bee3`  
		Last Modified: Wed, 18 Aug 2021 17:44:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-apache` - linux; 386

```console
$ docker pull matomo@sha256:c7a1697c2b5c9b2649d48cd8d92f988f22bf76eec13bdffb7099c347c186e690
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.3 MB (188343030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1059c14144deec2f9bf9c845b5f9edae39cc71337e5974605a9e511a5be9631`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 17 Aug 2021 01:40:28 GMT
ADD file:9afc107c0880864c9f16852bb6cc272a068f2c82a2df7c3444bbbc533f377156 in / 
# Tue, 17 Aug 2021 01:40:29 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 21:52:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 21:52:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 21:53:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 21:53:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 21:53:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 22:02:38 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 17 Aug 2021 22:02:38 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 17 Aug 2021 22:02:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 17 Aug 2021 22:02:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 17 Aug 2021 22:03:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 17 Aug 2021 22:03:01 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 17 Aug 2021 22:03:02 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 17 Aug 2021 22:03:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 22:03:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 22:03:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 17 Aug 2021 23:17:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 17 Aug 2021 23:17:58 GMT
ENV PHP_VERSION=7.4.22
# Tue, 17 Aug 2021 23:17:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.22.tar.xz.asc
# Tue, 17 Aug 2021 23:17:59 GMT
ENV PHP_SHA256=8e078cd7d2f49ac3fcff902490a5bb1addc885e7e3b0d8dd068f42c68297bde8
# Tue, 17 Aug 2021 23:18:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 23:18:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 17 Aug 2021 23:22:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 17 Aug 2021 23:23:00 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Tue, 17 Aug 2021 23:23:01 GMT
RUN docker-php-ext-enable sodium
# Tue, 17 Aug 2021 23:23:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 17 Aug 2021 23:23:01 GMT
STOPSIGNAL SIGWINCH
# Tue, 17 Aug 2021 23:23:02 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 17 Aug 2021 23:23:02 GMT
WORKDIR /var/www/html
# Tue, 17 Aug 2021 23:23:02 GMT
EXPOSE 80
# Tue, 17 Aug 2021 23:23:02 GMT
CMD ["apache2-foreground"]
# Wed, 18 Aug 2021 02:20:08 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 18 Aug 2021 02:23:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 02:23:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 18 Aug 2021 02:23:06 GMT
ENV MATOMO_VERSION=4.4.1
# Wed, 18 Aug 2021 02:23:29 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 02:23:30 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 18 Aug 2021 02:23:31 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Wed, 18 Aug 2021 02:23:31 GMT
VOLUME [/var/www/html]
# Wed, 18 Aug 2021 02:23:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 02:23:32 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6edd81381c438b83d2749dc056d46cd53320e27fb010b3e931ca1f0a752ddc07`  
		Last Modified: Tue, 17 Aug 2021 01:49:56 GMT  
		Size: 32.4 MB (32375657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde02ea43ea712182954343ee01b737ca6911ebdd1527d70da58d27b7a783340`  
		Last Modified: Wed, 18 Aug 2021 00:29:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75e82c83c65eda18ff4d7179d4b89c554a2792d4c36b04e03c2b9ede6515962`  
		Last Modified: Wed, 18 Aug 2021 00:29:45 GMT  
		Size: 92.7 MB (92712724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de8bb8fa63c86a9b01ad32ac4d7d10c7c3908efd8781160574009a46d9ec957`  
		Last Modified: Wed, 18 Aug 2021 00:29:23 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5020b8eb36c1dc1fdc847b0f9e27801ed927145025fa69137fd038e46f734cb`  
		Last Modified: Wed, 18 Aug 2021 00:30:31 GMT  
		Size: 19.7 MB (19691617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75db0c00c48f5a0fb6ca36f599e66882fbf1cb0a0ebccdfeb6c8df7d16448874`  
		Last Modified: Wed, 18 Aug 2021 00:30:24 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a535ab9a73ebe90cfb772df39ddb9b18ce3f36465cdc40ad268b1aebe247ff78`  
		Last Modified: Wed, 18 Aug 2021 00:30:24 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d3bb4f3f32fef0884297ebc9265b8149bf69aebf62e967ac9d0f9de69ec2d2`  
		Last Modified: Wed, 18 Aug 2021 00:39:15 GMT  
		Size: 10.7 MB (10688132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf55f0ed6d6a4152d3404cbd31c1c0bbe3bea2f45da121ea17d213d080861ee`  
		Last Modified: Wed, 18 Aug 2021 00:39:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d74832073247f5b027114d72105615aaed9d06c74e4f13cdf21195e51a63e4e`  
		Last Modified: Wed, 18 Aug 2021 00:39:17 GMT  
		Size: 14.2 MB (14236812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d960f1eae1e771eb71c2f4d25ab112792723ff85612f436cbd77feaa28a24ab0`  
		Last Modified: Wed, 18 Aug 2021 00:39:10 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4c8cf6c81b2ecffd8dd7b56c6c532b712c3978cf9b8f664ffe0af25046bcce`  
		Last Modified: Wed, 18 Aug 2021 00:39:10 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be7dcb8d904be03971456c7e0238a887d34f716245a91095008ae9840bd9115`  
		Last Modified: Wed, 18 Aug 2021 00:39:10 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119c5d6e8fb74ba2ad20888ddd80f9b31fe466ffae45554e3f3678f2ac6a85c0`  
		Last Modified: Wed, 18 Aug 2021 02:27:32 GMT  
		Size: 3.1 MB (3053429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd8f616646d61c1511056791f28ee68045daf2e583542fabc75b712e1b9122b`  
		Last Modified: Wed, 18 Aug 2021 02:27:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3679ef3da23a1fce537a7b1b082314ab72008655dc5005c4512bcb7c69ce3f78`  
		Last Modified: Wed, 18 Aug 2021 02:27:37 GMT  
		Size: 15.6 MB (15578406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeb38e803a3b7bb220860e98fdb1c1a47c072a9cc2922255c827047343abdf2`  
		Last Modified: Wed, 18 Aug 2021 02:27:31 GMT  
		Size: 303.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14816fa76d5b7738d707ad6572b35bc56c64868779ff593594d1745f38d6559`  
		Last Modified: Wed, 18 Aug 2021 02:27:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-apache` - linux; mips64le

```console
$ docker pull matomo@sha256:e474ed988fc5bcd5f14b19e2644c5f754b93ef63ff681cf608e8b97a7febfd8c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.2 MB (163210428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8cfc84cd42460b55328ec0c9feeb6087c4709599ae2f274898e2c37b5e9a0c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 17 Aug 2021 01:11:35 GMT
ADD file:4dff23dfe5a1c3cf77be5121c29de84ee66c4d10c85faa65f6122da1bfa13500 in / 
# Tue, 17 Aug 2021 01:11:36 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 21:04:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 21:04:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 21:04:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 21:04:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 21:04:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 21:17:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 17 Aug 2021 21:17:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 17 Aug 2021 21:18:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 17 Aug 2021 21:18:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 17 Aug 2021 21:18:18 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 17 Aug 2021 21:18:18 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 17 Aug 2021 21:18:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 17 Aug 2021 21:18:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 21:18:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 21:18:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Aug 2021 00:43:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 18 Aug 2021 00:43:47 GMT
ENV PHP_VERSION=7.4.22
# Wed, 18 Aug 2021 00:43:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.22.tar.xz.asc
# Wed, 18 Aug 2021 00:43:48 GMT
ENV PHP_SHA256=8e078cd7d2f49ac3fcff902490a5bb1addc885e7e3b0d8dd068f42c68297bde8
# Wed, 18 Aug 2021 00:44:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 00:44:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Aug 2021 00:51:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Aug 2021 00:51:47 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Wed, 18 Aug 2021 00:51:49 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Aug 2021 00:51:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Aug 2021 00:51:50 GMT
STOPSIGNAL SIGWINCH
# Wed, 18 Aug 2021 00:51:50 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 18 Aug 2021 00:51:50 GMT
WORKDIR /var/www/html
# Wed, 18 Aug 2021 00:51:51 GMT
EXPOSE 80
# Wed, 18 Aug 2021 00:51:51 GMT
CMD ["apache2-foreground"]
# Wed, 18 Aug 2021 13:15:34 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 18 Aug 2021 13:20:03 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 13:20:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 18 Aug 2021 13:20:05 GMT
ENV MATOMO_VERSION=4.4.1
# Wed, 18 Aug 2021 13:20:42 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 13:20:43 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 18 Aug 2021 13:20:43 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Wed, 18 Aug 2021 13:20:44 GMT
VOLUME [/var/www/html]
# Wed, 18 Aug 2021 13:20:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 13:20:44 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8375ff99ce3f614d73dc69b03575c7ebf072f4e05da52b0319fc3782d5ebb578`  
		Last Modified: Tue, 17 Aug 2021 01:20:19 GMT  
		Size: 29.6 MB (29619986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8262a73716bc8c43dd96ed353eaa7d6653e1b74527cc476cf5442c2234413f5`  
		Last Modified: Wed, 18 Aug 2021 03:32:21 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683e3b4bd71697f7de190513122c240bd01c1b5c1921be7eb1310c572bf9d081`  
		Last Modified: Wed, 18 Aug 2021 03:33:17 GMT  
		Size: 72.0 MB (72015372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f4cccd84833c8e05c27dff4f468d5dd0c173b6093c29ab18d1e86c443b2ca5`  
		Last Modified: Wed, 18 Aug 2021 03:32:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913f73a12d4e36317bd267870efdbfe1a0af8d0d712bee5247e233dcebfc3c20`  
		Last Modified: Wed, 18 Aug 2021 03:34:01 GMT  
		Size: 19.1 MB (19128742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb8ad622e9f1390c316e66b9bf2e50662245faaf32243bf1948c02180b062b6`  
		Last Modified: Wed, 18 Aug 2021 03:33:47 GMT  
		Size: 435.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e452452e959c3f5daf43604986cec8626399137f5fdb0fe338a8c2aa3d0478e`  
		Last Modified: Wed, 18 Aug 2021 03:33:47 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e306ad7fcc3d1fe4a7785493ca0b694c5c0a6a238bb613b3d588c649d66e52`  
		Last Modified: Wed, 18 Aug 2021 03:45:17 GMT  
		Size: 10.7 MB (10687073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d842b9ee9d452b91d049424d409bd6a8d51a84c5d6cf887deda99827387a6d`  
		Last Modified: Wed, 18 Aug 2021 03:45:11 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afc41c09e806de375c842137ab9be3fafc54b4b93a1f59034b0c70aa76a5739`  
		Last Modified: Wed, 18 Aug 2021 03:45:22 GMT  
		Size: 13.2 MB (13196839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6e26f6fdba4e1130ecb7a77ae39a4ed3785650766c97f250471ba7b924277d`  
		Last Modified: Wed, 18 Aug 2021 03:45:11 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ce3979599b8aaf44086a45384d8823c5a1a0b4146e3b17f7f080231b0d20c3`  
		Last Modified: Wed, 18 Aug 2021 03:45:12 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a699ee7b2ea044056a8b7ffa9ce724abe805c768397890e299bbdd43a6fc0093`  
		Last Modified: Wed, 18 Aug 2021 03:45:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79838ee977475755d7026f3c236dee921ff85d2cd30d1783e7eea392ea060df1`  
		Last Modified: Wed, 18 Aug 2021 13:26:28 GMT  
		Size: 3.0 MB (2979229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3a1ea70eb47a8eeeec11593de7103d792f91fa08f12a410122588fc045cb12`  
		Last Modified: Wed, 18 Aug 2021 13:26:25 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff6d619fbccf4359a1366c4939e03180ceb494d0e4a74f846369160e1f5391c`  
		Last Modified: Wed, 18 Aug 2021 13:26:39 GMT  
		Size: 15.6 MB (15577036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e3d724d2afa22a577b9093b159acd885866df7e948f5f96a0e652487d9c866`  
		Last Modified: Wed, 18 Aug 2021 13:26:25 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39f4bdbb41a6e77949721779ff4e8d06cd530245e6745558fb982400b7da3b8`  
		Last Modified: Wed, 18 Aug 2021 13:26:25 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-apache` - linux; ppc64le

```console
$ docker pull matomo@sha256:76340b5a90af689127643721ca8dd51771fb1045c4eb243166f4437063fda56e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.2 MB (177244719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d50b375af2e66a42d68702bfc7067d6f93564813d343fd57c6178d2bbb3f88a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:19:05 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 22 Jul 2021 12:19:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 22 Jul 2021 12:21:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:22:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Jul 2021 12:22:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Jul 2021 12:30:10 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Thu, 22 Jul 2021 12:30:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Thu, 22 Jul 2021 12:32:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Thu, 22 Jul 2021 12:32:42 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Thu, 22 Jul 2021 12:32:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Thu, 22 Jul 2021 12:32:58 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Thu, 22 Jul 2021 12:33:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Thu, 22 Jul 2021 12:33:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 12:33:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 12:33:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Jul 2021 14:30:33 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Jul 2021 23:55:15 GMT
ENV PHP_VERSION=7.4.22
# Thu, 29 Jul 2021 23:55:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.22.tar.xz.asc
# Thu, 29 Jul 2021 23:55:20 GMT
ENV PHP_SHA256=8e078cd7d2f49ac3fcff902490a5bb1addc885e7e3b0d8dd068f42c68297bde8
# Thu, 29 Jul 2021 23:56:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 29 Jul 2021 23:56:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Jul 2021 00:01:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Jul 2021 00:01:56 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 30 Jul 2021 00:02:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Jul 2021 00:02:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Jul 2021 00:02:10 GMT
STOPSIGNAL SIGWINCH
# Fri, 30 Jul 2021 00:02:11 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 30 Jul 2021 00:02:14 GMT
WORKDIR /var/www/html
# Fri, 30 Jul 2021 00:02:17 GMT
EXPOSE 80
# Fri, 30 Jul 2021 00:02:22 GMT
CMD ["apache2-foreground"]
# Fri, 30 Jul 2021 04:25:08 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 30 Jul 2021 04:27:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 30 Jul 2021 04:27:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 02 Aug 2021 21:57:21 GMT
ENV MATOMO_VERSION=4.4.1
# Mon, 02 Aug 2021 21:58:44 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Mon, 02 Aug 2021 21:58:51 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Mon, 02 Aug 2021 21:58:52 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Mon, 02 Aug 2021 21:58:54 GMT
VOLUME [/var/www/html]
# Mon, 02 Aug 2021 21:58:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 02 Aug 2021 21:58:58 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c744aca669d54986809be1e2a67eb9e2f0c23ad48ab4da67e0c595bf97a76a`  
		Last Modified: Thu, 22 Jul 2021 16:07:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69949ff352dba1d2e0826d16d0b93a1105fece06120256646f820ca4e023a19`  
		Last Modified: Thu, 22 Jul 2021 16:08:59 GMT  
		Size: 82.3 MB (82290779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d27c09515bc1d70dc3cb8a856c0db0ce76de299c9919d580eb32f61a7ea517`  
		Last Modified: Thu, 22 Jul 2021 16:07:47 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884ffb9dee9d233677c4afa7cb1496169fa44e71d2a70f415e43eadd584ed49d`  
		Last Modified: Thu, 22 Jul 2021 16:09:54 GMT  
		Size: 19.8 MB (19818437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9b1c84d470f3cfc4ab9e253cfb3be6a0c76557d11e98658835e703c9f9e879`  
		Last Modified: Thu, 22 Jul 2021 16:09:49 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb570758ef2a62add994aa1b2640d417d903c0d8bcc489f347a9157ab906df1a`  
		Last Modified: Thu, 22 Jul 2021 16:09:47 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d0d7dbc8fce9dfee0e3adf08621039f5e847f339c9628bebae409b05496545b`  
		Last Modified: Fri, 30 Jul 2021 01:08:22 GMT  
		Size: 10.7 MB (10686634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef335160e8381e12e047fd326f7d28c38c81e471264b940642c73ba169b9bcbe`  
		Last Modified: Fri, 30 Jul 2021 01:08:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aae1751681b7e83fa17865e272313c90e0e1bbc9aea5ec89db176cdd7c95049`  
		Last Modified: Fri, 30 Jul 2021 01:08:18 GMT  
		Size: 14.9 MB (14882432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ee72b35ea5c3170f73ecc37feac7e95b73c1300d4622ecd94bdcc27b16068a`  
		Last Modified: Fri, 30 Jul 2021 01:08:14 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea40b73d0bfff97b3ecd95a4bca3ac1fd01de7a9e1a5417e1f0df9f989620cb`  
		Last Modified: Fri, 30 Jul 2021 01:08:14 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587868979b89dd326d143582f3b251cb39dce356259b92ad7f32ebd564715511`  
		Last Modified: Fri, 30 Jul 2021 01:08:14 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e7e87696bb3ed5434e11ce5d2aae0f23357819af3fec65ab4ec02a7743aa0d`  
		Last Modified: Fri, 30 Jul 2021 04:36:36 GMT  
		Size: 3.4 MB (3431634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1653830a5c24cd19e944ee7553316df691b5360428c4f2c213f799f09cba317`  
		Last Modified: Fri, 30 Jul 2021 04:36:35 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e4d58ec98a5d3b647054286187ea8cfa32d15107c136fb6da2a1ec3ad0961a`  
		Last Modified: Mon, 02 Aug 2021 22:02:50 GMT  
		Size: 15.6 MB (15574836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c97a76c0abb8ac3c12d4a2f2353e22430e9129031d4473e84cc68ee1aaaa777`  
		Last Modified: Mon, 02 Aug 2021 22:02:46 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d736d353d34f2f9cd11c711cdab1ca9b278406cb856c06edfd27c500230554`  
		Last Modified: Mon, 02 Aug 2021 22:02:46 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-apache` - linux; s390x

```console
$ docker pull matomo@sha256:9340883abe17836ee0112f9bea3fd7abdf8c95df4170b076225a73d6f914dc82
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.7 MB (162692125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0c0b96797892a2239a5cffa18de5e027d1be2e1be4e38afadd4c150c3a18eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:02 GMT
ADD file:9a849f976712983c3bf95c9d110ab1c38643273c19644a436242e8b8bd5eb225 in / 
# Tue, 17 Aug 2021 01:49:07 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 23:52:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 17 Aug 2021 23:52:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 17 Aug 2021 23:52:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 23:52:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 17 Aug 2021 23:52:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 17 Aug 2021 23:56:16 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 17 Aug 2021 23:56:16 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 17 Aug 2021 23:56:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 17 Aug 2021 23:56:29 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 17 Aug 2021 23:56:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 17 Aug 2021 23:56:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 17 Aug 2021 23:56:30 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 17 Aug 2021 23:56:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 23:56:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 17 Aug 2021 23:56:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 18 Aug 2021 00:31:15 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 18 Aug 2021 00:31:16 GMT
ENV PHP_VERSION=7.4.22
# Wed, 18 Aug 2021 00:31:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.22.tar.xz.asc
# Wed, 18 Aug 2021 00:31:16 GMT
ENV PHP_SHA256=8e078cd7d2f49ac3fcff902490a5bb1addc885e7e3b0d8dd068f42c68297bde8
# Wed, 18 Aug 2021 00:31:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 00:31:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 18 Aug 2021 00:33:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 18 Aug 2021 00:33:24 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Wed, 18 Aug 2021 00:33:25 GMT
RUN docker-php-ext-enable sodium
# Wed, 18 Aug 2021 00:33:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 18 Aug 2021 00:33:25 GMT
STOPSIGNAL SIGWINCH
# Wed, 18 Aug 2021 00:33:25 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 18 Aug 2021 00:33:26 GMT
WORKDIR /var/www/html
# Wed, 18 Aug 2021 00:33:26 GMT
EXPOSE 80
# Wed, 18 Aug 2021 00:33:26 GMT
CMD ["apache2-foreground"]
# Wed, 18 Aug 2021 04:52:36 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 18 Aug 2021 04:53:40 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.20; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 04:53:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 18 Aug 2021 04:53:41 GMT
ENV MATOMO_VERSION=4.4.1
# Wed, 18 Aug 2021 04:53:56 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 04:53:58 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 18 Aug 2021 04:53:58 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Wed, 18 Aug 2021 04:53:58 GMT
VOLUME [/var/www/html]
# Wed, 18 Aug 2021 04:53:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 04:53:59 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:16c136b299a1426955abff4eb0ed556e3c2e8e67509fba84e416f1d5cc77189a`  
		Last Modified: Tue, 17 Aug 2021 01:57:33 GMT  
		Size: 29.6 MB (29647028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95186f11f9aca8af9be912823712ea541f8e6e600b179d3616d3be6b93736e00`  
		Last Modified: Wed, 18 Aug 2021 01:12:00 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a7d93dc02b570d50d80a1aa8b5124a704cb208cb9699b826113438de812870`  
		Last Modified: Wed, 18 Aug 2021 01:12:10 GMT  
		Size: 71.6 MB (71622148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ff946dfc28cc308722046900124caf233323b72bd2783f5b71846a58df3086`  
		Last Modified: Wed, 18 Aug 2021 01:12:01 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf34bdb15c8951c94f3f8be0067bcaed627581e63859f048a815d7579862fe7`  
		Last Modified: Wed, 18 Aug 2021 01:12:35 GMT  
		Size: 19.0 MB (19026307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f21256bcd2a7aa22771523fa8564c09ddcc2e7af08a2cce08745b5ced7860c9`  
		Last Modified: Wed, 18 Aug 2021 01:12:32 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c56103e88f74dc68c3230aa6e167b39fe42d1cdbdedb212633bfe002c6df42`  
		Last Modified: Wed, 18 Aug 2021 01:12:32 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ac5e5b360ce20c0a6c3ae7ad5b9af0d375c95d9ab438c8203c1fdd2193fc76`  
		Last Modified: Wed, 18 Aug 2021 01:16:29 GMT  
		Size: 10.7 MB (10687914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2dddd6a56a253c1f2f60eebf44826d0e3db8d37a1ad7f218251fe7d0be36e2`  
		Last Modified: Wed, 18 Aug 2021 01:16:27 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe25f5e3bedbed85fa8631f3ed1d760e01d93d29cf12807518c69e3e7f186a`  
		Last Modified: Wed, 18 Aug 2021 01:16:29 GMT  
		Size: 13.1 MB (13133803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e679828140afb83da616fe0e98efc731676e88e637f914bf0ddf33c607657f7`  
		Last Modified: Wed, 18 Aug 2021 01:16:27 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d565c9334e62fc0289fd1394bdfbb01aaa1c092354346e6f82ce81183e2a4a8c`  
		Last Modified: Wed, 18 Aug 2021 01:16:27 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978abad99f13d0f02abb5b758e4d7b1cfcb95e470cfd51dfc9176a5b462b9cbe`  
		Last Modified: Wed, 18 Aug 2021 01:16:27 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9eb235cd352785575b6ccdaa308a1bb53526266c483215126bbd08211f4f48`  
		Last Modified: Wed, 18 Aug 2021 04:56:36 GMT  
		Size: 3.0 MB (2990803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c747c72504e688cbdf5bd9c41ec2cf3f7319725fa7b414908f0210afa8a019c7`  
		Last Modified: Wed, 18 Aug 2021 04:56:35 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36412e070394aca1429b07698f63815a0248b320d6bfa42f179e8a93f2654ec2`  
		Last Modified: Wed, 18 Aug 2021 04:56:38 GMT  
		Size: 15.6 MB (15577871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2ed7ecbb52f7f304454c44cb94d8738bd1151c7357d764c6f57c000deff615`  
		Last Modified: Wed, 18 Aug 2021 04:56:35 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6da4bc610a5acf20eeb87d013cfca7682e7b89958ee6f821370ecc5a6b5f817`  
		Last Modified: Wed, 18 Aug 2021 04:56:35 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
