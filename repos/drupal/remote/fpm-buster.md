## `drupal:fpm-buster`

```console
$ docker pull drupal@sha256:9da9e70fc811ba98cd6af35423bdecc7d020fd1a4f29a6b7563c6b884ee6b5c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:fpm-buster` - linux; amd64

```console
$ docker pull drupal@sha256:18533d74dd78d3930a23ba2f369f99617e733d4604537ad184f77b0c6b9a1639
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.8 MB (165826160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb8ac6d13c8bbbb5ef659339314354ce5570b0acc2d18c97cb8433f31855050c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:35:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 22 Jul 2021 01:35:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 22 Jul 2021 01:36:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:36:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Jul 2021 01:36:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Jul 2021 01:53:43 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Jul 2021 01:53:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 01:53:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 01:53:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Jul 2021 02:29:37 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 30 Jul 2021 00:39:28 GMT
ENV PHP_VERSION=8.0.9
# Fri, 30 Jul 2021 00:39:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Fri, 30 Jul 2021 00:39:28 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Fri, 30 Jul 2021 00:39:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 30 Jul 2021 00:39:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Jul 2021 00:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Jul 2021 00:45:50 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 30 Jul 2021 00:45:51 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Jul 2021 00:45:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Jul 2021 00:45:51 GMT
WORKDIR /var/www/html
# Fri, 30 Jul 2021 00:45:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 30 Jul 2021 00:45:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 30 Jul 2021 00:45:53 GMT
EXPOSE 9000
# Fri, 30 Jul 2021 00:45:53 GMT
CMD ["php-fpm"]
# Fri, 30 Jul 2021 02:49:04 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 30 Jul 2021 02:49:04 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 30 Jul 2021 02:49:05 GMT
COPY file:3e162edb3278a885c516d518136f3034c1eced6f4248bd3295042096c46920e3 in /usr/local/bin/ 
# Fri, 13 Aug 2021 00:20:08 GMT
ENV DRUPAL_VERSION=9.2.4
# Fri, 13 Aug 2021 00:20:09 GMT
WORKDIR /opt/drupal
# Fri, 13 Aug 2021 00:20:18 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 13 Aug 2021 00:20:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba03c99d34ed5eef03bd9b50e93e7c4ef428d351bc473dbc5af6b35e3b38ca23`  
		Last Modified: Thu, 22 Jul 2021 04:14:30 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f637ed06e1a5cbebe59f7e1102e78d40b788c8ff3143b1c6e6e2d1fda3b8554`  
		Last Modified: Thu, 22 Jul 2021 04:14:43 GMT  
		Size: 76.7 MB (76681016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfd84713df3e0b309ebfe29910fd6efc5803314e93a7866d1e5e31b458f719d`  
		Last Modified: Thu, 22 Jul 2021 04:14:30 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433a69861e85a0ab0cdf4432721e337dcf08c5e3bb5895117dc04f62d00e993f`  
		Last Modified: Fri, 30 Jul 2021 02:20:47 GMT  
		Size: 11.0 MB (11000212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a936b7cd1c7c33af75f6250fe246227f880feefb929df85328eac710fc1eae`  
		Last Modified: Fri, 30 Jul 2021 02:20:44 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92804f1310e20f5789770a570ebb69f4e9618038329960299e79fd0a3b4cf145`  
		Last Modified: Fri, 30 Jul 2021 02:20:48 GMT  
		Size: 29.2 MB (29221079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10147aecdd5c59671823ac2709b97a20c05246957d72581ea9a2eb74b950af98`  
		Last Modified: Fri, 30 Jul 2021 02:20:44 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1525d88eed9489ff47f60b5163bf06e441d80f452e3cb43c203631f812302f4c`  
		Last Modified: Fri, 30 Jul 2021 02:20:44 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae1786a42c053e85ae96072360110dbb698acc02bc6c607dddd34fd356a4684`  
		Last Modified: Fri, 30 Jul 2021 02:20:44 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fcce6ebf323be4b46e0474364bde00f85cd2a29cc09d03a150e22ed1e52919`  
		Last Modified: Fri, 30 Jul 2021 03:07:15 GMT  
		Size: 2.0 MB (2028902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2b15beced30d5d9c3217d05fbc311c702804c349cfc6760939567eae875542`  
		Last Modified: Fri, 30 Jul 2021 03:07:14 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048e8bfd206a4b157f19e4086c0a38fa289463b4ca130fd1cbd243a62fd0af41`  
		Last Modified: Fri, 30 Jul 2021 03:07:15 GMT  
		Size: 553.9 KB (553914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248ab4d9685ff88c8d035e051da298f544d1c3f057e607368dbe41aaaef785bb`  
		Last Modified: Fri, 13 Aug 2021 00:30:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63c1826c52a91bf4414b5eccd04ba9544315edb5b1a121e5e0c32c7a52bbed4`  
		Last Modified: Fri, 13 Aug 2021 00:30:43 GMT  
		Size: 19.2 MB (19182688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:1d693435ecebeaefafd7b1439861187b30a21df1565c1a432f0047f0e55da3c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.9 MB (140945339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef20e8e83f80b489a82a3f37df00c3d4805e559708381e0ef6a3827575d6ddc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

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
# Thu, 22 Jul 2021 14:48:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Jul 2021 14:48:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 14:48:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 14:48:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Jul 2021 15:10:08 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 30 Jul 2021 00:06:21 GMT
ENV PHP_VERSION=8.0.9
# Fri, 30 Jul 2021 00:06:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Fri, 30 Jul 2021 00:06:22 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Fri, 30 Jul 2021 00:06:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 30 Jul 2021 00:06:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Jul 2021 00:11:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Jul 2021 00:11:04 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 30 Jul 2021 00:11:06 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Jul 2021 00:11:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Jul 2021 00:11:08 GMT
WORKDIR /var/www/html
# Fri, 30 Jul 2021 00:11:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 30 Jul 2021 00:11:11 GMT
STOPSIGNAL SIGQUIT
# Fri, 30 Jul 2021 00:11:11 GMT
EXPOSE 9000
# Fri, 30 Jul 2021 00:11:12 GMT
CMD ["php-fpm"]
# Fri, 30 Jul 2021 03:52:52 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 30 Jul 2021 03:52:54 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 30 Jul 2021 03:52:55 GMT
COPY file:3e162edb3278a885c516d518136f3034c1eced6f4248bd3295042096c46920e3 in /usr/local/bin/ 
# Tue, 03 Aug 2021 19:00:15 GMT
ENV DRUPAL_VERSION=9.2.3
# Tue, 03 Aug 2021 19:00:15 GMT
WORKDIR /opt/drupal
# Tue, 03 Aug 2021 19:00:44 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 03 Aug 2021 19:00:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:87c6cce96c4c8171e2997feeb8b8c0be9eaf21062835c19b91b4392ec47787a5`  
		Last Modified: Fri, 30 Jul 2021 01:45:17 GMT  
		Size: 11.0 MB (10998081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd49c855913181d2d5d29258dc8b69ac7e2bf5de7213f9d0eae882cba6350bc`  
		Last Modified: Fri, 30 Jul 2021 01:45:12 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1de51663a6b2d0a9d1e24c22f57dc3cb873d8b868aed603b197afe9ec24da73`  
		Last Modified: Fri, 30 Jul 2021 01:45:28 GMT  
		Size: 26.5 MB (26473863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19443c52a976ac1ac300fa1b55c8f0b3947e0ffacadbaba9093d729767d9fc36`  
		Last Modified: Fri, 30 Jul 2021 01:45:12 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256365a94e1712e8257e57f3bb1515da0bfe2283c4bbaf569e7e2c74dd6e8534`  
		Last Modified: Fri, 30 Jul 2021 01:45:12 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733444dc312a88b5a865d2676b7e1029d51e9329e50c6228375671a8844e5c0c`  
		Last Modified: Fri, 30 Jul 2021 01:45:12 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef0b8f9995d1cc8b5d9c0ed728034d566373740f49a1a2a79a044a43ddbe549`  
		Last Modified: Fri, 30 Jul 2021 04:36:25 GMT  
		Size: 1.5 MB (1463169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0eed086ef57031b9b55cff71621ccb283b5fb45a0c88af6e607aad3b8f13a7`  
		Last Modified: Fri, 30 Jul 2021 04:36:24 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9b3c2f2b7b22ff23c2e853388c19bfdb4ecf5ef660b73a5b1f4bbf6ddfe22d`  
		Last Modified: Fri, 30 Jul 2021 04:36:25 GMT  
		Size: 553.9 KB (553919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8655d486ac34f4e3edd76992dcb20e8a664e52c316cff3dc4db417237ed6f08c`  
		Last Modified: Tue, 03 Aug 2021 19:27:38 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6692526e1ca302d80ebfac42e9f05e977125fcb84017de89a647a84e12a1db1c`  
		Last Modified: Tue, 03 Aug 2021 19:28:04 GMT  
		Size: 19.2 MB (19184242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:1b489704c660544ce6d84d29fab6de5a86aebc5191ff27bdd8d33e2f427bf54a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.3 MB (157339012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38bb568222cb3f9bf2112b9c7287a33a828e63fd7e911451d98fd665288689b8`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 07:59:53 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 22 Jul 2021 07:59:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 22 Jul 2021 08:00:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 08:00:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Jul 2021 08:00:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Jul 2021 08:10:33 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Jul 2021 08:10:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 08:10:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 08:10:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Jul 2021 08:28:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 29 Jul 2021 22:50:45 GMT
ENV PHP_VERSION=8.0.9
# Thu, 29 Jul 2021 22:50:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Thu, 29 Jul 2021 22:50:45 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Thu, 29 Jul 2021 22:50:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 29 Jul 2021 22:50:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Jul 2021 22:54:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Jul 2021 22:54:14 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Jul 2021 22:54:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Jul 2021 22:54:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Jul 2021 22:54:15 GMT
WORKDIR /var/www/html
# Thu, 29 Jul 2021 22:54:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Jul 2021 22:54:16 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Jul 2021 22:54:16 GMT
EXPOSE 9000
# Thu, 29 Jul 2021 22:54:17 GMT
CMD ["php-fpm"]
# Fri, 30 Jul 2021 01:32:01 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 30 Jul 2021 01:32:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 30 Jul 2021 01:32:02 GMT
COPY file:3e162edb3278a885c516d518136f3034c1eced6f4248bd3295042096c46920e3 in /usr/local/bin/ 
# Tue, 03 Aug 2021 18:40:42 GMT
ENV DRUPAL_VERSION=9.2.3
# Tue, 03 Aug 2021 18:40:42 GMT
WORKDIR /opt/drupal
# Tue, 03 Aug 2021 18:40:56 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 03 Aug 2021 18:40:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44bf6e1c2ffecd0cb804c5c9724b0f855bd48677407824a7b027d09146df1f0`  
		Last Modified: Thu, 22 Jul 2021 09:24:16 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b532f48bc4e6d89cb03d2540f7ae329af87d635ed865265a2023fbfe1fc232a`  
		Last Modified: Thu, 22 Jul 2021 09:24:23 GMT  
		Size: 70.4 MB (70356654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d305caec4584e49bc16aba430471ac6c8598af8fb0933c75aa4a3a4878de283`  
		Last Modified: Thu, 22 Jul 2021 09:24:11 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068e3ed6f28bf92f640f855194bc62ee46c9b7a2f87ab9162bb0c9c6c4b4d437`  
		Last Modified: Fri, 30 Jul 2021 00:14:15 GMT  
		Size: 11.0 MB (10998783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71d82b648d87bf58144bc7dd547d357b2c38a3b9871b0cdd48d869e9863e4ac`  
		Last Modified: Fri, 30 Jul 2021 00:14:11 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451efe6f008eaada9362c2355452fb28d5c983451c92a89a26f046fa06399abb`  
		Last Modified: Fri, 30 Jul 2021 00:14:18 GMT  
		Size: 28.6 MB (28633429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5228c5aaef36157a88ee01b5fee93eaa954689307bec5f3556770f5f7f310ad0`  
		Last Modified: Fri, 30 Jul 2021 00:14:12 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4f5412dc4360d14efb7f66f4379dfd547dd4f10c2566506873f3dca0396cbc`  
		Last Modified: Fri, 30 Jul 2021 00:14:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9998f149987ad808ec980adf78aa3d23a07c7fbbfcdfd6ac76502078988007`  
		Last Modified: Fri, 30 Jul 2021 00:14:11 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d32e89ab97eb5a8d1a5cb0f8428114f100c2a40403e7959cd3a3147fe03ab4e2`  
		Last Modified: Fri, 30 Jul 2021 01:53:36 GMT  
		Size: 1.7 MB (1684635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf9d38da72a483732832584efacbd973da1c391641070b6962e04b4928f0b23`  
		Last Modified: Fri, 30 Jul 2021 01:53:36 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc061583e24df60fb9ede74404b79fa8b4ef3f700137fd1cebe3b4d3fc53955f`  
		Last Modified: Fri, 30 Jul 2021 01:53:36 GMT  
		Size: 553.9 KB (553913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae245a770a2007ad3d9e21c784c9a6934407404b94d72ac2dacfbf534cf4ef`  
		Last Modified: Tue, 03 Aug 2021 18:54:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef556f60c85d207315eef6fe11eeb494a9f48c7f424c10089cae551e31b5925`  
		Last Modified: Tue, 03 Aug 2021 18:54:28 GMT  
		Size: 19.2 MB (19184255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-buster` - linux; 386

```console
$ docker pull drupal@sha256:afda49e2a56873e11b1758730a1b35cc4c184cd16f8180fc37817eb2a772b067
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.6 MB (171642867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94f203107510125c74fa1d04ea4259b00af8d3671ed08428b31213a972db5142`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 09:40:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 22 Jul 2021 09:40:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 22 Jul 2021 09:40:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 09:40:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Jul 2021 09:40:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Jul 2021 09:51:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Jul 2021 09:51:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 09:51:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 09:51:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Jul 2021 10:15:17 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 29 Jul 2021 21:01:23 GMT
ENV PHP_VERSION=8.0.9
# Thu, 29 Jul 2021 21:01:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Thu, 29 Jul 2021 21:01:24 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Thu, 29 Jul 2021 21:01:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 29 Jul 2021 21:01:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Jul 2021 21:12:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Jul 2021 21:12:57 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Jul 2021 21:12:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Jul 2021 21:12:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Jul 2021 21:13:00 GMT
WORKDIR /var/www/html
# Thu, 29 Jul 2021 21:13:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Jul 2021 21:13:02 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Jul 2021 21:13:02 GMT
EXPOSE 9000
# Thu, 29 Jul 2021 21:13:03 GMT
CMD ["php-fpm"]
# Fri, 30 Jul 2021 01:31:13 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 30 Jul 2021 01:31:15 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 30 Jul 2021 01:31:15 GMT
COPY file:f539a671699d0ee2c6a9addc1c9882f0a57e431136013791bb98020df3e6cbd3 in /usr/local/bin/ 
# Fri, 13 Aug 2021 00:39:29 GMT
ENV DRUPAL_VERSION=9.2.4
# Fri, 13 Aug 2021 00:39:29 GMT
WORKDIR /opt/drupal
# Fri, 13 Aug 2021 00:39:42 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 13 Aug 2021 00:39:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4477693d6242c3b02c6c58a73152007ec665dbcc5536c01096b6330b3f6d85`  
		Last Modified: Thu, 22 Jul 2021 12:00:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d6cc239dfcc297e081117ef07ba613b79a64337489686cc1f0c4519e7727d4`  
		Last Modified: Thu, 22 Jul 2021 12:00:45 GMT  
		Size: 81.2 MB (81230062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70703a1ba8fa6c334df3d6d7a8bba52f9df93ff417bdefa6c2cc6655f3ad5afa`  
		Last Modified: Thu, 22 Jul 2021 12:00:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecf4ffd63abe76475c0646dd56835565d245577f04cb96c9e195a935eaceab6`  
		Last Modified: Fri, 30 Jul 2021 00:13:03 GMT  
		Size: 11.0 MB (10999422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0007dc60914140f258d4cb301d1317f10e3c7972ff44354a094fe867cfc38a`  
		Last Modified: Fri, 30 Jul 2021 00:12:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd696b8760fb669f0a1fe348eb70ebfe04571595dabf20902f93e2f21e5a57`  
		Last Modified: Fri, 30 Jul 2021 00:13:07 GMT  
		Size: 29.8 MB (29772028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec4b03630be857d202e339225d90e2acc40f2ec23cd9e7b5fbcd82f49a8f5c6`  
		Last Modified: Fri, 30 Jul 2021 00:12:59 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7bbe920f86b457fa0368772bb0913eae479b34fd12723c43a4d32dab4897825`  
		Last Modified: Fri, 30 Jul 2021 00:12:59 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ebec313228f38f49a650eb9310b309f467ee674f1825354657695cb34b1b80`  
		Last Modified: Fri, 30 Jul 2021 00:12:59 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f00c4ec9397cd5d7d76dd7245eac9f74704b003dc660d3026ccb45511ea867`  
		Last Modified: Fri, 30 Jul 2021 02:03:45 GMT  
		Size: 2.1 MB (2095460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7274db9da724fe22b128e605774a93d2f7ed37c6831aca689933cf8c5c546e`  
		Last Modified: Fri, 30 Jul 2021 02:03:44 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731bdeb68e94dcabcad026cadd0938ac73f67c43370792f0320d6fd56c558003`  
		Last Modified: Fri, 30 Jul 2021 02:03:44 GMT  
		Size: 553.2 KB (553186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf2080922ae4a6b6997091c56331084a1e64f833a3a377dd09043c639978282`  
		Last Modified: Fri, 13 Aug 2021 00:56:49 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c622b49e7583b6fb4e9a889644867ab9ca3be8eca9a8e1a60a2940d23bcae562`  
		Last Modified: Fri, 13 Aug 2021 00:56:56 GMT  
		Size: 19.2 MB (19182695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-buster` - linux; ppc64le

```console
$ docker pull drupal@sha256:3f6d4bdd94e19f97a12eccebf3f522b64c4c6044b0f4afde37dcfbca2644ba61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.1 MB (176117084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:808e140c5bfbf730dcdec3d9a86a236c62882258a4961e170b57a337e8585e6e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

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
# Thu, 22 Jul 2021 12:44:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Jul 2021 12:44:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 12:45:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 12:45:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Jul 2021 13:44:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 29 Jul 2021 23:11:45 GMT
ENV PHP_VERSION=8.0.9
# Thu, 29 Jul 2021 23:11:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Thu, 29 Jul 2021 23:11:52 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Thu, 29 Jul 2021 23:12:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 29 Jul 2021 23:12:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Jul 2021 23:17:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Jul 2021 23:17:22 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Jul 2021 23:17:28 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Jul 2021 23:17:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Jul 2021 23:17:38 GMT
WORKDIR /var/www/html
# Thu, 29 Jul 2021 23:17:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Jul 2021 23:17:46 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Jul 2021 23:17:48 GMT
EXPOSE 9000
# Thu, 29 Jul 2021 23:17:52 GMT
CMD ["php-fpm"]
# Fri, 30 Jul 2021 02:17:23 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 30 Jul 2021 02:17:31 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 30 Jul 2021 02:17:36 GMT
COPY file:3e162edb3278a885c516d518136f3034c1eced6f4248bd3295042096c46920e3 in /usr/local/bin/ 
# Fri, 13 Aug 2021 02:16:44 GMT
ENV DRUPAL_VERSION=9.2.4
# Fri, 13 Aug 2021 02:16:47 GMT
WORKDIR /opt/drupal
# Fri, 13 Aug 2021 02:17:23 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 13 Aug 2021 02:17:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:3236dd2a9b464602bc56537153e425157afa1a83dbbb58bb5617dd9492668bde`  
		Last Modified: Fri, 30 Jul 2021 01:03:28 GMT  
		Size: 11.0 MB (10999933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e43bed0c824687b5a2c4f8b372601952ac591f73e848bf31f4fa97fd50d3e68a`  
		Last Modified: Fri, 30 Jul 2021 01:03:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffd57068d4d1ef2005e33d741a18ed8358981f138b74a551089f7bcc31df734`  
		Last Modified: Fri, 30 Jul 2021 01:03:29 GMT  
		Size: 30.6 MB (30587506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf4d50e00a9233fffd04bd1646358f4ef57e7fc26a70c248372a06ef406c570`  
		Last Modified: Fri, 30 Jul 2021 01:03:23 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a95e0994fe4f5d78626a55beda010ae3ce1ca638ec16a7a98cb6a4a4344459`  
		Last Modified: Fri, 30 Jul 2021 01:03:23 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca3a5e6f98140a0e09bd8f675af55e346b359be1ace9d89a8938c96eb8a381f`  
		Last Modified: Fri, 30 Jul 2021 01:03:23 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a151389b8dfb5473f2519529571da6b6189558df571878cf87f7285b87372c`  
		Last Modified: Fri, 30 Jul 2021 03:03:09 GMT  
		Size: 1.9 MB (1935912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa8ffe003a45cd03027f2bbd4f509428f057e0bd10f22d567789839ebd4e4be`  
		Last Modified: Fri, 30 Jul 2021 03:03:07 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375180b673f4e3036be0393265d4b38d051d7976e8a3c278b4558e58b0df5804`  
		Last Modified: Fri, 30 Jul 2021 03:03:07 GMT  
		Size: 553.9 KB (553919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c2a1c5cbb1b5a71d551a1b46d2bdc74f7393fde9e82d3354ec9108e171c1b77`  
		Last Modified: Fri, 13 Aug 2021 02:52:34 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302c00ec38373c2bc9deb24ac3f78c0033f810f217f7f767e62e9063c0a62547`  
		Last Modified: Fri, 13 Aug 2021 02:55:04 GMT  
		Size: 19.2 MB (19182773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-buster` - linux; s390x

```console
$ docker pull drupal@sha256:8e78fdb07535db0feca575f99ffe21ec7e340c3f671285a3c1db47835006c8f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.9 MB (150882281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfb2a1691c38be9ab9a20155ad31fbbb8565e301bb0fb8d3bdc17f37118d3905`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 06:31:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 22 Jul 2021 06:31:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 22 Jul 2021 06:31:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 06:31:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Jul 2021 06:31:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Jul 2021 06:39:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Jul 2021 06:39:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 06:39:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Jul 2021 06:39:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Jul 2021 06:57:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 29 Jul 2021 22:43:08 GMT
ENV PHP_VERSION=8.0.9
# Thu, 29 Jul 2021 22:43:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Thu, 29 Jul 2021 22:43:09 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Thu, 29 Jul 2021 22:43:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 29 Jul 2021 22:43:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Jul 2021 22:46:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Jul 2021 22:46:05 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 29 Jul 2021 22:46:06 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Jul 2021 22:46:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Jul 2021 22:46:06 GMT
WORKDIR /var/www/html
# Thu, 29 Jul 2021 22:46:07 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Jul 2021 22:46:07 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Jul 2021 22:46:07 GMT
EXPOSE 9000
# Thu, 29 Jul 2021 22:46:08 GMT
CMD ["php-fpm"]
# Fri, 30 Jul 2021 03:26:29 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 30 Jul 2021 03:26:31 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 30 Jul 2021 03:26:31 GMT
COPY file:3e162edb3278a885c516d518136f3034c1eced6f4248bd3295042096c46920e3 in /usr/local/bin/ 
# Fri, 13 Aug 2021 03:14:52 GMT
ENV DRUPAL_VERSION=9.2.4
# Fri, 13 Aug 2021 03:14:52 GMT
WORKDIR /opt/drupal
# Fri, 13 Aug 2021 03:15:19 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 13 Aug 2021 03:15:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e14906a92e7864b1de2aa3cd4a352a34fa76fa8507adcbbe0cb5b7e798c5c8`  
		Last Modified: Thu, 22 Jul 2021 08:41:43 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657542f864cdb34d7361833d34fce13e1ed95e90ab57449c83457cee81caf6f9`  
		Last Modified: Thu, 22 Jul 2021 08:41:53 GMT  
		Size: 64.7 MB (64710955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4454013019daddacaf9fc30a9b52c6039ca76ecf89ea7dc520fac7a072eab8a4`  
		Last Modified: Thu, 22 Jul 2021 08:41:43 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf75402d174805cb17b691af87c82af87fe418ea706f03b688be9f802cea0a6`  
		Last Modified: Fri, 30 Jul 2021 00:20:18 GMT  
		Size: 11.0 MB (10998314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d445bbc1c5f19c7985be5304c259aa4697be144ae224d7915eb56a8f1553d847`  
		Last Modified: Fri, 30 Jul 2021 00:20:13 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed59274e4f243f151c51f908b7ef5debba4d0926ba1d2330cd58cb17e8a6610f`  
		Last Modified: Fri, 30 Jul 2021 00:20:18 GMT  
		Size: 28.0 MB (27986679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fcf8e629b0ef862f3cc445235d3bd30a80afee751c1ddb3d41810ee3ba335f`  
		Last Modified: Fri, 30 Jul 2021 00:20:13 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175221a02bf30cf15f7627281e736e54f557289e2316dcb5d370440da37c855a`  
		Last Modified: Fri, 30 Jul 2021 00:20:13 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea86522153dfc1e7c19632dcaabdbd9b0c9fc28e28284e7e483df6d0905a2e35`  
		Last Modified: Fri, 30 Jul 2021 00:20:13 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740535d92e28ef8af27174c1265a8d5fd720d87885f73e53fa9f47b19f3d9317`  
		Last Modified: Fri, 30 Jul 2021 03:55:42 GMT  
		Size: 1.7 MB (1676466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac53816999f7e1820de4e1309b93a4470770c4725274672456d15c9b07e55591`  
		Last Modified: Fri, 30 Jul 2021 03:55:42 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae7f3d5a8ee71a7e8f57dfd15e29d526578ea619e3e2ef389b02c60b11931ca`  
		Last Modified: Fri, 30 Jul 2021 03:55:42 GMT  
		Size: 553.9 KB (553918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af05b889f2f4dbb41ff4ca5fda255138d2eea94010674b05a9616c603135bc6`  
		Last Modified: Fri, 13 Aug 2021 03:36:00 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa54738305ef154379cc0c18c004b291f279d1a4ef14d8c60ea88cffadd781a`  
		Last Modified: Fri, 13 Aug 2021 03:36:04 GMT  
		Size: 19.2 MB (19182641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
