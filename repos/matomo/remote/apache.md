## `matomo:apache`

```console
$ docker pull matomo@sha256:34f3460fb3eb5608901534abcb67ff446c393b0c4cf982a95caccf73d8121637
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

### `matomo:apache` - linux; amd64

```console
$ docker pull matomo@sha256:6bc9105a61c7a190c904f3db1711a2dda3f255a5785d87ad286fb3eb9dd3fe17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.6 MB (184621168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:259930c55d2a301d8a27d67b83c6cca7a46ba3c088a0184a3c98b828e2018be2`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Wed, 11 May 2022 13:27:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 12 May 2022 20:01:36 GMT
ENV PHP_VERSION=8.0.19
# Thu, 12 May 2022 20:01:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Thu, 12 May 2022 20:01:37 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Thu, 12 May 2022 20:01:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 May 2022 20:01:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 May 2022 20:04:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 May 2022 20:04:51 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 May 2022 20:04:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 May 2022 20:04:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 May 2022 20:04:52 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 May 2022 20:04:52 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 May 2022 20:04:52 GMT
WORKDIR /var/www/html
# Thu, 12 May 2022 20:04:52 GMT
EXPOSE 80
# Thu, 12 May 2022 20:04:52 GMT
CMD ["apache2-foreground"]
# Thu, 12 May 2022 21:45:15 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 12 May 2022 21:45:15 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 12 May 2022 21:46:46 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 		procps 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 21:46:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 17 May 2022 22:19:41 GMT
ENV MATOMO_VERSION=4.10.0
# Tue, 17 May 2022 22:19:55 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys F529A27008477483777FC23D63BB30D0E5D2C749; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 May 2022 22:19:56 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Tue, 17 May 2022 22:19:56 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Tue, 17 May 2022 22:19:56 GMT
VOLUME [/var/www/html]
# Tue, 17 May 2022 22:19:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 May 2022 22:19:56 GMT
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
	-	`sha256:af45e7153a31404d654ff2c2bd7f670b0f0dd373a71777f6bae6aabababbd127`  
		Last Modified: Thu, 12 May 2022 20:54:01 GMT  
		Size: 11.1 MB (11118855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b546fbaf263bc4603fcf4a3cf5c2129492ab03d6166cc4c0528043a537ea2224`  
		Last Modified: Thu, 12 May 2022 20:53:57 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16dd2cabbcd262c843c9cf409f9dc56eb5df84b71eb9830c3435a77c90af48d6`  
		Last Modified: Thu, 12 May 2022 20:53:59 GMT  
		Size: 10.8 MB (10774053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a426b492806becf5bf4320743c6e4d127a906569cd19a8577327aea4e4c246`  
		Last Modified: Thu, 12 May 2022 20:53:57 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94e73d5f13e6936d12c75a6962e2e0bb435dd637efc61210bba75cef2ad3ac8`  
		Last Modified: Thu, 12 May 2022 20:53:57 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5a3464a278bbc7ee8d4b8cb3018db28fbf1c7e8bdb5a9a2fd68ac82e08e148`  
		Last Modified: Thu, 12 May 2022 20:53:57 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b383928d53b3fc9abd70db1786f58c08c4011f8ec093468f5588a5cb7743aede`  
		Last Modified: Thu, 12 May 2022 21:51:29 GMT  
		Size: 3.4 MB (3358330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa9c153bd21d58fc857202b97724bda31af9116d2a96ef5d918096501baef8d`  
		Last Modified: Thu, 12 May 2022 21:51:28 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c15a8f8a10abe0488734be65b0c6fe2b4751063e8fab567ececbd13f95f0a52`  
		Last Modified: Tue, 17 May 2022 22:20:55 GMT  
		Size: 17.1 MB (17133190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da586f0cc9de2f664c957671df5dc25f47f389ac88c420cfcc55bb10847fa108`  
		Last Modified: Tue, 17 May 2022 22:20:51 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a00879cafeda39e78836a50d2bfd71826f9f297701535d53c500712e9576068`  
		Last Modified: Tue, 17 May 2022 22:20:51 GMT  
		Size: 628.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:apache` - linux; arm variant v5

```console
$ docker pull matomo@sha256:2a86b0d681d6a2d2019913711284fd397b3c4dae36e274f13f3ab32d903a0468
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.8 MB (161798323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e58c3695736309842795e440cfdce81a5f8c90828e6b90d08f9fd9b19f4d878a`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Wed, 11 May 2022 10:39:33 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 12 May 2022 18:59:15 GMT
ENV PHP_VERSION=8.0.19
# Thu, 12 May 2022 18:59:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Thu, 12 May 2022 18:59:16 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Thu, 12 May 2022 18:59:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 May 2022 18:59:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 May 2022 19:06:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 May 2022 19:06:12 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 May 2022 19:06:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 May 2022 19:06:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 May 2022 19:06:15 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 May 2022 19:06:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 May 2022 19:06:16 GMT
WORKDIR /var/www/html
# Thu, 12 May 2022 19:06:16 GMT
EXPOSE 80
# Thu, 12 May 2022 19:06:17 GMT
CMD ["apache2-foreground"]
# Thu, 12 May 2022 20:30:26 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 12 May 2022 20:30:26 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 12 May 2022 20:34:11 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 		procps 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 20:34:12 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 20:34:13 GMT
ENV MATOMO_VERSION=4.9.1
# Thu, 12 May 2022 20:35:05 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys F529A27008477483777FC23D63BB30D0E5D2C749; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 20:35:07 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 12 May 2022 20:35:07 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Thu, 12 May 2022 20:35:07 GMT
VOLUME [/var/www/html]
# Thu, 12 May 2022 20:35:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 May 2022 20:35:08 GMT
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
	-	`sha256:2a8446fac83f811f52668e3e56f99767a9d0dbe8e694eec6c97896a0bc8d33ea`  
		Last Modified: Thu, 12 May 2022 19:55:56 GMT  
		Size: 11.1 MB (11117599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a308651481ac207456e38aae01c89a114c038892cd83e7746a57cd8e0d24aee`  
		Last Modified: Thu, 12 May 2022 19:55:51 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e545b099358eb75f5279ea5254e8f89cad9b130963607829ce4a18144caa77de`  
		Last Modified: Thu, 12 May 2022 19:55:59 GMT  
		Size: 9.8 MB (9789558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92bf96e1a8446adb084477af1b09568fcba745e9e5469042d02b18316e408be`  
		Last Modified: Thu, 12 May 2022 19:55:51 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1cbe0da93228bd41858adbf379018a962c4f087c1d78f15bd2ae8036334fc6`  
		Last Modified: Thu, 12 May 2022 19:55:51 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b3eddd3abe92450aafa12936c54d7567dccf1e9ccc6eb17483b50a18c371f9`  
		Last Modified: Thu, 12 May 2022 19:55:51 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b161591f9f02e20714083963616b64a19e0c1e491263a47da9ab98bd8d9afa`  
		Last Modified: Thu, 12 May 2022 20:41:16 GMT  
		Size: 2.8 MB (2832736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f66c539288a52745b535b314ebc6c4d83d631034a91bec0aff7b797907916cd0`  
		Last Modified: Thu, 12 May 2022 20:41:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87557b1a96f5bfd55df21003a6ee94f2390f7a18e3b4d15fc90e939a44815b2c`  
		Last Modified: Thu, 12 May 2022 20:41:32 GMT  
		Size: 16.9 MB (16900656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b0fe0f1fe6ab4d51bd6a2028dae194eed8dff623eda90015b4e4854508e7a5`  
		Last Modified: Thu, 12 May 2022 20:41:14 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47587d9e0cd830554c9c8f97629cba65b36aef526adebcc11efebb42da2d085`  
		Last Modified: Thu, 12 May 2022 20:41:14 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:apache` - linux; arm variant v7

```console
$ docker pull matomo@sha256:5e4f524a82439cb6d4b6a09205c99a6db26ef5de638720fe83965fb329ef23d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.1 MB (154129297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a980de7854ad41686dde83780263a1755c9ef49a3ae3b1e1cd7661cb7413436b`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Wed, 11 May 2022 15:08:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 13 May 2022 06:19:38 GMT
ENV PHP_VERSION=8.0.19
# Fri, 13 May 2022 06:19:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Fri, 13 May 2022 06:19:39 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Fri, 13 May 2022 06:19:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 13 May 2022 06:20:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 06:24:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 06:24:34 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 13 May 2022 06:24:35 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 06:24:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 06:24:36 GMT
STOPSIGNAL SIGWINCH
# Fri, 13 May 2022 06:24:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 13 May 2022 06:24:37 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 06:24:38 GMT
EXPOSE 80
# Fri, 13 May 2022 06:24:38 GMT
CMD ["apache2-foreground"]
# Fri, 13 May 2022 10:51:04 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 13 May 2022 10:51:05 GMT
ENV PHP_MEMORY_LIMIT=256M
# Fri, 13 May 2022 10:54:44 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 		procps 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 May 2022 10:54:46 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 17 May 2022 21:57:59 GMT
ENV MATOMO_VERSION=4.10.0
# Tue, 17 May 2022 21:59:06 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys F529A27008477483777FC23D63BB30D0E5D2C749; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 May 2022 21:59:07 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Tue, 17 May 2022 21:59:07 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Tue, 17 May 2022 21:59:08 GMT
VOLUME [/var/www/html]
# Tue, 17 May 2022 21:59:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 May 2022 21:59:09 GMT
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
	-	`sha256:4b463811295cc95c7d1cbdee76749d0a8659cb34f876b76aa087e324688d9fcf`  
		Last Modified: Fri, 13 May 2022 07:49:42 GMT  
		Size: 11.1 MB (11117617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94573c9b314e299743785bd3768251642556f19b59eb070214daaeff3c76e481`  
		Last Modified: Fri, 13 May 2022 07:49:38 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88915bcdb878aa96361565e64ce31be19a7b0f216f0cccef233e8de33c1737e8`  
		Last Modified: Fri, 13 May 2022 07:49:45 GMT  
		Size: 9.3 MB (9305836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d1981f3e101db28231c136a645cfbf42a07ac3fedcf350686ba5204acd0ea9`  
		Last Modified: Fri, 13 May 2022 07:49:38 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e2cf5967a668a6687dec1107d1c3bbccedd24899a7efffaa1a22a6c561f83`  
		Last Modified: Fri, 13 May 2022 07:49:38 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02582bb657ea6e2972516bd05e75f33a98acd136e8cea4bbf06c30bdb3af81e5`  
		Last Modified: Fri, 13 May 2022 07:49:38 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d3868534cc2f5d8114be932e706315d3e39caffe1488386bbb1584785849b1`  
		Last Modified: Fri, 13 May 2022 11:06:54 GMT  
		Size: 2.7 MB (2681070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14542b75c868111bb3c37d3f69101d5848349f7bbc17c90d7c4716d089b6ad7a`  
		Last Modified: Fri, 13 May 2022 11:06:52 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9ab35ff9ccf1e390365ac7b45d7038b9e41663ce56cee9b5c2f8d5606b874b`  
		Last Modified: Tue, 17 May 2022 22:03:05 GMT  
		Size: 17.1 MB (17131853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c750eaa41526adb9cd03b9c47cf8e448f8735d85395bc0425c87dae26a29cf`  
		Last Modified: Tue, 17 May 2022 22:02:47 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b179ed9b335c1e6468dc0dd1fc6f4569b40683b448f7ff2b284f3a284a9fdb`  
		Last Modified: Tue, 17 May 2022 22:02:47 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:apache` - linux; arm64 variant v8

```console
$ docker pull matomo@sha256:617c752a46a2a330a23b97ce40be72044b2c1b553a881e93f0a4fc85c45715e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176311098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cede6f2566aa1bdde19b93bf2177dc481912b000d3d34fe69837fe9e18cf1505`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Wed, 11 May 2022 06:20:33 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 12 May 2022 20:37:25 GMT
ENV PHP_VERSION=8.0.19
# Thu, 12 May 2022 20:37:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Thu, 12 May 2022 20:37:26 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Thu, 12 May 2022 20:37:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 May 2022 20:37:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 May 2022 20:40:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 May 2022 20:40:09 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 May 2022 20:40:09 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 May 2022 20:40:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 May 2022 20:40:11 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 May 2022 20:40:13 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 May 2022 20:40:13 GMT
WORKDIR /var/www/html
# Thu, 12 May 2022 20:40:14 GMT
EXPOSE 80
# Thu, 12 May 2022 20:40:15 GMT
CMD ["apache2-foreground"]
# Thu, 12 May 2022 23:20:23 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 12 May 2022 23:20:24 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 12 May 2022 23:21:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 		procps 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 23:21:43 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 23:21:43 GMT
ENV MATOMO_VERSION=4.9.1
# Thu, 12 May 2022 23:22:14 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys F529A27008477483777FC23D63BB30D0E5D2C749; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 23:22:16 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 12 May 2022 23:22:17 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Thu, 12 May 2022 23:22:17 GMT
VOLUME [/var/www/html]
# Thu, 12 May 2022 23:22:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 May 2022 23:22:19 GMT
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
	-	`sha256:b7d5bb53ab81a84a3da570fea9d7e612a8720f8f3592952d925950a9b3c2eefb`  
		Last Modified: Thu, 12 May 2022 21:57:41 GMT  
		Size: 10.9 MB (10902670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e746251e9b3cc416dbbe582632e11a49a4c5692d456b4f70cbe6431014d404b`  
		Last Modified: Thu, 12 May 2022 21:57:38 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381961d92b927da49f3e3de321a95988aa01019e044afb85765c7fe09d85b7c5`  
		Last Modified: Thu, 12 May 2022 21:57:40 GMT  
		Size: 10.2 MB (10229984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7688d05d9696481aee7be57bfb147091b80d6d21224cfd0031389156e9a62b5c`  
		Last Modified: Thu, 12 May 2022 21:57:38 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014e86f9b1339368bde85437a24f79f0444b9ad4112ecd12f920c5259c3c1009`  
		Last Modified: Thu, 12 May 2022 21:57:38 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723eb1e68bb5706ea851f801b0cf57976fa4f74c0eeb6f2686ead442c4a09743`  
		Last Modified: Thu, 12 May 2022 21:57:38 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a95cafa0a81a13962495bb2b6ae9b15c77ed428d664e4bbbb7b11a13dc4410`  
		Last Modified: Thu, 12 May 2022 23:27:46 GMT  
		Size: 2.8 MB (2760256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689bf5ef913eee091cb5dd84847b0af0cafd4161c7afbec997b06368c334752b`  
		Last Modified: Thu, 12 May 2022 23:27:45 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca4abb93f1d342fe64cd6a07c9aef680a0e43096c6d06aa30163414d12e5a06`  
		Last Modified: Thu, 12 May 2022 23:27:49 GMT  
		Size: 16.7 MB (16684817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1050982a4377efb42d662400b17caaa28967ee0bdf67c0d98ea019cbdfbd36af`  
		Last Modified: Thu, 12 May 2022 23:27:45 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2177038fa408c9b48066efa68e3ea91ff96aff00ebce2f5fe862d5e0e7b8db31`  
		Last Modified: Thu, 12 May 2022 23:27:45 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:apache` - linux; 386

```console
$ docker pull matomo@sha256:51884c4cf1fbc9e6e51eee622ff4d0b7329472f69cc3f417d90c901da3cbbfbd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.1 MB (186106779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa6daae44ac6ff4ecbb6d2f18e5e41bdfa685998033d201689ce9549861b6a12`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Wed, 11 May 2022 08:07:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 12 May 2022 20:29:15 GMT
ENV PHP_VERSION=8.0.19
# Thu, 12 May 2022 20:29:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Thu, 12 May 2022 20:29:17 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Thu, 12 May 2022 20:29:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 May 2022 20:29:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 May 2022 20:32:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 May 2022 20:32:16 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 May 2022 20:32:16 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 May 2022 20:32:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 May 2022 20:32:18 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 May 2022 20:32:20 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 May 2022 20:32:20 GMT
WORKDIR /var/www/html
# Thu, 12 May 2022 20:32:21 GMT
EXPOSE 80
# Thu, 12 May 2022 20:32:22 GMT
CMD ["apache2-foreground"]
# Thu, 12 May 2022 21:59:39 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 12 May 2022 21:59:40 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 12 May 2022 22:01:05 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 		procps 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 22:01:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 22:01:06 GMT
ENV MATOMO_VERSION=4.9.1
# Thu, 12 May 2022 22:01:36 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys F529A27008477483777FC23D63BB30D0E5D2C749; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 22:01:38 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 12 May 2022 22:01:39 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Thu, 12 May 2022 22:01:39 GMT
VOLUME [/var/www/html]
# Thu, 12 May 2022 22:01:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 May 2022 22:01:41 GMT
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
	-	`sha256:0cfe9631f32500eef49c95ff02ecb8fbb7914a5dfa534e29b407568c6e037d71`  
		Last Modified: Thu, 12 May 2022 21:25:17 GMT  
		Size: 10.9 MB (10902681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e1ff1469b720e25f4d7694d232d10a704a99f84c4b9532057f611e9083df85`  
		Last Modified: Thu, 12 May 2022 21:25:13 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6133546e3409db1ca7093500fbb921f96208ad6c17f011cd89b279fdd8d160bc`  
		Last Modified: Thu, 12 May 2022 21:25:15 GMT  
		Size: 11.0 MB (10978340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6390c7aea96ffb2b488aa0b69912344e5ba581bdf157e2e18c002288d173b6`  
		Last Modified: Thu, 12 May 2022 21:25:13 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027b69538f419c3b92533e75892ecee7437a114b1a14c5b14a2462fabe3f429f`  
		Last Modified: Thu, 12 May 2022 21:25:13 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb599dbe95d2e39a89beb1bcf6a25cb789d35a29b43a9b93f32ef441f88d60ba`  
		Last Modified: Thu, 12 May 2022 21:25:14 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a277c509d90bf6da5eee80f3c09d11143b0b11333b347ea5325e30ad2b57d1`  
		Last Modified: Thu, 12 May 2022 22:07:07 GMT  
		Size: 3.1 MB (3131838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310055d9ed0bfa654a30a480ac01a898f4dc8e52eba3cfdb809d23a54da1d240`  
		Last Modified: Thu, 12 May 2022 22:07:07 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d0e250b59389e3730387663a5f326961948163ff1619da338156d81e72c141`  
		Last Modified: Thu, 12 May 2022 22:07:10 GMT  
		Size: 16.7 MB (16684849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d077740fb620c9f32af0a5ff944cd19f7e85ca61ec70d85dc8f9934b31cfe6c7`  
		Last Modified: Thu, 12 May 2022 22:07:07 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535113f2a80ce6c857185c4e438c383763e137bf9175064b6146ffd42c489a3d`  
		Last Modified: Thu, 12 May 2022 22:07:07 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:apache` - linux; mips64le

```console
$ docker pull matomo@sha256:fe8f824e6624d5ae78b1afe29f4462511bb99c02d3baec50539459eeb94d89d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.9 MB (160882127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71e838561f6f032b7a6c5a8c2016e3378eddcb2a293401808706d61e7c4b2247`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 May 2022 02:23:35 GMT
ADD file:d47dce2adbc9352ef1d437730bab3b579dd8d2bf29dd60cd8a8b65396b39e36e in / 
# Wed, 11 May 2022 02:23:40 GMT
CMD ["bash"]
# Wed, 11 May 2022 13:59:07 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 13:59:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 14:00:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:00:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 14:00:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 14:15:16 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 May 2022 14:15:20 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 May 2022 14:16:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 May 2022 14:16:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 May 2022 14:16:27 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 May 2022 14:16:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 14:16:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 14:16:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 18:04:26 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 13 May 2022 08:44:42 GMT
ENV PHP_VERSION=8.0.19
# Fri, 13 May 2022 08:44:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Fri, 13 May 2022 08:44:49 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Fri, 13 May 2022 08:45:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 13 May 2022 08:45:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 08:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 08:59:15 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 13 May 2022 08:59:22 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 08:59:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 08:59:30 GMT
STOPSIGNAL SIGWINCH
# Fri, 13 May 2022 08:59:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 13 May 2022 08:59:36 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 08:59:40 GMT
EXPOSE 80
# Fri, 13 May 2022 08:59:44 GMT
CMD ["apache2-foreground"]
# Fri, 13 May 2022 13:27:45 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 13 May 2022 13:27:48 GMT
ENV PHP_MEMORY_LIMIT=256M
# Fri, 13 May 2022 13:32:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 		procps 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 May 2022 13:32:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 17 May 2022 22:07:54 GMT
ENV MATOMO_VERSION=4.10.0
# Tue, 17 May 2022 22:08:56 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys F529A27008477483777FC23D63BB30D0E5D2C749; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 May 2022 22:09:03 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Tue, 17 May 2022 22:09:07 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Tue, 17 May 2022 22:09:13 GMT
VOLUME [/var/www/html]
# Tue, 17 May 2022 22:09:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 17 May 2022 22:09:24 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:438a36bf0b6e75ff6f0fbb2b7669dfb86361416f4d808912d30cf5b91ad2eea9`  
		Last Modified: Wed, 11 May 2022 02:33:43 GMT  
		Size: 29.6 MB (29641051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af72c70f4c7609bdf33b81257f7cc1437a3ba6d23a3c9f60b583c2cd826a01a`  
		Last Modified: Wed, 11 May 2022 22:55:31 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a5f8d31267ed1e4ed0ce8d2d9e169cd418ccbdd5ec7785d1a3385960515fc7`  
		Last Modified: Wed, 11 May 2022 22:56:23 GMT  
		Size: 71.8 MB (71810215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8173bf73bc545d79bb26e83b5b8bab54ea33f27d8ec70d76f0702e082d24dbd`  
		Last Modified: Wed, 11 May 2022 22:55:30 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d542a3a40e316e167de3a706cb480c87816f284c3b2f8d326479af54351ece`  
		Last Modified: Wed, 11 May 2022 22:57:04 GMT  
		Size: 18.9 MB (18933439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a65d94876db9c8d5aaf8a09e51c80d98628dc7fb3cd4ffdfc92efd5ef03411`  
		Last Modified: Wed, 11 May 2022 22:56:52 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78723fab34286cdbe901d4f5246920bdb2503fc5f809d958b30316fb8851a754`  
		Last Modified: Wed, 11 May 2022 22:56:53 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8806e56ef4ce3e354405e10de18307eeb5619758d53f5e0145b8bc8faec7f324`  
		Last Modified: Fri, 13 May 2022 10:25:55 GMT  
		Size: 10.9 MB (10901385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca950c5f5c07abac0bdd551f8ce16a7da354679214a9faa9706c12b0f7bd420c`  
		Last Modified: Fri, 13 May 2022 10:25:50 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531c525d107e5abddadb1c312b31594345b6777dbb0579ac5e2175ec23364d53`  
		Last Modified: Fri, 13 May 2022 10:25:57 GMT  
		Size: 9.9 MB (9917149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0539ceaca86ef5884a67449252de26cb08da9d456b2ddc7f7004563e38329e75`  
		Last Modified: Fri, 13 May 2022 10:25:50 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588a19c43bec3c86a359e80a920ab45681255f6611592806b7d1017ac2cc4c7f`  
		Last Modified: Fri, 13 May 2022 10:25:49 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67548f07dc797146c382ab4644336d5c9e3e56a13a9987cfe7b440ed023c38ed`  
		Last Modified: Fri, 13 May 2022 10:25:50 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f15bb6bb723ed7de08c39a12f3ae4654505930b99c9d4bf5ea9e2332a8a0a6`  
		Last Modified: Fri, 13 May 2022 13:42:17 GMT  
		Size: 2.8 MB (2759138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f858f983f9a8cc9a6afb316554802deb424afab04139d072f8d1e2859b5fa1`  
		Last Modified: Fri, 13 May 2022 13:42:15 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6612774e0c92f70a6ecb8ab9b58a5d3fd803479419f2a17f27316ff281ce423e`  
		Last Modified: Tue, 17 May 2022 22:11:52 GMT  
		Size: 16.9 MB (16912971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326c2b0e8af8b53e73222a9e217e37e3c907985c414d28d56d9cad105804df9f`  
		Last Modified: Tue, 17 May 2022 22:11:38 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79038e6be368398c98a586646fcc3b55a6d755ee2c8604e078fc947b0737a8b`  
		Last Modified: Tue, 17 May 2022 22:11:38 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:apache` - linux; ppc64le

```console
$ docker pull matomo@sha256:fc7a7621c0c81de80a4b30d3011891dd93e43e07f90ffa7c88fce69681a233f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **184.8 MB (184809522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2382780840e4282794779f0763b5a69bf6eeaba793fd9ffa3feb2f1953f046fa`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Wed, 11 May 2022 17:41:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 13 May 2022 01:21:21 GMT
ENV PHP_VERSION=8.0.19
# Fri, 13 May 2022 01:21:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Fri, 13 May 2022 01:21:25 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Fri, 13 May 2022 01:22:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 13 May 2022 01:22:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 01:33:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 01:33:35 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 13 May 2022 01:33:47 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 01:34:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 01:34:09 GMT
STOPSIGNAL SIGWINCH
# Fri, 13 May 2022 01:34:12 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 13 May 2022 01:34:16 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 01:34:21 GMT
EXPOSE 80
# Fri, 13 May 2022 01:34:25 GMT
CMD ["apache2-foreground"]
# Fri, 13 May 2022 10:04:10 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 13 May 2022 10:04:13 GMT
ENV PHP_MEMORY_LIMIT=256M
# Fri, 13 May 2022 10:07:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 		procps 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 May 2022 10:07:43 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 13 May 2022 10:07:47 GMT
ENV MATOMO_VERSION=4.9.1
# Fri, 13 May 2022 10:08:44 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys F529A27008477483777FC23D63BB30D0E5D2C749; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 May 2022 10:08:48 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 13 May 2022 10:08:49 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Fri, 13 May 2022 10:08:52 GMT
VOLUME [/var/www/html]
# Fri, 13 May 2022 10:08:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 13 May 2022 10:09:01 GMT
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
	-	`sha256:c4c9e4339efc65976b15d06af28c648e9227a31b5b33958b4959a197337a9fdd`  
		Last Modified: Fri, 13 May 2022 03:21:09 GMT  
		Size: 11.1 MB (11119075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322cf44a2fb26ceff036d6d6d042789f35bd88b7365d3d14ee09fa68cff79fe7`  
		Last Modified: Fri, 13 May 2022 03:21:05 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e56238719c8f31780b2919660a25945f3491fc19528e66169b43dd1af99c573`  
		Last Modified: Fri, 13 May 2022 03:21:07 GMT  
		Size: 11.1 MB (11137294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1266e809a15304ad628b69a4dd72e3baddb91b5877930715b709823e60209d57`  
		Last Modified: Fri, 13 May 2022 03:21:05 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb90d75516914f148a894f1ace29f3413f906d708f83988ccf6dc4faa51155`  
		Last Modified: Fri, 13 May 2022 03:21:05 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00adbe0005ae07c9b35a63d8f590d1ce0a3c1ceb4086145f7c93b6cc362950`  
		Last Modified: Fri, 13 May 2022 03:21:05 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5532d464fffeaf545e4d635b61000dc82719ed21ed43033c3f4ef4ca83b84e`  
		Last Modified: Fri, 13 May 2022 10:22:54 GMT  
		Size: 3.3 MB (3276266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe23d4be76397c07ff0c781b2c7f7ff1e81bce8a7500474c6a6d65ae2201f75`  
		Last Modified: Fri, 13 May 2022 10:22:53 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f5ba27ec86e07dcd09f89d5df6aaed144b0390c07bddfac9f137f8fb205ced`  
		Last Modified: Fri, 13 May 2022 10:22:57 GMT  
		Size: 16.9 MB (16903221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f6d20d69d5fafd4c2c9e33eaeac23072b3982523ff6f8deadb154d514a4d8d`  
		Last Modified: Fri, 13 May 2022 10:22:53 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3a7cb108e2a22208f5401d82497c29b89810f8f54b89dca99ed688b8b6afb0`  
		Last Modified: Fri, 13 May 2022 10:22:53 GMT  
		Size: 633.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:apache` - linux; s390x

```console
$ docker pull matomo@sha256:8c76deb5a2e631d7f69b87cbf2e05e728a44520f5cf5e3599ee8112076738765
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.3 MB (161261356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102f7c78a09a3aa65d5baca635e6f55ffc7833f4dafe18018cdbd92efe01806e`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Wed, 11 May 2022 09:46:40 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 12 May 2022 20:26:37 GMT
ENV PHP_VERSION=8.0.19
# Thu, 12 May 2022 20:26:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.19.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.19.tar.xz.asc
# Thu, 12 May 2022 20:26:37 GMT
ENV PHP_SHA256=ba62219c4b0486cbb2a04f0796749a46b0ee1f5a142ed454212b4e2460cb0fab
# Thu, 12 May 2022 20:26:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 May 2022 20:26:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 May 2022 20:28:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 May 2022 20:28:42 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 May 2022 20:28:42 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 May 2022 20:28:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 May 2022 20:28:42 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 May 2022 20:28:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 May 2022 20:28:43 GMT
WORKDIR /var/www/html
# Thu, 12 May 2022 20:28:43 GMT
EXPOSE 80
# Thu, 12 May 2022 20:28:43 GMT
CMD ["apache2-foreground"]
# Thu, 12 May 2022 22:14:52 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 12 May 2022 22:14:53 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 12 May 2022 22:17:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 		procps 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.6; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 22:17:50 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 22:17:50 GMT
ENV MATOMO_VERSION=4.9.1
# Thu, 12 May 2022 22:18:19 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys F529A27008477483777FC23D63BB30D0E5D2C749; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 22:18:23 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 12 May 2022 22:18:24 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Thu, 12 May 2022 22:18:24 GMT
VOLUME [/var/www/html]
# Thu, 12 May 2022 22:18:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 May 2022 22:18:25 GMT
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
	-	`sha256:8104a42c0dd526d74235178802d4a78d544f3cdedd369941478616e611c44597`  
		Last Modified: Thu, 12 May 2022 21:15:44 GMT  
		Size: 11.1 MB (11117853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609eada90a7a5a3864797e39b642edbd8695947bc93ffee604d215fc4a454c72`  
		Last Modified: Thu, 12 May 2022 21:15:43 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280473cff49eaa24348c83861584f5963043872d0cb7d743b242a43e9bf1cb69`  
		Last Modified: Thu, 12 May 2022 21:15:44 GMT  
		Size: 9.9 MB (9921955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0650b3f705b092b82696e2dd37992c4ffb88fddb34958dd2c0f5b5c0048bbe`  
		Last Modified: Thu, 12 May 2022 21:15:42 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec6c5ebb7f05e2fd78ef48768f8213a070f22efe0dad237432e968030e4adf5`  
		Last Modified: Thu, 12 May 2022 21:15:42 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a589eebeae7d3b1beaf6a02b187182e3b4d602d218d867389fe4dc2fae740e`  
		Last Modified: Thu, 12 May 2022 21:15:42 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2bc45638e0b8679cbb9d0f070c7d79a4c40055a70d4d649cba82facb852fe6`  
		Last Modified: Thu, 12 May 2022 22:27:23 GMT  
		Size: 3.0 MB (2982850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611a0a35385782b5503c5a3dd44f90f4051c989faa22c642e722a7c6ced64004`  
		Last Modified: Thu, 12 May 2022 22:27:22 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcf23b97bdcf23c8d7ee6744bf1a5e07bf291675b79b5071531f4958013588d`  
		Last Modified: Thu, 12 May 2022 22:27:25 GMT  
		Size: 16.9 MB (16900906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ded0ce5ae11ee44fd3dfc285e8d04203267722a277ae6b8d68b2d5e47aead04`  
		Last Modified: Thu, 12 May 2022 22:27:22 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b7ce49bbaff821440502a65d6ec1dd54e9b5fbb6dbdff5917e4fb62a990cc3`  
		Last Modified: Thu, 12 May 2022 22:27:22 GMT  
		Size: 632.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
