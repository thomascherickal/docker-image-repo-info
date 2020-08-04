## `matomo:latest`

```console
$ docker pull matomo@sha256:831bc55ef0ae1c5b28b4bf37083b8250695fc1485b4fda2dbbdb5c5f83765446
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

### `matomo:latest` - linux; amd64

```console
$ docker pull matomo@sha256:d7e6920efbbb91a0e2cab0799cabf912e096be56497f24354e0f90a2870c4066
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.8 MB (165753141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a04ac33d026880fe72ec91943117963e350ce30e57d6dc345342d7e995ddb79d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:44:09 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 08:44:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 08:44:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 08:44:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 08:44:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 08:53:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 08:53:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 08:53:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 08:53:19 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 08:53:20 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 08:53:21 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 08:53:21 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 08:53:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 08:53:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 08:53:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 09:27:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 22 Jul 2020 09:27:49 GMT
ENV PHP_VERSION=7.4.8
# Wed, 22 Jul 2020 09:27:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.8.tar.xz.asc
# Wed, 22 Jul 2020 09:27:49 GMT
ENV PHP_SHA256=642843890b732e8af01cb661e823ae01472af1402f211c83009c9b3abd073245 PHP_MD5=
# Wed, 22 Jul 2020 09:28:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 09:28:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 09:32:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 09:32:27 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 09:32:28 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 09:32:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 09:32:29 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 09:32:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 09:32:30 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 09:32:30 GMT
EXPOSE 80
# Wed, 22 Jul 2020 09:32:31 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jul 2020 05:56:59 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 23 Jul 2020 05:58:18 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-5.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 05:58:19 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 23 Jul 2020 05:58:19 GMT
ENV MATOMO_VERSION=3.14.0
# Thu, 23 Jul 2020 05:58:31 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 05:58:31 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 23 Jul 2020 05:58:32 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Thu, 23 Jul 2020 05:58:32 GMT
VOLUME [/var/www/html]
# Thu, 23 Jul 2020 05:58:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jul 2020 05:58:32 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081a822af59557fab64a7e6b1f10993a1447c4565bee919c5a63f20e5d447207`  
		Last Modified: Wed, 22 Jul 2020 11:57:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5bea655fca655018e10a9078d5092b4d7d491ef2a9c380a0adf1c7ed119b88`  
		Last Modified: Wed, 22 Jul 2020 11:57:28 GMT  
		Size: 76.6 MB (76648810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5d9e6a44c7084c807b3c4203ec786d5bb187a14e4344496dca2d4148030e6e`  
		Last Modified: Wed, 22 Jul 2020 11:57:02 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c80d726a75cac175ad1a0f31047d9b7809b93e94ee08e0ea99d1fa8b2f8229`  
		Last Modified: Wed, 22 Jul 2020 11:57:50 GMT  
		Size: 18.7 MB (18675907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41f3ef5189e5c08bea0c669d2d214c7c8acc874f2b8f37bff1747483a664515c`  
		Last Modified: Wed, 22 Jul 2020 11:57:44 GMT  
		Size: 432.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a9c1efdc831a6e3cc46fd388cfac71cc76d715242b9c3a1a389dce263c3cc0`  
		Last Modified: Wed, 22 Jul 2020 11:57:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348c6ac678133e4b155798da0e81ad03bcb6035294d3b9663387cf73d2a14ba0`  
		Last Modified: Wed, 22 Jul 2020 11:59:00 GMT  
		Size: 10.6 MB (10620034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d16c4c4b2a5f0a5b3d345f7016fc199699b58759383db895c6c836ece236b49b`  
		Last Modified: Wed, 22 Jul 2020 11:58:59 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:035ee560bfbcfdcd849df9faf0ebe85370b0ecf68c117bb3490c86e53ff3fc1b`  
		Last Modified: Wed, 22 Jul 2020 11:59:03 GMT  
		Size: 13.8 MB (13803754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c16f7d16e8657b40dc22f726bc5e605f17905f4e2b4bc296cb9bf218f913caf`  
		Last Modified: Wed, 22 Jul 2020 11:58:59 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560feb679e04e202b3bf2c8c68715e9d9c50621e51fd33016700b2b6b1576594`  
		Last Modified: Wed, 22 Jul 2020 11:58:59 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc8defe61af3c69a26425e57b1737313373b9d997fc7cbd92964be45eb653fa`  
		Last Modified: Wed, 22 Jul 2020 11:58:59 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8784fb59498f42839835a645d278cceaddc3be3b48697b52e89411563eb520c`  
		Last Modified: Thu, 23 Jul 2020 06:00:49 GMT  
		Size: 3.5 MB (3519089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8408cdd6af1d1f973972c5251202a501ef1e25e7921c971424cbd113fe967e35`  
		Last Modified: Thu, 23 Jul 2020 06:00:48 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eff54803a2d9681b9d45110e2bc90e01476c9fffca2932b5002f23faff8832`  
		Last Modified: Thu, 23 Jul 2020 06:00:52 GMT  
		Size: 15.4 MB (15380857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aef2985091b6ec2b3e1564ae69be4e5fbb54e72e3f0b0670ca834bce42e26b1`  
		Last Modified: Thu, 23 Jul 2020 06:00:48 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9aaea308fc0b68401ce338ec3dade97979e613b131af41a716fa77922d5c727`  
		Last Modified: Thu, 23 Jul 2020 06:00:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:latest` - linux; arm variant v5

```console
$ docker pull matomo@sha256:b9a6611c702d6930c1212dc06fa81ce380acd733b2e4bc7126aaff18a4908864
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.9 MB (143891569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b910275a5d33b576ac70dc75f5ec8b8e4ff68d00ea608588d6f027c65c9e505`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 00:51:01 GMT
ADD file:4ea2d111c970d510f4eccf0fa08caafde1d227fc4c249d67c1b9d99998b0b906 in / 
# Wed, 22 Jul 2020 00:51:04 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:37:57 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 02:38:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 02:39:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 02:39:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 02:39:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 02:46:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 02:46:01 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 02:46:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 02:46:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 02:47:08 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 02:47:09 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 02:47:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 02:47:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 02:47:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 02:47:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 03:08:52 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 22 Jul 2020 03:08:53 GMT
ENV PHP_VERSION=7.4.8
# Wed, 22 Jul 2020 03:08:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.8.tar.xz.asc
# Wed, 22 Jul 2020 03:08:54 GMT
ENV PHP_SHA256=642843890b732e8af01cb661e823ae01472af1402f211c83009c9b3abd073245 PHP_MD5=
# Wed, 22 Jul 2020 03:09:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 03:09:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 03:12:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 03:13:09 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 03:13:30 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 03:13:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 03:13:40 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 03:13:49 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 03:13:54 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 03:14:02 GMT
EXPOSE 80
# Wed, 22 Jul 2020 03:14:07 GMT
CMD ["apache2-foreground"]
# Wed, 22 Jul 2020 18:05:53 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 22 Jul 2020 18:08:23 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-5.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:08:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Jul 2020 18:08:44 GMT
ENV MATOMO_VERSION=3.14.0
# Wed, 22 Jul 2020 18:09:28 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:09:37 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 22 Jul 2020 18:09:46 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Wed, 22 Jul 2020 18:09:49 GMT
VOLUME [/var/www/html]
# Wed, 22 Jul 2020 18:09:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 18:09:55 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:7ae4223cfc253e8d54407ec654ed8fb606352daea8da124f33dacd17626259ad`  
		Last Modified: Wed, 22 Jul 2020 00:58:53 GMT  
		Size: 24.8 MB (24837461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121b9a2d2615295452a8d377696a9c2ffb89b0176f7cc3b701db363dbb4142f0`  
		Last Modified: Wed, 22 Jul 2020 04:39:35 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae84ea44ff3bff3f0c88ef55cd974a2c80a16e636d903143859b537ce76d0fb`  
		Last Modified: Wed, 22 Jul 2020 04:39:56 GMT  
		Size: 58.8 MB (58799780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8462af0cdae0d179cc321c75b4e11be78793c1b3c7abf6032619bead6d90625f`  
		Last Modified: Wed, 22 Jul 2020 04:39:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f957f0803bb1b7f286e604ebc2fa6e9d1eb5ca7e3c52495ce2e323373e4794fc`  
		Last Modified: Wed, 22 Jul 2020 04:40:20 GMT  
		Size: 18.0 MB (18024762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545af90b203c679e341f1d33eacd0629f2b3e98426bb13115cc3f45f24fcdc4d`  
		Last Modified: Wed, 22 Jul 2020 04:40:15 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188f0ab43370f25ca1d73bb0d2dcd2fb820238826aa74b427c53d6f3157525fc`  
		Last Modified: Wed, 22 Jul 2020 04:40:15 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9ef32050cdca83f4afda8f3382cb84dfca23c6f2db1a3b9acba29b06b8a857`  
		Last Modified: Wed, 22 Jul 2020 04:41:58 GMT  
		Size: 10.6 MB (10618135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bca7269c9d0e654624ae48e90b4d388352bd199da922dc79a528ba214e9f2df`  
		Last Modified: Wed, 22 Jul 2020 04:41:55 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e10021ecd3207535051cb685dff82f2f893cd22a14fb0e3e8a3480e4f25108`  
		Last Modified: Wed, 22 Jul 2020 04:42:00 GMT  
		Size: 12.9 MB (12890869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d46f7e25ff49c1a46d900ba0ab5d3103c63e829445c8f7943afa3c717997b5b`  
		Last Modified: Wed, 22 Jul 2020 04:41:55 GMT  
		Size: 2.3 KB (2285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b8d0f2ade3302525d6dcc2005c76e3b12f23f9c349003f303859aea17ad525`  
		Last Modified: Wed, 22 Jul 2020 04:41:55 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c8deceea209f0a49099bbaf02b992deaa360c6e8f47cb38a112c715be43c7c`  
		Last Modified: Wed, 22 Jul 2020 04:41:55 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e3e0e200530892966ebedfac9722fec964e8d9af9ee6ee629c9ffd4e88cb56`  
		Last Modified: Wed, 22 Jul 2020 18:14:49 GMT  
		Size: 3.3 MB (3335486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05504f4c2d42f8dc297364d80cac8c6f75bee5e07677e5a4fb5b5cfa4b77318`  
		Last Modified: Wed, 22 Jul 2020 18:14:49 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ecf2e4fba728dce46f179c5e00b7be2a0eccbe7054ea7bcb35b6ce8396a2bb`  
		Last Modified: Wed, 22 Jul 2020 18:14:57 GMT  
		Size: 15.4 MB (15378809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9688cb44779e5d86e3f1f9e852fed4ab63d6fb3b4d6b5e4c4f7c270544650080`  
		Last Modified: Wed, 22 Jul 2020 18:14:48 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e8235fefe4c584a069b5b54fd4dd91cefb968e6935e2a81344943c73a78e32`  
		Last Modified: Wed, 22 Jul 2020 18:14:48 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:latest` - linux; arm variant v7

```console
$ docker pull matomo@sha256:ae0002402e83d98e5bf79afaac4842ff26baeab62ae4306a610ef08de6c7d1d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.1 MB (141097403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62b53efe222560bac78936d2f44d9d3af2cd1ccfa346669467fb39b09ad47c40`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 01:19:50 GMT
ADD file:c47f7b84c9113624f53d9c52e13f649f1e5d739665b5a5a5df6b1d5b5274d71b in / 
# Wed, 22 Jul 2020 01:19:58 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 09:31:35 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 09:31:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 09:32:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 09:32:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 09:32:19 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 09:35:40 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 09:35:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 09:36:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 09:36:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 09:36:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 09:36:13 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 09:36:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 09:36:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 09:36:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 09:36:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 09:57:18 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 22 Jul 2020 09:57:30 GMT
ENV PHP_VERSION=7.4.8
# Wed, 22 Jul 2020 09:57:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.8.tar.xz.asc
# Wed, 22 Jul 2020 09:57:41 GMT
ENV PHP_SHA256=642843890b732e8af01cb661e823ae01472af1402f211c83009c9b3abd073245 PHP_MD5=
# Wed, 22 Jul 2020 09:58:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 09:58:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 10:01:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 10:01:46 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 10:02:01 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 10:02:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 10:02:06 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 10:02:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 10:02:12 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 10:02:15 GMT
EXPOSE 80
# Wed, 22 Jul 2020 10:02:20 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jul 2020 04:57:22 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 23 Jul 2020 04:59:31 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-5.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 04:59:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 23 Jul 2020 04:59:37 GMT
ENV MATOMO_VERSION=3.14.0
# Thu, 23 Jul 2020 05:00:13 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 05:00:15 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 23 Jul 2020 05:00:18 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Thu, 23 Jul 2020 05:00:20 GMT
VOLUME [/var/www/html]
# Thu, 23 Jul 2020 05:00:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jul 2020 05:00:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0c4667eb56da53c2c07c288a210a70fb8d6089f57ce32a2cd88c2a75ae9ad8af`  
		Last Modified: Wed, 22 Jul 2020 01:40:34 GMT  
		Size: 22.7 MB (22705906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73a476362b835810ad6f6eaecc2a497b4302f2b8ac196c911884fe753f3be0c`  
		Last Modified: Wed, 22 Jul 2020 11:54:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbec70860f5643fca4a35066a02be7aab2ad53c776daa74f2b6d2bc97ad9f9f3`  
		Last Modified: Wed, 22 Jul 2020 11:55:12 GMT  
		Size: 59.5 MB (59505456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7f7b8f25575d1efc6595391f7314710b2d0187564386d0cf3a81a74c4278d6`  
		Last Modified: Wed, 22 Jul 2020 11:54:53 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b46f8661c634c6b6f0f1a6e45a3452a8731b0d139678e65fe2c43eb310e9162`  
		Last Modified: Wed, 22 Jul 2020 11:55:47 GMT  
		Size: 17.5 MB (17481960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f081e3e7911001e5da489b54d64f3752a6e5faf47b5181166f0270fa9fdd0ee`  
		Last Modified: Wed, 22 Jul 2020 11:55:42 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5aae3a57b1751f2cc89b35efb321ebaed34df66f7f7db8713b8b4c93af3685d`  
		Last Modified: Wed, 22 Jul 2020 11:55:42 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ff2e8b6c5a67d58e14c47928fce5a22b609d3e212ad815227f9cede5cd74d02`  
		Last Modified: Wed, 22 Jul 2020 11:57:27 GMT  
		Size: 10.6 MB (10618112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7229bb52424dc1b4558295111bdfe3439e1b56aeba79019163be219fb1a8089`  
		Last Modified: Wed, 22 Jul 2020 11:57:23 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df45617152f1a6a7c209d51498c7e0c20336fbf29d042dc66527df5c01f638e9`  
		Last Modified: Wed, 22 Jul 2020 11:57:29 GMT  
		Size: 12.2 MB (12197251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573aa5decee2befc75ca9a74e00e66e9f31e1bd58c897d424d676677408f1725`  
		Last Modified: Wed, 22 Jul 2020 11:57:23 GMT  
		Size: 2.3 KB (2288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7fc3ae274aeb597990bfa9dc45ce232764628ec4e28ce020e88504465e9b22`  
		Last Modified: Wed, 22 Jul 2020 11:57:23 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c70ba8a7b5004feb1ba8a2e5b2a72da979e2fb4b89310d5e12b18f97d5312db`  
		Last Modified: Wed, 22 Jul 2020 11:57:23 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01fc23b104627270c5708666681bedcb0ec339777e543ceedc8a40ecac30055`  
		Last Modified: Thu, 23 Jul 2020 05:04:20 GMT  
		Size: 3.2 MB (3203602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1720f14592e0593f9f9fcd55d2367ac3f76a17a2118e46a32f9349c3750788`  
		Last Modified: Thu, 23 Jul 2020 05:04:19 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c087d4d2f544edde9ee11bdba4fce2600efb73eea1f073543b090cd47212c493`  
		Last Modified: Thu, 23 Jul 2020 05:04:26 GMT  
		Size: 15.4 MB (15378841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a2f2b3d39ec6cf296aaa525965fb054ba013500cac175799818ad939ff7b84`  
		Last Modified: Thu, 23 Jul 2020 05:04:19 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a742268ce92032cc0ff6a6b0e156902d643667181e46324945d07f54c02b0292`  
		Last Modified: Thu, 23 Jul 2020 05:04:19 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:latest` - linux; arm64 variant v8

```console
$ docker pull matomo@sha256:bde5dd94e98d83ccc872ce157778513f3cfad03e1d54db1ce1a3ab854abd42eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.8 MB (157833894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e87906655d41c6a447df873c20182ef40e08b1dda406b417c1ed0946fb830df`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 11:19:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 11:19:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 11:20:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 11:20:48 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 11:21:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 11:25:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 11:25:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 11:26:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 11:26:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 11:26:18 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 11:26:19 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 11:26:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 11:26:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 11:26:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 11:26:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 11:46:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 22 Jul 2020 11:46:15 GMT
ENV PHP_VERSION=7.4.8
# Wed, 22 Jul 2020 11:46:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.8.tar.xz.asc
# Wed, 22 Jul 2020 11:46:19 GMT
ENV PHP_SHA256=642843890b732e8af01cb661e823ae01472af1402f211c83009c9b3abd073245 PHP_MD5=
# Wed, 22 Jul 2020 11:46:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 11:46:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:50:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 11:50:10 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:50:13 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 11:50:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 11:50:24 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 11:50:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:50:38 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 11:50:44 GMT
EXPOSE 80
# Wed, 22 Jul 2020 11:50:47 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jul 2020 03:01:31 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 23 Jul 2020 03:03:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-5.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 03:03:57 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 23 Jul 2020 03:03:57 GMT
ENV MATOMO_VERSION=3.14.0
# Thu, 23 Jul 2020 03:04:19 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 03:04:26 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 23 Jul 2020 03:04:27 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Thu, 23 Jul 2020 03:04:27 GMT
VOLUME [/var/www/html]
# Thu, 23 Jul 2020 03:04:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jul 2020 03:04:29 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d0ba90fa18020ed9569da0e936f2c6d545f48231f27020a883d5de88d96a10`  
		Last Modified: Wed, 22 Jul 2020 13:32:50 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a37699742587260a77a7c676da89681dc8ca92dd2db86faee3dcc77109ccea`  
		Last Modified: Wed, 22 Jul 2020 13:33:12 GMT  
		Size: 70.3 MB (70337912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f6e19fa909b49d726f813175349e7ea4dcaa9589076b04108e40eda3f792b4`  
		Last Modified: Wed, 22 Jul 2020 13:32:49 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aec0a9b64ab8386df6bf5d945a5b1c5712c549bca9f1a0d3808138b57fa607e`  
		Last Modified: Wed, 22 Jul 2020 13:34:15 GMT  
		Size: 18.6 MB (18579398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6462f70cfa9f8b1238b00624079f1dbfe0cd6c85d195dacf4fab20d812a1d26c`  
		Last Modified: Wed, 22 Jul 2020 13:34:10 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bad882d5dcc21edad5bd6842a791c6a838844f61872200feff6f162c8d1d7e1`  
		Last Modified: Wed, 22 Jul 2020 13:34:07 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073f51e63bd9a6b5f95421624da75b080db7815580da1f7c4a9f40db4e2efafc`  
		Last Modified: Wed, 22 Jul 2020 13:36:43 GMT  
		Size: 10.6 MB (10618900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c9584743c6da68ddd1abf832ba7820e07c14b76d2528d088948e9d36c97a16`  
		Last Modified: Wed, 22 Jul 2020 13:36:39 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f43af95f3c86dd85c2d3e97552571296d5ff65f1546a1aee9b3b1e3c3598359`  
		Last Modified: Wed, 22 Jul 2020 13:36:43 GMT  
		Size: 13.6 MB (13591950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d545fe0011fedbe5d047b4a70bc06df209c859c6be9911131027aea4bb7138f`  
		Last Modified: Wed, 22 Jul 2020 13:36:39 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8236a0b4951550e4a6ac284e997f2fc262ded51f15a3afd3113e8009a791bfd8`  
		Last Modified: Wed, 22 Jul 2020 13:36:39 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0c5f7c915556acfa7b3f9aed423677e98e25832fbf4336d871e53f2089ea15`  
		Last Modified: Wed, 22 Jul 2020 13:36:39 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0461c783e10c0550512b5c7bedfaa1683af6bd7d1ad6ec639d023cd3ad4c22fb`  
		Last Modified: Thu, 23 Jul 2020 03:08:18 GMT  
		Size: 3.5 MB (3461923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a49d65e1bac6dac3d29d0abe1e5c7b42b3d78d4d9ea2922a6397f2fee36b59`  
		Last Modified: Thu, 23 Jul 2020 03:08:17 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d19993334b06735572436372b41dba39e2220686822e3cd8cc053ac5a08710`  
		Last Modified: Thu, 23 Jul 2020 03:08:23 GMT  
		Size: 15.4 MB (15379733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5ff6f45261e4532f40e2bc752a5a3538c8137760cd908e7a7fc4e3b98eed00`  
		Last Modified: Thu, 23 Jul 2020 03:08:17 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb20113f5d36531b64e347b4b3c9cd4cf568804b9bb1cded4e9dfca1edf400c`  
		Last Modified: Thu, 23 Jul 2020 03:08:17 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:latest` - linux; 386

```console
$ docker pull matomo@sha256:a3bf74264c67ba523d89e479b21aa1b1f6f2dace313a2e734faa0a73c45b0a8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.7 MB (171743664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99ba9751c29a130412214a8c143b670c77a7caa5718f18416ae84b4ef5ff57ae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:35 GMT
ADD file:cc791c21e6022a12dd1445a35f4cca9392ad8edfe34ea5852f3e87862c943628 in / 
# Tue, 04 Aug 2020 03:37:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 12:50:23 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 12:50:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 12:50:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 12:50:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 12:50:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 12:55:58 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Aug 2020 12:55:58 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Aug 2020 12:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Aug 2020 12:56:09 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Aug 2020 12:56:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Aug 2020 12:56:10 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 04 Aug 2020 12:56:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 04 Aug 2020 12:56:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 12:56:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 12:56:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 13:17:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 04 Aug 2020 13:17:23 GMT
ENV PHP_VERSION=7.4.8
# Tue, 04 Aug 2020 13:17:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.8.tar.xz.asc
# Tue, 04 Aug 2020 13:17:24 GMT
ENV PHP_SHA256=642843890b732e8af01cb661e823ae01472af1402f211c83009c9b3abd073245 PHP_MD5=
# Tue, 04 Aug 2020 13:17:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Aug 2020 13:17:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Aug 2020 13:20:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 04 Aug 2020 13:20:40 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 04 Aug 2020 13:20:41 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Aug 2020 13:20:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Aug 2020 13:20:42 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Aug 2020 13:20:42 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Aug 2020 13:20:42 GMT
WORKDIR /var/www/html
# Tue, 04 Aug 2020 13:20:42 GMT
EXPOSE 80
# Tue, 04 Aug 2020 13:20:42 GMT
CMD ["apache2-foreground"]
# Tue, 04 Aug 2020 19:39:40 GMT
LABEL maintainer=pierre@piwik.org
# Tue, 04 Aug 2020 19:41:07 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-5.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 19:41:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 04 Aug 2020 19:41:08 GMT
ENV MATOMO_VERSION=3.14.0
# Tue, 04 Aug 2020 19:41:21 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 19:41:22 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Tue, 04 Aug 2020 19:41:22 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Tue, 04 Aug 2020 19:41:22 GMT
VOLUME [/var/www/html]
# Tue, 04 Aug 2020 19:41:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 19:41:22 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:23ad22c16ab9d635a179d5d341096c34912941507b0c77ac97083b9795d8516f`  
		Last Modified: Tue, 04 Aug 2020 03:42:33 GMT  
		Size: 27.8 MB (27750435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:329242062d68d28d6b2a87364a30d8b71938ba033610ecfd79f13769a96294e2`  
		Last Modified: Tue, 04 Aug 2020 14:58:57 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8aaae05adb825dff3551448f99133aba9f351d7f26f8c75f6486b4b38bd51c`  
		Last Modified: Tue, 04 Aug 2020 14:59:19 GMT  
		Size: 81.2 MB (81196323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65de971d0774dc002b56e15b037e7d4db04da66913020270e1285355323dbb`  
		Last Modified: Tue, 04 Aug 2020 14:58:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5237681b89148747d9421150d867c5cc8449bf341cbc8ad214f71d9b03794a23`  
		Last Modified: Tue, 04 Aug 2020 14:59:36 GMT  
		Size: 19.1 MB (19112679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7cf510e15402722d29174d2b186ac456076ed7d047fe794a07db362136ba17`  
		Last Modified: Tue, 04 Aug 2020 14:59:30 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be410499ff850773e8553b98b72aa2ee3faac6f4ae8040ea8f296bd35a419521`  
		Last Modified: Tue, 04 Aug 2020 14:59:30 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b55d2f2761e2d5a9f88dd8346e4891a15f8bdf82415fa86d4f11080800236c0`  
		Last Modified: Tue, 04 Aug 2020 15:00:44 GMT  
		Size: 10.6 MB (10619276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e8b403fc1df70517f991f26f7c2bd39403a42cfa4285833733f9ed2ac5a24e`  
		Last Modified: Tue, 04 Aug 2020 15:00:42 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71c1cc7715d0be695cca0d105be367b8c0b71e0397eda06bd560341a095eca4`  
		Last Modified: Tue, 04 Aug 2020 15:00:48 GMT  
		Size: 14.1 MB (14137433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99df7e53d2edd1b9aaf4e37f356a6ae1a9048cbb6947a59a21ac4c531541c8ca`  
		Last Modified: Tue, 04 Aug 2020 15:00:42 GMT  
		Size: 2.3 KB (2286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed12927eb30deec2b245b11c9c1d9a5583274ebc9a92699fdb9bb26f4973940a`  
		Last Modified: Tue, 04 Aug 2020 15:00:42 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a7b294d1578c90bb49364d2a0cd6b812fa22a2979c40af8423b388ea10390f`  
		Last Modified: Tue, 04 Aug 2020 15:00:42 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6f5c360faa171ced25b9ba4c0389a58dc41698ea680962139411906c2696c8`  
		Last Modified: Tue, 04 Aug 2020 19:43:37 GMT  
		Size: 3.5 MB (3541396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11ff9f4a069987bd27fd7d527b527a4019743adde1928f9a94c8bdfa3784f4e`  
		Last Modified: Tue, 04 Aug 2020 19:43:36 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41372cc1bb5ecbe1000ea2503368411cfde6b376bba31d80d52873bc173ee904`  
		Last Modified: Tue, 04 Aug 2020 19:43:42 GMT  
		Size: 15.4 MB (15379966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb60f597236f7b7d2a4364e406baef80984fffe0cf8114e7813c2ca4a71fac7b`  
		Last Modified: Tue, 04 Aug 2020 19:43:36 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a9d2436bd20ba13dde802d9c16ef6d90e1fe2c1ac3dac34796c6f133a153d3`  
		Last Modified: Tue, 04 Aug 2020 19:43:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:latest` - linux; mips64le

```console
$ docker pull matomo@sha256:e737fbb47143de634b9dec86e8996912545126cb7e285a573fda1585bf724423
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.3 MB (148339783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7322f0810e1899044e1d1bd4a81a68310a38c5c601bba2097a88c0ccb403e993`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 01:09:52 GMT
ADD file:67401cc8bdd27435a027e4051d2eb03c5012a09274aaae230008279234586dfb in / 
# Wed, 22 Jul 2020 01:09:53 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 10:58:51 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 10:58:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 10:59:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 10:59:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 10:59:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 11:12:34 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 11:12:35 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 11:13:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 11:13:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 11:13:06 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 11:13:06 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 11:13:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 11:13:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 11:13:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 11:13:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 12:04:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 22 Jul 2020 12:04:34 GMT
ENV PHP_VERSION=7.4.8
# Wed, 22 Jul 2020 12:04:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.8.tar.xz.asc
# Wed, 22 Jul 2020 12:04:35 GMT
ENV PHP_SHA256=642843890b732e8af01cb661e823ae01472af1402f211c83009c9b3abd073245 PHP_MD5=
# Wed, 22 Jul 2020 12:04:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 12:04:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 12:12:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 12:12:42 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 12:12:44 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 12:12:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 12:12:45 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 12:12:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 12:12:46 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 12:12:46 GMT
EXPOSE 80
# Wed, 22 Jul 2020 12:12:46 GMT
CMD ["apache2-foreground"]
# Wed, 22 Jul 2020 21:37:59 GMT
LABEL maintainer=pierre@piwik.org
# Wed, 22 Jul 2020 21:42:12 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-5.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 21:42:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 22 Jul 2020 21:42:14 GMT
ENV MATOMO_VERSION=3.14.0
# Wed, 22 Jul 2020 21:42:47 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 21:42:48 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Wed, 22 Jul 2020 21:42:48 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Wed, 22 Jul 2020 21:42:49 GMT
VOLUME [/var/www/html]
# Wed, 22 Jul 2020 21:42:49 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Jul 2020 21:42:49 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:2cab09a0ed78d8465b06bc43bf504e7c4ed41f36db2ee9cb181c154d562fc9ff`  
		Last Modified: Wed, 22 Jul 2020 01:16:46 GMT  
		Size: 25.8 MB (25764196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8463e01d615b1d9517d01aa40d7ba0e6f6a788293708a58d907fa6221b7ff2`  
		Last Modified: Wed, 22 Jul 2020 14:18:42 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b823b35b4bd69b6de3643bb888921aa9369941215577b5970313929f85cd6fe`  
		Last Modified: Wed, 22 Jul 2020 14:19:32 GMT  
		Size: 61.4 MB (61386557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514d0f889e1897eb582ad0ce9cf56634f335da1e0f69b6193ec78ac78cc68af3`  
		Last Modified: Wed, 22 Jul 2020 14:18:41 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833124c62ae0ecd011111e6a50af48ce39b4583ae6259a2d55d6cb1ac211d774`  
		Last Modified: Wed, 22 Jul 2020 14:20:24 GMT  
		Size: 18.6 MB (18606092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2651b9994223d022cde9c6e3b1c789b95b41b47bca6871d648e476595cd287ed`  
		Last Modified: Wed, 22 Jul 2020 14:20:11 GMT  
		Size: 448.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b97f58d27aac769f11bff21558457913af2612c36d16c46ee10bdf6d726543`  
		Last Modified: Wed, 22 Jul 2020 14:20:11 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038cd744361d5225b81a2041f583f4881d077c8c1bdfef2700a037c8bcd84e71`  
		Last Modified: Wed, 22 Jul 2020 14:23:47 GMT  
		Size: 10.6 MB (10617425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673e45eaadf706c30c5a40975cba89fb144407b8eb7e582b9b35c60cc9a7d629`  
		Last Modified: Wed, 22 Jul 2020 14:23:40 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6189004150215b9b0ab0091514c56749d053d78b029fe0fad3c77da3e397c34`  
		Last Modified: Wed, 22 Jul 2020 14:23:51 GMT  
		Size: 13.1 MB (13109886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23eebc8454a1f44662dd84edcdd2d662dd48d9d8ad48056a0b21531ce89297d`  
		Last Modified: Wed, 22 Jul 2020 14:23:40 GMT  
		Size: 2.3 KB (2284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3ef468911e882dc7d0cc73587890be69e4b8506c5feee0269966c465f35e2b`  
		Last Modified: Wed, 22 Jul 2020 14:23:40 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6ad44ee9b8b4070b9c5a4410319e0ccbb35d0ad155ff8ef04e8a5d5bcfa1a2`  
		Last Modified: Wed, 22 Jul 2020 14:23:40 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9a93669d337f047a52d3cace7e7f14167d786a615d3bc8d831be84df84cfcc`  
		Last Modified: Wed, 22 Jul 2020 21:48:12 GMT  
		Size: 3.5 MB (3471564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee317458b070520f8b29cf056a09d2290e24ead563d99b97bcad4d337ddacca`  
		Last Modified: Wed, 22 Jul 2020 21:48:09 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57558bad329e0b2d58428f684fdeb15160221ddf88366dd5d79f15c4a039c992`  
		Last Modified: Wed, 22 Jul 2020 21:48:23 GMT  
		Size: 15.4 MB (15377903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be6dc65705fbb97c0ae4a27245b6ea624ccb8a435e7da3ad3021a2433b70c32`  
		Last Modified: Wed, 22 Jul 2020 21:48:09 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2b5a1500671b2c4dbf6c5ff84410c0d3b95fdadb17feee8ae1553c788b75f5`  
		Last Modified: Wed, 22 Jul 2020 21:48:09 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:latest` - linux; ppc64le

```console
$ docker pull matomo@sha256:50ea272117ab6a3bb3989af06be80f701b9176d2cc6480d2ed965f6b09536541
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.2 MB (177196021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95a1b8b5c60149bf40212a36ab6deae6b6bb4841becdc634f5b5542eb1c85176`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 22 Jul 2020 02:16:05 GMT
ADD file:037dec996d9b742fc49f675272aa42ebd31f04226ba3d28836a6556cb61c29e7 in / 
# Wed, 22 Jul 2020 02:16:14 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 10:19:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 22 Jul 2020 10:19:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 22 Jul 2020 10:23:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 10:24:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 22 Jul 2020 10:24:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 22 Jul 2020 10:31:39 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 22 Jul 2020 10:31:43 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 22 Jul 2020 10:33:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 22 Jul 2020 10:33:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 22 Jul 2020 10:33:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 22 Jul 2020 10:33:36 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 22 Jul 2020 10:33:42 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 22 Jul 2020 10:33:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 10:33:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 22 Jul 2020 10:33:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 22 Jul 2020 11:06:42 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 22 Jul 2020 11:06:47 GMT
ENV PHP_VERSION=7.4.8
# Wed, 22 Jul 2020 11:06:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.8.tar.xz.asc
# Wed, 22 Jul 2020 11:06:58 GMT
ENV PHP_SHA256=642843890b732e8af01cb661e823ae01472af1402f211c83009c9b3abd073245 PHP_MD5=
# Wed, 22 Jul 2020 11:08:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 22 Jul 2020 11:08:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:18:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 22 Jul 2020 11:18:23 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:18:32 GMT
RUN docker-php-ext-enable sodium
# Wed, 22 Jul 2020 11:18:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 22 Jul 2020 11:18:43 GMT
STOPSIGNAL SIGWINCH
# Wed, 22 Jul 2020 11:18:45 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 22 Jul 2020 11:18:57 GMT
WORKDIR /var/www/html
# Wed, 22 Jul 2020 11:19:05 GMT
EXPOSE 80
# Wed, 22 Jul 2020 11:19:12 GMT
CMD ["apache2-foreground"]
# Thu, 23 Jul 2020 01:38:49 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 23 Jul 2020 01:43:01 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-5.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 01:43:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 23 Jul 2020 01:43:42 GMT
ENV MATOMO_VERSION=3.14.0
# Thu, 23 Jul 2020 01:46:25 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 01:46:29 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 23 Jul 2020 01:46:32 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Thu, 23 Jul 2020 01:46:36 GMT
VOLUME [/var/www/html]
# Thu, 23 Jul 2020 01:46:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Jul 2020 01:47:03 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d022338f917106731b8902d4c3d7009435a41381c11c8d210bbd6af007569f69`  
		Last Modified: Wed, 22 Jul 2020 02:26:01 GMT  
		Size: 30.5 MB (30524562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0664a61881d05cc0e8746a8342755ac9442a4f3e87073026096655cc55b0cc3`  
		Last Modified: Wed, 22 Jul 2020 13:40:57 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d65645e6fdf84bfa39a94f46a90aacec09a0d1d2d2606c365eb9a65c678fd4`  
		Last Modified: Wed, 22 Jul 2020 13:41:16 GMT  
		Size: 82.3 MB (82263064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a1f3da03577e1ffffca6abcd3a26313f2ed2f8424e1f2dfe21237345fd9b47`  
		Last Modified: Wed, 22 Jul 2020 13:40:56 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5aac227a858593c6ac591b034979662721f134208c6f657fc0cdcc50f932c28`  
		Last Modified: Wed, 22 Jul 2020 13:42:01 GMT  
		Size: 19.8 MB (19812717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc67444503678c507c7e200d091883e3efe5463840d760c2cc4424be652a66c`  
		Last Modified: Wed, 22 Jul 2020 13:41:56 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9862a2035d6f95cde26e90287a17412d671778d047eca5331343352c5a6979`  
		Last Modified: Wed, 22 Jul 2020 13:41:56 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00529d7f087c6c4753f524c27271f256326e1d4e6862dbae39b247fbc1e994e2`  
		Last Modified: Wed, 22 Jul 2020 13:44:20 GMT  
		Size: 10.6 MB (10619998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:def2914250a7f5a6f063be4870b697de60fbb58582908babea3d7f3bb1613c9b`  
		Last Modified: Wed, 22 Jul 2020 13:44:11 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68ca052f137a346f262de4898526369bfe0c4f84c862eaf73a3bdf7d60bfaf0`  
		Last Modified: Wed, 22 Jul 2020 13:44:18 GMT  
		Size: 14.8 MB (14844219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fe0daf9874b2be6f13692902ce7792ec143a911d9d44eb4e01885466da7cff`  
		Last Modified: Wed, 22 Jul 2020 13:44:11 GMT  
		Size: 2.3 KB (2283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e162194d37ad459c6ce5ba570210361ddb377c9e8aad1ff8f03f38a8e6d51f`  
		Last Modified: Wed, 22 Jul 2020 13:44:12 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046f05c674c9d300b0169ea204fd8a9b7c8be986feaa4d34db4e58e61bf6025f`  
		Last Modified: Wed, 22 Jul 2020 13:44:11 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabff5ca015d00a5abb4e35c56f344727dc893610f7786fdf4c2c7e88c673355`  
		Last Modified: Thu, 23 Jul 2020 01:55:18 GMT  
		Size: 3.7 MB (3743456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2ceace32a6a04398b703824f51c402444778d7a330acc6c9e34c7bb25e00be`  
		Last Modified: Thu, 23 Jul 2020 01:55:17 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1abd9294779dbd7ecd23da86d2740518312827b98a88812081b9f73e25e1e21`  
		Last Modified: Thu, 23 Jul 2020 01:55:21 GMT  
		Size: 15.4 MB (15381736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a427d893e6d6c8292dca90b09b4ed61eaf4d2a3b8606be99301ab8ec8ff62f60`  
		Last Modified: Thu, 23 Jul 2020 01:55:17 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46cd0d0d43d72e0c41c61aa7132bfc8cf84da6bb87371a98e960bada4eb1724`  
		Last Modified: Thu, 23 Jul 2020 01:55:17 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:latest` - linux; s390x

```console
$ docker pull matomo@sha256:c9105c126552ae974efef7a39016100ed41eea92dbc8c6f9fe53e9aab701072d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151438708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895bb98e0395ab56f1f64616fd05223b6d92683ff6400e2f828acb0d81d7f5a5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 04 Aug 2020 01:17:16 GMT
ADD file:2ffa27c57800f9370adbaecca870158ec38c3d25a58b8803e2447c5e9320c5bb in / 
# Tue, 04 Aug 2020 01:17:17 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 03:17:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 04 Aug 2020 03:17:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 04 Aug 2020 03:17:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 03:18:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 04 Aug 2020 03:18:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 04 Aug 2020 03:20:19 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 04 Aug 2020 03:20:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 04 Aug 2020 03:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 04 Aug 2020 03:20:28 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 04 Aug 2020 03:20:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 03:20:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 04 Aug 2020 03:20:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 04 Aug 2020 03:29:43 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 04 Aug 2020 03:29:43 GMT
ENV PHP_VERSION=7.4.8
# Tue, 04 Aug 2020 03:29:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.8.tar.xz.asc
# Tue, 04 Aug 2020 03:29:44 GMT
ENV PHP_SHA256=642843890b732e8af01cb661e823ae01472af1402f211c83009c9b3abd073245 PHP_MD5=
# Tue, 04 Aug 2020 03:29:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 04 Aug 2020 03:29:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 04 Aug 2020 03:31:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 04 Aug 2020 03:31:09 GMT
COPY multi:af24b1d34daac0a277386947399eceaaf20d3065d4be5db00b1d6466cf006c49 in /usr/local/bin/ 
# Tue, 04 Aug 2020 03:31:09 GMT
RUN docker-php-ext-enable sodium
# Tue, 04 Aug 2020 03:31:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 04 Aug 2020 03:31:10 GMT
STOPSIGNAL SIGWINCH
# Tue, 04 Aug 2020 03:31:10 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 04 Aug 2020 03:31:10 GMT
WORKDIR /var/www/html
# Tue, 04 Aug 2020 03:31:10 GMT
EXPOSE 80
# Tue, 04 Aug 2020 03:31:11 GMT
CMD ["apache2-foreground"]
# Tue, 04 Aug 2020 10:29:43 GMT
LABEL maintainer=pierre@piwik.org
# Tue, 04 Aug 2020 10:30:47 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libldap2-dev 		libpng-dev 		libzip-dev 	; 		debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch"; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-5.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:30:48 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 04 Aug 2020 10:30:48 GMT
ENV MATOMO_VERSION=3.14.0
# Tue, 04 Aug 2020 10:30:59 GMT
RUN set -ex; 	fetchDeps=" 		dirmngr 		gnupg 	"; 	apt-get update; 	apt-get install -y --no-install-recommends 		$fetchDeps 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:31:01 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Tue, 04 Aug 2020 10:31:01 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Tue, 04 Aug 2020 10:31:02 GMT
VOLUME [/var/www/html]
# Tue, 04 Aug 2020 10:31:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Aug 2020 10:31:02 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0c46adfa2de4a7b7eb1fe2f0cb928f9e15a4cc94b7b975f13392f397cbfb0f2c`  
		Last Modified: Tue, 04 Aug 2020 01:20:03 GMT  
		Size: 25.7 MB (25707641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f8604b15b40b87c7c78f35c952be34d77e22c70a7a3d634af952bed77df82a`  
		Last Modified: Tue, 04 Aug 2020 03:56:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c79c3a25fa505e04cf025f8485f429f891ecf1609983c99d0f0b81a99aa8f54`  
		Last Modified: Tue, 04 Aug 2020 03:56:16 GMT  
		Size: 64.7 MB (64706546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007fcb88e4f44656bd1669c15b17ec295337d9d3a8ac3764848b6130f737ac05`  
		Last Modified: Tue, 04 Aug 2020 03:56:06 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef93b86f4a7b3b0359b5f145a6f9cfa99af8cbc9e23a11458d496d3d4902854`  
		Last Modified: Tue, 04 Aug 2020 03:56:35 GMT  
		Size: 18.5 MB (18522609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d03de6a7739c46b225f487b15c9e4745f8a3360dc4d59e0c81b5659e6e209e9e`  
		Last Modified: Tue, 04 Aug 2020 03:56:33 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16499546079fb354707b57f0646a75ded183022339942a95fe84bcfa606be992`  
		Last Modified: Tue, 04 Aug 2020 03:56:32 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea38ae10cad7ba0a8b10d61f6f485498b17bc6a8332170c301efdca7e405a02`  
		Last Modified: Tue, 04 Aug 2020 03:57:38 GMT  
		Size: 10.6 MB (10618372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f5f023fcdfa5ba19d4437e82fdb47ee3db2961243b9554c337fed27d7ede82`  
		Last Modified: Tue, 04 Aug 2020 03:57:35 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4dc94b0224c064612d508478d72cb7105dd5b4bf7258a0a43fbc065d89c282`  
		Last Modified: Tue, 04 Aug 2020 03:57:38 GMT  
		Size: 13.0 MB (13021591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1346bad8d596871674e5b2c0d4f7dfb5c46dddd3fa98788ba716a5fd7a6eac5`  
		Last Modified: Tue, 04 Aug 2020 03:57:35 GMT  
		Size: 2.3 KB (2287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43700986432cbcb2f093d9c290554832fd1a5a617260cbb163b1f68043c8de6e`  
		Last Modified: Tue, 04 Aug 2020 03:57:35 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b8f0164243592cda14c28a9ad269b5e59f28e9a665dde9ef34484d1e6bba4`  
		Last Modified: Tue, 04 Aug 2020 03:57:35 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68373a83419a1f9f82155d1be85e44da26cf6ffda7f7ba0e0510f9bae1d745c5`  
		Last Modified: Tue, 04 Aug 2020 10:32:59 GMT  
		Size: 3.5 MB (3476704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d120f60e1d098a67467a4e4d211f4e57dc27eda9ec0381a75298fce3930954`  
		Last Modified: Tue, 04 Aug 2020 10:32:59 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d834d6698fc81d049edb76ed8b43459f150d14cca4511766c2c5b8e14f25ed9`  
		Last Modified: Tue, 04 Aug 2020 10:33:01 GMT  
		Size: 15.4 MB (15378984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ce7e575a84aac7b97c4f81f4fe7f2102109656a8b3e94017b467f4cd6aed31`  
		Last Modified: Tue, 04 Aug 2020 10:32:59 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74f02391e8d0e8c5702e9262050042b7b87b8c08366d8f385fcd77167d000c7`  
		Last Modified: Tue, 04 Aug 2020 10:32:59 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
