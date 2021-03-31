## `phpmyadmin:5-apache`

```console
$ docker pull phpmyadmin@sha256:00de8b38856a5f9eaf826e3838a64f3c6ce8f71c82ab4bfe6876a806a07fb8cc
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

### `phpmyadmin:5-apache` - linux; amd64

```console
$ docker pull phpmyadmin@sha256:bc4fa20bdaf2c52b0b2a58528bd08489f42e59fffcdb0da9e2ddcbeb760aff0a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.0 MB (163968801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622471936dcc84495fc62a938972030baa604d86df86b95c8f15662d625442c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:59 GMT
ADD file:b2085f4b0a7cb0e5754874c712254e5cd941062b27b8d7ed2080520196b91597 in / 
# Fri, 26 Mar 2021 15:20:59 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 06:55:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 27 Mar 2021 06:55:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 27 Mar 2021 06:55:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 06:55:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 27 Mar 2021 06:55:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 27 Mar 2021 07:04:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 27 Mar 2021 07:04:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 27 Mar 2021 07:04:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 27 Mar 2021 07:04:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 27 Mar 2021 07:04:22 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 27 Mar 2021 07:04:22 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 27 Mar 2021 07:04:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 27 Mar 2021 07:04:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 27 Mar 2021 07:04:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 27 Mar 2021 07:04:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 27 Mar 2021 07:33:00 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 27 Mar 2021 07:33:00 GMT
ENV PHP_VERSION=7.4.16
# Sat, 27 Mar 2021 07:33:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Sat, 27 Mar 2021 07:33:01 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Sat, 27 Mar 2021 07:33:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 27 Mar 2021 07:33:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 27 Mar 2021 07:37:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 27 Mar 2021 07:37:21 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Sat, 27 Mar 2021 07:37:22 GMT
RUN docker-php-ext-enable sodium
# Sat, 27 Mar 2021 07:37:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 27 Mar 2021 07:37:22 GMT
STOPSIGNAL SIGWINCH
# Sat, 27 Mar 2021 07:37:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 27 Mar 2021 07:37:22 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 07:37:23 GMT
EXPOSE 80
# Sat, 27 Mar 2021 07:37:23 GMT
CMD ["apache2-foreground"]
# Sun, 28 Mar 2021 00:25:41 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 28 Mar 2021 00:25:42 GMT
ENV MAX_EXECUTION_TIME=600
# Sun, 28 Mar 2021 00:25:42 GMT
ENV MEMORY_LIMIT=512M
# Sun, 28 Mar 2021 00:25:42 GMT
ENV UPLOAD_LIMIT=2048K
# Sun, 28 Mar 2021 00:25:43 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Sun, 28 Mar 2021 00:25:43 GMT
ENV VERSION=5.1.0
# Sun, 28 Mar 2021 00:25:43 GMT
ENV SHA256=aa8ccf357f672012384df34e1c2bc70147476761c8458a0dad6233497e142c68
# Sun, 28 Mar 2021 00:25:43 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.1.0/phpMyAdmin-5.1.0-all-languages.tar.xz
# Sun, 28 Mar 2021 00:25:44 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.1.0 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Sun, 28 Mar 2021 00:25:55 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 28 Mar 2021 00:25:55 GMT
COPY file:74e988fef607090521e63cea57b4c61ab22b3a2a131bc55f0cf4a0d9c36ce65d in /etc/phpmyadmin/config.inc.php 
# Sun, 28 Mar 2021 00:25:55 GMT
COPY file:7a1864d35a5b72dc75fa085c7d09497f417e1ef1eacb8597037c366f1978b5fa in /docker-entrypoint.sh 
# Sun, 28 Mar 2021 00:25:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 28 Mar 2021 00:25:56 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ac2522cc72690febc428fb46fb39a4efc5e0a721c3ad15d9992b01515f2fad1a`  
		Last Modified: Fri, 26 Mar 2021 15:27:47 GMT  
		Size: 27.1 MB (27100996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2eaf06d6cfffe0634040e22cc100be8198afa930907ee33c6b1cf753d980c0`  
		Last Modified: Sat, 27 Mar 2021 08:31:10 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353d7ace7314deb5de3d34a7c84e322bac00c0a20ff52026898b2e811b15ad0b`  
		Last Modified: Sat, 27 Mar 2021 08:31:33 GMT  
		Size: 76.7 MB (76678510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e4975b15a36c02725af1642db3e9b5a72fd2486fcc8b6ef24a0c5c4c218b3d`  
		Last Modified: Sat, 27 Mar 2021 08:31:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54c541ce8eaa257ffddab7f695007d4df10b470316ee132152a20523cefc323`  
		Last Modified: Sat, 27 Mar 2021 08:32:30 GMT  
		Size: 18.7 MB (18679266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5f70c3328b938319063decdc1d0d1d76daf62f9cc278c22880241e5ba39def`  
		Last Modified: Sat, 27 Mar 2021 08:32:27 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7721d733906f3d3ab586f2793ac11f40613d0acc2aafb32edd1f07ae806d3e0a`  
		Last Modified: Sat, 27 Mar 2021 08:32:27 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a49155542c3c40152fd52f6abaca1f8e683df0efe618fa4907522faa2815a1`  
		Last Modified: Sat, 27 Mar 2021 08:35:32 GMT  
		Size: 10.7 MB (10672024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a365bc9f6befce77babdcf4e1e54050612ce8f20bbf17cd57091754a571cf80a`  
		Last Modified: Sat, 27 Mar 2021 08:35:29 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a4e47167a59506209f1985111483cac0e4047602dab8b0aa80dc9bbea7635d`  
		Last Modified: Sat, 27 Mar 2021 08:35:32 GMT  
		Size: 13.8 MB (13833356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b65d3ed44fc1daf65467c634a00ea1b0c18ad1a08897a9a6bc668ad7f6edaf`  
		Last Modified: Sat, 27 Mar 2021 08:35:29 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1e61773eb855ffc418cb68bce51a7106c6dccf747d9356c79673fcc0ae29e8`  
		Last Modified: Sat, 27 Mar 2021 08:35:29 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29159fb4bccbc7edddad426d438ac97c6e67fe84dfbc9376f92fdbbe698a6c6`  
		Last Modified: Sat, 27 Mar 2021 08:35:29 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb2ad0cd25048546a2680a59199bb1ae9eb78c401f7f6dbed6c474159161bec`  
		Last Modified: Sun, 28 Mar 2021 00:27:20 GMT  
		Size: 2.9 MB (2900526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724c2094fd988fd93c7a0b3ecbbabc5ea5ee85fc6b0f0f634554b4e3430e7a6`  
		Last Modified: Sun, 28 Mar 2021 00:27:20 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74d3d7cd27f7d101782331da8b9f25f88eaf18ef0c0cc663103294bfad3555c`  
		Last Modified: Sun, 28 Mar 2021 00:27:24 GMT  
		Size: 14.1 MB (14095878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23c2a81bcd47a73dcd96e0e6e0c482cf10c7f18f765ddccc0489896f7a94f14`  
		Last Modified: Sun, 28 Mar 2021 00:27:22 GMT  
		Size: 1.5 KB (1528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4438038ef379af0457c52062dcdd7fde2761cf3d005350822f7d0509699c0fb9`  
		Last Modified: Sun, 28 Mar 2021 00:27:20 GMT  
		Size: 772.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-apache` - linux; arm variant v5

```console
$ docker pull phpmyadmin@sha256:5446b9a14a7de8f69ccc5b1cdc08912981972b81915867346008d01f756e070e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.1 MB (142086516 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37bfc0bc6bf4ef28a8247c81774d1da3db3d71e07281ee4912b9642d2f682347`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 30 Mar 2021 21:51:08 GMT
ADD file:779165b34b3be18f6c24e448997bf6497e3b27ff72954fe3cdced0ebcc77b6b8 in / 
# Tue, 30 Mar 2021 21:51:11 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:16:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 31 Mar 2021 00:16:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 31 Mar 2021 00:16:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:16:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 00:16:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 00:21:39 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 31 Mar 2021 00:21:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 31 Mar 2021 00:22:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 31 Mar 2021 00:22:14 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 31 Mar 2021 00:22:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 31 Mar 2021 00:22:17 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 31 Mar 2021 00:22:18 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 31 Mar 2021 00:22:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:22:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:22:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 00:39:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 00:39:11 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 00:39:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 00:39:13 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 00:39:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 00:39:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:42:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 00:42:49 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:42:58 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 00:42:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 00:43:00 GMT
STOPSIGNAL SIGWINCH
# Wed, 31 Mar 2021 00:43:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:43:03 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 00:43:03 GMT
EXPOSE 80
# Wed, 31 Mar 2021 00:43:05 GMT
CMD ["apache2-foreground"]
# Wed, 31 Mar 2021 13:27:34 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:27:35 GMT
ENV MAX_EXECUTION_TIME=600
# Wed, 31 Mar 2021 13:27:35 GMT
ENV MEMORY_LIMIT=512M
# Wed, 31 Mar 2021 13:27:36 GMT
ENV UPLOAD_LIMIT=2048K
# Wed, 31 Mar 2021 13:27:38 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Wed, 31 Mar 2021 13:27:40 GMT
ENV VERSION=5.1.0
# Wed, 31 Mar 2021 13:27:40 GMT
ENV SHA256=aa8ccf357f672012384df34e1c2bc70147476761c8458a0dad6233497e142c68
# Wed, 31 Mar 2021 13:27:41 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.1.0/phpMyAdmin-5.1.0-all-languages.tar.xz
# Wed, 31 Mar 2021 13:27:43 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.1.0 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Wed, 31 Mar 2021 13:28:18 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:28:20 GMT
COPY file:74e988fef607090521e63cea57b4c61ab22b3a2a131bc55f0cf4a0d9c36ce65d in /etc/phpmyadmin/config.inc.php 
# Wed, 31 Mar 2021 13:28:21 GMT
COPY file:7a1864d35a5b72dc75fa085c7d09497f417e1ef1eacb8597037c366f1978b5fa in /docker-entrypoint.sh 
# Wed, 31 Mar 2021 13:28:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 31 Mar 2021 13:28:24 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:7cbaf854daf876ddd338771dec41777b0dfcad33c1fc8ea3512a0708333e4465`  
		Last Modified: Tue, 30 Mar 2021 21:58:44 GMT  
		Size: 24.9 MB (24873214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae61257e71ed1fe36dd059766677f4a537b356c6fc540a3ca4ba7402f6f3d590`  
		Last Modified: Wed, 31 Mar 2021 01:29:10 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe994f5a2a99df2b5e9f78688bf4a0a7da6f65bbcc6a46c31e2b096ce25c012f`  
		Last Modified: Wed, 31 Mar 2021 01:29:35 GMT  
		Size: 58.8 MB (58815883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9eca09f3156e497ec384a401521d8dc49d572b779a60298cad4e6929d8f38aa`  
		Last Modified: Wed, 31 Mar 2021 01:29:09 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0225a634d639e6a59e6adc3e3db8addca7af5f10689a5e112480c3097749e48`  
		Last Modified: Wed, 31 Mar 2021 01:30:19 GMT  
		Size: 18.0 MB (18026259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ad8888e12bd76fd2c37d8c477098a1970f5377c9b442874bfdb90784ff1e38`  
		Last Modified: Wed, 31 Mar 2021 01:30:14 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a423f61452f9bd99e76e9d663ab623d7d467756799695c922e9727637a154d9a`  
		Last Modified: Wed, 31 Mar 2021 01:30:14 GMT  
		Size: 520.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01707d42999aa808ea2c319efd471e6dfd14f197ac6607e266168c071fd8d3e`  
		Last Modified: Wed, 31 Mar 2021 01:32:27 GMT  
		Size: 10.7 MB (10670339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6a34945beb76dbb8dd2672df2857396045acdbfa08e133a611c1e6ad3b414a`  
		Last Modified: Wed, 31 Mar 2021 01:32:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9169440779c7906cc0180731afc03aad9d0f9d2da43dc945ed7dd2b448f321`  
		Last Modified: Wed, 31 Mar 2021 01:32:30 GMT  
		Size: 12.9 MB (12922510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f51bfaeb057d9a41cbbddd95f825fe01ea0842f02f243ab2517ee6fffa884fc`  
		Last Modified: Wed, 31 Mar 2021 01:32:24 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de55dc42e6154d3893b44d3bb1cdf684748349f791f9fd293b90b4e2ac2f17f4`  
		Last Modified: Wed, 31 Mar 2021 01:32:24 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff47c8ca10fdc42954faba885ae1ffc238b887f18920cc65050f0ed0019eb9b1`  
		Last Modified: Wed, 31 Mar 2021 01:32:25 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f529ed18c4e7c46c1f6264fe8e1c7833883438b91e0acdb5695b629ef88421e`  
		Last Modified: Wed, 31 Mar 2021 13:32:00 GMT  
		Size: 2.7 MB (2679206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aa52f5aa7082e44379fef495e9b7ae7a9f2a83042b419c110558933ac91a0e`  
		Last Modified: Wed, 31 Mar 2021 13:31:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc520586894d3fc3042b7dff8c65760e5b5379b2a96f64bce0a53bb8bc3986b`  
		Last Modified: Wed, 31 Mar 2021 13:32:06 GMT  
		Size: 14.1 MB (14090846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbb0a6300394e771f7d0e38725719cca6afc6be6bf27da9d760c1a4b30067fd`  
		Last Modified: Wed, 31 Mar 2021 13:32:00 GMT  
		Size: 1.5 KB (1531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfe2c04f36b432762d98b317feb2515e36ee12be1c89a389dc93d2c76717c1e`  
		Last Modified: Wed, 31 Mar 2021 13:31:59 GMT  
		Size: 772.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-apache` - linux; arm variant v7

```console
$ docker pull phpmyadmin@sha256:bb08ef1c12249738a9731755b76cf3e3fee3a115331f9a12aa348843ed63b6ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.2 MB (139213925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e02ad22b4a09240090a8d71a7da6f9d62bf3c1d303baf54d06760dd6ab9eb151`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 26 Mar 2021 11:17:38 GMT
ADD file:911acc83e6d3d4b00ecc59effce9e5ab69d62aa3e77a24db76e270db8cedce5f in / 
# Fri, 26 Mar 2021 11:17:39 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:19:04 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 26 Mar 2021 18:19:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 26 Mar 2021 18:19:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:19:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 26 Mar 2021 18:19:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 26 Mar 2021 18:23:49 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Fri, 26 Mar 2021 18:23:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Fri, 26 Mar 2021 18:24:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Fri, 26 Mar 2021 18:24:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Fri, 26 Mar 2021 18:24:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Fri, 26 Mar 2021 18:24:20 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Fri, 26 Mar 2021 18:24:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Fri, 26 Mar 2021 18:24:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 18:24:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 18:24:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Mar 2021 18:39:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 26 Mar 2021 18:39:08 GMT
ENV PHP_VERSION=7.4.16
# Fri, 26 Mar 2021 18:39:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Fri, 26 Mar 2021 18:39:10 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Fri, 26 Mar 2021 18:39:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 26 Mar 2021 18:39:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:42:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 18:42:05 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:42:11 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 18:42:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 18:42:15 GMT
STOPSIGNAL SIGWINCH
# Fri, 26 Mar 2021 18:42:15 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:42:17 GMT
WORKDIR /var/www/html
# Fri, 26 Mar 2021 18:42:19 GMT
EXPOSE 80
# Fri, 26 Mar 2021 18:42:20 GMT
CMD ["apache2-foreground"]
# Sat, 27 Mar 2021 14:42:41 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 14:42:42 GMT
ENV MAX_EXECUTION_TIME=600
# Sat, 27 Mar 2021 14:42:43 GMT
ENV MEMORY_LIMIT=512M
# Sat, 27 Mar 2021 14:42:44 GMT
ENV UPLOAD_LIMIT=2048K
# Sat, 27 Mar 2021 14:42:48 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Sat, 27 Mar 2021 14:42:50 GMT
ENV VERSION=5.1.0
# Sat, 27 Mar 2021 14:42:53 GMT
ENV SHA256=aa8ccf357f672012384df34e1c2bc70147476761c8458a0dad6233497e142c68
# Sat, 27 Mar 2021 14:42:55 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.1.0/phpMyAdmin-5.1.0-all-languages.tar.xz
# Sat, 27 Mar 2021 14:42:55 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.1.0 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Sat, 27 Mar 2021 14:43:23 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 14:43:25 GMT
COPY file:74e988fef607090521e63cea57b4c61ab22b3a2a131bc55f0cf4a0d9c36ce65d in /etc/phpmyadmin/config.inc.php 
# Sat, 27 Mar 2021 14:43:26 GMT
COPY file:7a1864d35a5b72dc75fa085c7d09497f417e1ef1eacb8597037c366f1978b5fa in /docker-entrypoint.sh 
# Sat, 27 Mar 2021 14:43:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 27 Mar 2021 14:43:27 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:05a8be0db5eb6dbb349e49a01211d3a11adc23881f696760a058c0c8ae8e39b7`  
		Last Modified: Fri, 26 Mar 2021 11:27:34 GMT  
		Size: 22.7 MB (22709509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d28c0b6fab1499bb2c7612e43e400e80dd01221d80304b2314e6fae3122d16`  
		Last Modified: Fri, 26 Mar 2021 19:24:07 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750c9e4cb128bf48dda1dcb9cf167ad2a67b9d8b8f561a7b1d2ad81622a67850`  
		Last Modified: Fri, 26 Mar 2021 19:24:28 GMT  
		Size: 59.5 MB (59512646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629683649fade51a76c161487a63561cfefa29a345b8815f66673ebda404501c`  
		Last Modified: Fri, 26 Mar 2021 19:24:07 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402275acac7e1772b37a2232d7a761f88e14ecc7f2ba6d4b01863b25fc7e10ba`  
		Last Modified: Fri, 26 Mar 2021 19:25:10 GMT  
		Size: 17.5 MB (17481694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c1f324afe558d1c68590950b835a6a4eaa2be30dbd3bda021dbacbbae98479`  
		Last Modified: Fri, 26 Mar 2021 19:25:02 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622ec2b77047b7e5be79ec6cbbc4c32eb4df21f0fa102b2baeb1850d2c651651`  
		Last Modified: Fri, 26 Mar 2021 19:25:02 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d2c18982f446b5e0b95c7abbd0d4ce4cdb16970a5c3aba482f99ff353a2b09`  
		Last Modified: Fri, 26 Mar 2021 19:27:31 GMT  
		Size: 10.7 MB (10670285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef5b7a01847030642616eda9f6677a25cef0b8613f4fd65d9751c1d0673a713`  
		Last Modified: Fri, 26 Mar 2021 19:27:27 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d238e402eed46f7b5fdc045b63d5726fdc304ce77fe788729faca39cb2949d22`  
		Last Modified: Fri, 26 Mar 2021 19:27:33 GMT  
		Size: 12.2 MB (12219154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a82bc0a55c8f373a2b489dae843e17a00da56ef34da23c15304cbe85a728d0`  
		Last Modified: Fri, 26 Mar 2021 19:27:27 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ddeb7fc5608cf9369d758e8707fc8cd7bc8cb89e83c0ce40e2141e0704c82a`  
		Last Modified: Fri, 26 Mar 2021 19:27:27 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378655f0a6210353369dd85e94024c86c5037e1c08403beb56607ec82b83a09f`  
		Last Modified: Fri, 26 Mar 2021 19:27:27 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bc00040e54780bd40a22fc2f12f8207821caccf66eb1eabb975f53637fa491`  
		Last Modified: Sat, 27 Mar 2021 14:46:39 GMT  
		Size: 2.5 MB (2521902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df001d5c3577dd106b90d32bf5a4e4581b5b53ff4c17ae3317a1a504ccd67e9`  
		Last Modified: Sat, 27 Mar 2021 14:46:38 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0896f260e57c0f74bd2c8a2ea567fd7aaf48cac55db31bdb2b0a475ab5523dfc`  
		Last Modified: Sat, 27 Mar 2021 14:46:45 GMT  
		Size: 14.1 MB (14090490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35004c4d628678008a54571232ad0b65765d3efdb1aea60dddd9ad00afa6f6b9`  
		Last Modified: Sat, 27 Mar 2021 14:46:38 GMT  
		Size: 1.5 KB (1528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c459ffbe56060d01339b5915e9df724ee8528aa13062da98994a5183927a4a1`  
		Last Modified: Sat, 27 Mar 2021 14:46:38 GMT  
		Size: 772.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-apache` - linux; arm64 variant v8

```console
$ docker pull phpmyadmin@sha256:c46bce3e47676b556a8b16f396c72bcd7e391829194719eec16954840a2e3c63
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.0 MB (156021548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60d6c450e654a507e846d6458ebea4ced7fceb441933f6c030e048374255b841`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:54 GMT
ADD file:c8c0d923527574a26725e0a1995051870ed169ff6b6ebfe77c50810f5583690b in / 
# Fri, 26 Mar 2021 15:41:56 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 05:39:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 27 Mar 2021 05:39:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 27 Mar 2021 05:39:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 05:40:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 27 Mar 2021 05:40:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 27 Mar 2021 05:44:17 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 27 Mar 2021 05:44:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 27 Mar 2021 05:44:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 27 Mar 2021 05:44:40 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 27 Mar 2021 05:44:42 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 27 Mar 2021 05:44:43 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 27 Mar 2021 05:44:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 27 Mar 2021 05:44:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 27 Mar 2021 05:44:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 27 Mar 2021 05:44:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 27 Mar 2021 06:01:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 27 Mar 2021 06:01:08 GMT
ENV PHP_VERSION=7.4.16
# Sat, 27 Mar 2021 06:01:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Sat, 27 Mar 2021 06:01:09 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Sat, 27 Mar 2021 06:01:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 27 Mar 2021 06:01:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 27 Mar 2021 06:04:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 27 Mar 2021 06:04:24 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Sat, 27 Mar 2021 06:04:27 GMT
RUN docker-php-ext-enable sodium
# Sat, 27 Mar 2021 06:04:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 27 Mar 2021 06:04:28 GMT
STOPSIGNAL SIGWINCH
# Sat, 27 Mar 2021 06:04:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 27 Mar 2021 06:04:30 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 06:04:31 GMT
EXPOSE 80
# Sat, 27 Mar 2021 06:04:32 GMT
CMD ["apache2-foreground"]
# Sun, 28 Mar 2021 01:45:17 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 28 Mar 2021 01:45:18 GMT
ENV MAX_EXECUTION_TIME=600
# Sun, 28 Mar 2021 01:45:19 GMT
ENV MEMORY_LIMIT=512M
# Sun, 28 Mar 2021 01:45:19 GMT
ENV UPLOAD_LIMIT=2048K
# Sun, 28 Mar 2021 01:45:21 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Sun, 28 Mar 2021 01:45:22 GMT
ENV VERSION=5.1.0
# Sun, 28 Mar 2021 01:45:23 GMT
ENV SHA256=aa8ccf357f672012384df34e1c2bc70147476761c8458a0dad6233497e142c68
# Sun, 28 Mar 2021 01:45:23 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.1.0/phpMyAdmin-5.1.0-all-languages.tar.xz
# Sun, 28 Mar 2021 01:45:24 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.1.0 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Sun, 28 Mar 2021 01:45:47 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 28 Mar 2021 01:45:48 GMT
COPY file:74e988fef607090521e63cea57b4c61ab22b3a2a131bc55f0cf4a0d9c36ce65d in /etc/phpmyadmin/config.inc.php 
# Sun, 28 Mar 2021 01:45:49 GMT
COPY file:7a1864d35a5b72dc75fa085c7d09497f417e1ef1eacb8597037c366f1978b5fa in /docker-entrypoint.sh 
# Sun, 28 Mar 2021 01:45:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 28 Mar 2021 01:45:51 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:989f98f7e44fde3e2eb49bc6d2bfed15401201d21cd90f42cd9fc4c26eef8bb0`  
		Last Modified: Fri, 26 Mar 2021 15:48:47 GMT  
		Size: 25.9 MB (25856384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b416b7b614ed8fceb6b3c6ff1736bd4150e20019a953020a2bd036841b2414c`  
		Last Modified: Sat, 27 Mar 2021 06:47:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ee2b6f075269bc86b1fba704b10e5eb69756b5b1ef041f9db5b3b80b318a5f`  
		Last Modified: Sat, 27 Mar 2021 06:48:10 GMT  
		Size: 70.4 MB (70355779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db2456a117cc41ec71f5b78f38e147a20bace1644f1b7484165144ebd93f3b3`  
		Last Modified: Sat, 27 Mar 2021 06:47:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cadd0e834888125ff424ee4dfe68a9c25f81da27239b74219083f6079a654c7`  
		Last Modified: Sat, 27 Mar 2021 06:48:43 GMT  
		Size: 18.6 MB (18579966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74681577fb4f6076646ab1619082abe87f6dd60a6339e9dd3748bba8e5920bb9`  
		Last Modified: Sat, 27 Mar 2021 06:48:38 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2056198c1bf0f69ce29faae9902a7f1c31aa69084fd2ecef8d07bbbb8e260cb`  
		Last Modified: Sat, 27 Mar 2021 06:48:39 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc5a4bb40006ddc0c1b7b22a710e8d103345dad12e4a41b3af750156509fa1d3`  
		Last Modified: Sat, 27 Mar 2021 06:50:33 GMT  
		Size: 10.7 MB (10670840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3fd0187a51d2204d366028f31236bcc6abcab43b419d719ebd129a8414ead0`  
		Last Modified: Sat, 27 Mar 2021 06:50:30 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca3385d750eb9125b18a6226b8cbcf8c9c8ee7aa735a1b3db77432fe648b7f82`  
		Last Modified: Sat, 27 Mar 2021 06:50:34 GMT  
		Size: 13.6 MB (13611181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b86c945b5b99c2b0604790e6c68d0dfe8d061e5668a45952c5e2151020e514`  
		Last Modified: Sat, 27 Mar 2021 06:50:30 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1efc63e4cbf186300ef5e36c2c2b254fd5f9d4dd05db223ed56722241ec9d4`  
		Last Modified: Sat, 27 Mar 2021 06:50:31 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667ae615a60de904a176bb061501cd05b79171bd59eabef8b0b8bba8719b3f3`  
		Last Modified: Sat, 27 Mar 2021 06:50:30 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e635124b5ad0b4b1c400fb77ebb5cb802b27c931f5f190976c78a0bf3a4023`  
		Last Modified: Sun, 28 Mar 2021 01:48:33 GMT  
		Size: 2.8 MB (2846240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd871f7e2199dc3218409222fc1ab7971dafc075ceb891b3d38ca7e027563f1`  
		Last Modified: Sun, 28 Mar 2021 01:48:32 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3aaf16031939e7336d5138ef1e47f0149030080bb02d61e9451ff9f0eb9122b`  
		Last Modified: Sun, 28 Mar 2021 01:48:37 GMT  
		Size: 14.1 MB (14092908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a82516e0c4d538bcd5620951986f7d1faeadb99e2e9178f3558b7f4469114c6`  
		Last Modified: Sun, 28 Mar 2021 01:48:32 GMT  
		Size: 1.5 KB (1528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b8fc7640f9c80873c6ec3e0cef218b17df1af83aba0dfbbdf2e1ec1959060b`  
		Last Modified: Sun, 28 Mar 2021 01:48:32 GMT  
		Size: 772.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-apache` - linux; 386

```console
$ docker pull phpmyadmin@sha256:cd0b06eff6518ddebf2c3d0467d2f27d6812f0717a4c1fa4b94af45305e6afb5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.1 MB (170101728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30d896b5df2d704409ce6169c9619b532749f10b05b856084b4aac154b6e546`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:48 GMT
ADD file:d11c47560c0a88a83a3a0ce5af82fc17a07075e877293e4f922f126959810ea3 in / 
# Tue, 30 Mar 2021 21:39:49 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 05:38:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 31 Mar 2021 05:38:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 31 Mar 2021 05:39:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 05:39:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 05:39:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 05:44:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 31 Mar 2021 05:44:41 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 31 Mar 2021 05:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 31 Mar 2021 05:44:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 31 Mar 2021 05:44:54 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 31 Mar 2021 05:44:54 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 31 Mar 2021 05:44:54 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 31 Mar 2021 05:44:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 05:44:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 05:44:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 06:05:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 06:05:22 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 06:05:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 06:05:23 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 06:05:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 06:05:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 06:10:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 06:10:28 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Wed, 31 Mar 2021 06:10:29 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 06:10:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 06:10:29 GMT
STOPSIGNAL SIGWINCH
# Wed, 31 Mar 2021 06:10:29 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 31 Mar 2021 06:10:30 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 06:10:30 GMT
EXPOSE 80
# Wed, 31 Mar 2021 06:10:30 GMT
CMD ["apache2-foreground"]
# Wed, 31 Mar 2021 17:03:53 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 17:03:54 GMT
ENV MAX_EXECUTION_TIME=600
# Wed, 31 Mar 2021 17:03:54 GMT
ENV MEMORY_LIMIT=512M
# Wed, 31 Mar 2021 17:03:54 GMT
ENV UPLOAD_LIMIT=2048K
# Wed, 31 Mar 2021 17:03:55 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Wed, 31 Mar 2021 17:03:56 GMT
ENV VERSION=5.1.0
# Wed, 31 Mar 2021 17:03:56 GMT
ENV SHA256=aa8ccf357f672012384df34e1c2bc70147476761c8458a0dad6233497e142c68
# Wed, 31 Mar 2021 17:03:56 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.1.0/phpMyAdmin-5.1.0-all-languages.tar.xz
# Wed, 31 Mar 2021 17:03:56 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.1.0 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Wed, 31 Mar 2021 17:04:15 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 17:04:16 GMT
COPY file:74e988fef607090521e63cea57b4c61ab22b3a2a131bc55f0cf4a0d9c36ce65d in /etc/phpmyadmin/config.inc.php 
# Wed, 31 Mar 2021 17:04:16 GMT
COPY file:7a1864d35a5b72dc75fa085c7d09497f417e1ef1eacb8597037c366f1978b5fa in /docker-entrypoint.sh 
# Wed, 31 Mar 2021 17:04:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 31 Mar 2021 17:04:16 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:548dde0830bd6b881c0c068db5a4e39aa720d2a0c5ac3897296a023dda7b3391`  
		Last Modified: Tue, 30 Mar 2021 21:46:41 GMT  
		Size: 27.8 MB (27788996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98b67b2c4467eacf10bfe3c2eef4cb9d9dc040023f3562413a987120aa2b38c`  
		Last Modified: Wed, 31 Mar 2021 07:32:04 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398a2808bbaf89e86620a60aae2b88361cd9f03abd0f3e9b04b43ddf645bbc2e`  
		Last Modified: Wed, 31 Mar 2021 07:32:39 GMT  
		Size: 81.2 MB (81230040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409fe28765e314abeb61d6d24aeacc128e934cb1bea417f77e92842b06f368ca`  
		Last Modified: Wed, 31 Mar 2021 07:32:03 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fdef2e85fbb8926daadce6771eec940814020940a21a91347c618923055b6c`  
		Last Modified: Wed, 31 Mar 2021 07:34:00 GMT  
		Size: 19.1 MB (19114939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2edb0fc5fd93f16011b981cc964f1ce3e984470528dfcb542642bfda4529929`  
		Last Modified: Wed, 31 Mar 2021 07:33:54 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59803048ef999597656449dfe53b712c8070c7c03ddaad612f72ce3134ced7e`  
		Last Modified: Wed, 31 Mar 2021 07:33:54 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77866575e1085621e2c36e025c165298b2ee51c112acda589d58e209adcb04d1`  
		Last Modified: Wed, 31 Mar 2021 07:38:36 GMT  
		Size: 10.7 MB (10671361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fd41613fecb572e1151bc7adcb1692c0a7073af72bcf9e5e744bab32898e5d`  
		Last Modified: Wed, 31 Mar 2021 07:38:30 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aff27841cd925275a632ba6c5759207fc87d7c9b91ef825d9e9392453cec446`  
		Last Modified: Wed, 31 Mar 2021 07:38:37 GMT  
		Size: 14.2 MB (14168826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291ec9b416fd42eab7f4a1d93c799fb3cd402d380cb18cdaa3b5bd743f6bad1b`  
		Last Modified: Wed, 31 Mar 2021 07:38:34 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c82c8faf191a882cece952391671f4b20dd58fadf9af05cefac4e4afb628fe0`  
		Last Modified: Wed, 31 Mar 2021 07:38:31 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3074b4d2bf65c7d6c3cb6934c06be1ff9aa9b453bf62ec77090862b7fb31d93f`  
		Last Modified: Wed, 31 Mar 2021 07:38:30 GMT  
		Size: 891.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f0330238fcfe5a95a2a035928be635fba175cb58ad7dbce4b648eec3e781d1`  
		Last Modified: Wed, 31 Mar 2021 17:07:58 GMT  
		Size: 3.0 MB (3025033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d4fca2c251008f2eac31a1115701bb0b79554ced9638d9a9e1ef05116c0ea9`  
		Last Modified: Wed, 31 Mar 2021 17:07:56 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0b70b47e5a8f8f7d557178725e0080296bcc8d89b72bb7acb67ee5638a3ebf`  
		Last Modified: Wed, 31 Mar 2021 17:08:06 GMT  
		Size: 14.1 MB (14094311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828712afbedbd160186b7d16b5d3b08c7b583a056b27adee7ec4163d41afdc8a`  
		Last Modified: Wed, 31 Mar 2021 17:07:56 GMT  
		Size: 1.5 KB (1527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4daa3c3821e88591cd42ca68d1b746b17b31c1dc8c7785e5f7f1fbc11f57ba62`  
		Last Modified: Wed, 31 Mar 2021 17:07:56 GMT  
		Size: 772.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-apache` - linux; mips64le

```console
$ docker pull phpmyadmin@sha256:0a214aa1a294075f9652c5617334d9c0cfc10c0392772e4a444f538f5e4e7d75
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.5 MB (146542606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99872b0fc47a687bc0a5d233d52f5ba1e49dcce1679bd4e1e6a88b88438a5cca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 30 Mar 2021 22:09:47 GMT
ADD file:b5b2f1fc18276a3928a2d904fedc2991239e065051f16680662a22627d15e809 in / 
# Tue, 30 Mar 2021 22:09:48 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:27:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 31 Mar 2021 00:27:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 31 Mar 2021 00:28:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:28:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 00:28:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 00:41:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 31 Mar 2021 00:41:07 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 31 Mar 2021 00:41:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 31 Mar 2021 00:41:34 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 31 Mar 2021 00:41:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 31 Mar 2021 00:41:37 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 31 Mar 2021 00:41:37 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 31 Mar 2021 00:41:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:41:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:41:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 01:29:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 01:29:38 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 01:29:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 01:29:38 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 01:30:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 01:30:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:37:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 01:37:50 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:37:52 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 01:37:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 01:37:53 GMT
STOPSIGNAL SIGWINCH
# Wed, 31 Mar 2021 01:37:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 31 Mar 2021 01:37:54 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 01:37:54 GMT
EXPOSE 80
# Wed, 31 Mar 2021 01:37:54 GMT
CMD ["apache2-foreground"]
# Wed, 31 Mar 2021 13:25:19 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:25:19 GMT
ENV MAX_EXECUTION_TIME=600
# Wed, 31 Mar 2021 13:25:20 GMT
ENV MEMORY_LIMIT=512M
# Wed, 31 Mar 2021 13:25:20 GMT
ENV UPLOAD_LIMIT=2048K
# Wed, 31 Mar 2021 13:25:22 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Wed, 31 Mar 2021 13:25:22 GMT
ENV VERSION=5.1.0
# Wed, 31 Mar 2021 13:25:22 GMT
ENV SHA256=aa8ccf357f672012384df34e1c2bc70147476761c8458a0dad6233497e142c68
# Wed, 31 Mar 2021 13:25:23 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.1.0/phpMyAdmin-5.1.0-all-languages.tar.xz
# Wed, 31 Mar 2021 13:25:23 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.1.0 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Wed, 31 Mar 2021 13:25:59 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 13:25:59 GMT
COPY file:74e988fef607090521e63cea57b4c61ab22b3a2a131bc55f0cf4a0d9c36ce65d in /etc/phpmyadmin/config.inc.php 
# Wed, 31 Mar 2021 13:26:00 GMT
COPY file:7a1864d35a5b72dc75fa085c7d09497f417e1ef1eacb8597037c366f1978b5fa in /docker-entrypoint.sh 
# Wed, 31 Mar 2021 13:26:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 31 Mar 2021 13:26:00 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:17fa7bb8f5ce4138c383674409fef134204b2ae72f4a997a2cebccad07e8e32b`  
		Last Modified: Tue, 30 Mar 2021 22:16:21 GMT  
		Size: 25.8 MB (25806366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352cbf73d26a044699ae2f07261cb972fea9bcddf88ba2198123b5deda9e10f4`  
		Last Modified: Wed, 31 Mar 2021 02:51:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719d1191368872841cbb21ecc69ac171357d4b1e986c7a460dcb0bc3d060f095`  
		Last Modified: Wed, 31 Mar 2021 02:52:26 GMT  
		Size: 61.4 MB (61403934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378cc22997f22b69d3ca6ba56580b5d4484b5ce25878d6418a118d57ba4f3901`  
		Last Modified: Wed, 31 Mar 2021 02:51:33 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62127adbed234a9716aa432d63f5ae149d7ee75760975aeb689b946bff15018e`  
		Last Modified: Wed, 31 Mar 2021 02:53:39 GMT  
		Size: 18.6 MB (18611846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d871e5e37c3826ba352fbc4195db2beb75a09531d9d2ffd54c082acc3116e9b`  
		Last Modified: Wed, 31 Mar 2021 02:53:27 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287285d0016f6c7e1245afa87cec55748ca10ce804ebad7bd7be584d800e3958`  
		Last Modified: Wed, 31 Mar 2021 02:53:26 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00bb7252e605f9d6d44db8e13ffc40d69bba29e7056303796886473f2ba09f5`  
		Last Modified: Wed, 31 Mar 2021 02:56:59 GMT  
		Size: 10.7 MB (10669809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af1f8e81b53ba5a78af086cd62194473838dd01d92984489ac5df0432a909a5`  
		Last Modified: Wed, 31 Mar 2021 02:56:54 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d641839f4a33746de988911afe5c71325e58f7935733c0aa1ccc9db5a2fedd2`  
		Last Modified: Wed, 31 Mar 2021 02:57:05 GMT  
		Size: 13.1 MB (13145837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35085a9bf16bc80e84b0706123dcb6deec56755c0c52fbca8a180e444bba63e5`  
		Last Modified: Wed, 31 Mar 2021 02:56:54 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d5105f329c9e6b157d41cdfefcc3d7dc735219175384d45f25882202f8dda7`  
		Last Modified: Wed, 31 Mar 2021 02:56:54 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9398692363fcd5f84781ff55f510926135dc4ac1bb5cf3727bccfbd092da316`  
		Last Modified: Wed, 31 Mar 2021 02:56:54 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fef1f3f3e6855692bcfbbd6e4ab55b9ab77c94db58c21dd35b39a8e16e7adb2`  
		Last Modified: Wed, 31 Mar 2021 13:29:37 GMT  
		Size: 2.8 MB (2809135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044d99fccdd86340681c4fd9bb8146844883269f792f409bbef90ae3b6266588`  
		Last Modified: Wed, 31 Mar 2021 13:29:35 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649253527fb8ed8a7293694c1a2584cc25cdd450ab1a833f948839fd0c711cb5`  
		Last Modified: Wed, 31 Mar 2021 13:29:49 GMT  
		Size: 14.1 MB (14087586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7a6bd114f0ec8d20eba7dd401efb8685eabd06b70991f780f1cafa02d392e6`  
		Last Modified: Wed, 31 Mar 2021 13:29:35 GMT  
		Size: 1.5 KB (1497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be500e12805e3244eedcfa627cb1bc02387c47ba803d740e8d746101a5629977`  
		Last Modified: Wed, 31 Mar 2021 13:29:35 GMT  
		Size: 771.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-apache` - linux; ppc64le

```console
$ docker pull phpmyadmin@sha256:c009bbfd04e746af7e5b80692fe7d06be34ab59f3c94e808f7f406eaba27a69a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.5 MB (175457585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e5ac2ec343b7303fd78fbd9cf5182af97a34c20483137f1f1c5af5008ba5921`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Fri, 26 Mar 2021 15:14:22 GMT
ADD file:feb26657639018f8f43408e43e8ecec7e84632f33b42d5521241b842b58747d5 in / 
# Fri, 26 Mar 2021 15:14:28 GMT
CMD ["bash"]
# Sat, 27 Mar 2021 12:15:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 27 Mar 2021 12:15:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 27 Mar 2021 12:18:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 27 Mar 2021 12:18:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 27 Mar 2021 12:19:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 27 Mar 2021 12:28:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 27 Mar 2021 12:29:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 27 Mar 2021 12:31:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 27 Mar 2021 12:31:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 27 Mar 2021 12:31:40 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 27 Mar 2021 12:31:44 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 27 Mar 2021 12:31:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 27 Mar 2021 12:31:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 27 Mar 2021 12:31:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 27 Mar 2021 12:32:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 27 Mar 2021 13:21:40 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 27 Mar 2021 13:21:48 GMT
ENV PHP_VERSION=7.4.16
# Sat, 27 Mar 2021 13:21:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Sat, 27 Mar 2021 13:21:57 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Sat, 27 Mar 2021 13:24:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 27 Mar 2021 13:24:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 27 Mar 2021 13:33:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 27 Mar 2021 13:33:28 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Sat, 27 Mar 2021 13:33:42 GMT
RUN docker-php-ext-enable sodium
# Sat, 27 Mar 2021 13:33:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 27 Mar 2021 13:33:56 GMT
STOPSIGNAL SIGWINCH
# Sat, 27 Mar 2021 13:34:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 27 Mar 2021 13:34:07 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 13:34:13 GMT
EXPOSE 80
# Sat, 27 Mar 2021 13:34:19 GMT
CMD ["apache2-foreground"]
# Sun, 28 Mar 2021 08:52:56 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 28 Mar 2021 08:53:01 GMT
ENV MAX_EXECUTION_TIME=600
# Sun, 28 Mar 2021 08:53:04 GMT
ENV MEMORY_LIMIT=512M
# Sun, 28 Mar 2021 08:53:08 GMT
ENV UPLOAD_LIMIT=2048K
# Sun, 28 Mar 2021 08:53:15 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Sun, 28 Mar 2021 08:53:17 GMT
ENV VERSION=5.1.0
# Sun, 28 Mar 2021 08:53:21 GMT
ENV SHA256=aa8ccf357f672012384df34e1c2bc70147476761c8458a0dad6233497e142c68
# Sun, 28 Mar 2021 08:53:24 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.1.0/phpMyAdmin-5.1.0-all-languages.tar.xz
# Sun, 28 Mar 2021 08:53:27 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.1.0 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Sun, 28 Mar 2021 08:54:32 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 28 Mar 2021 08:54:34 GMT
COPY file:74e988fef607090521e63cea57b4c61ab22b3a2a131bc55f0cf4a0d9c36ce65d in /etc/phpmyadmin/config.inc.php 
# Sun, 28 Mar 2021 08:54:36 GMT
COPY file:7a1864d35a5b72dc75fa085c7d09497f417e1ef1eacb8597037c366f1978b5fa in /docker-entrypoint.sh 
# Sun, 28 Mar 2021 08:54:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 28 Mar 2021 08:54:41 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:035681ea37d9aab4545aa2211af3bf79addea316f71afde84412406734ef8a85`  
		Last Modified: Fri, 26 Mar 2021 15:22:05 GMT  
		Size: 30.5 MB (30525677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c3efff20858e093a0bff310124796f2321b2bc8964e0d0e48b22c9f4876058`  
		Last Modified: Sat, 27 Mar 2021 14:34:32 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9259c2b9906eef8f4a0c3d0d0b394c6497e7810228a52ad6ef5d2fa451d42b52`  
		Last Modified: Sat, 27 Mar 2021 14:34:49 GMT  
		Size: 82.3 MB (82290413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f4d9b55064b59044559292c4bf2445bef705cc996a4186ae5b4093a07a32be`  
		Last Modified: Sat, 27 Mar 2021 14:34:31 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4852f5d2ead79af043efc780980e2ca898ef5b936eac6fe618e788420b16c6ee`  
		Last Modified: Sat, 27 Mar 2021 14:35:59 GMT  
		Size: 19.8 MB (19818428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00e01469baa8d78f6aed1754bba7133ecc1c93a03d38aa6c058dbdda0117e24`  
		Last Modified: Sat, 27 Mar 2021 14:35:54 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a808486650c424510050b53dd2fd2caa68070fbfdcfa1d72b37bb565144152b0`  
		Last Modified: Sat, 27 Mar 2021 14:35:51 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2f724feec6582a6254edbdbd9f1a8ba99734bd9ca7e24db9ae24dd4950be52`  
		Last Modified: Sat, 27 Mar 2021 14:38:58 GMT  
		Size: 10.7 MB (10672104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108a56ec0b082242afc703e20a50585105bdaaaa1e3af5690474ed3804495826`  
		Last Modified: Sat, 27 Mar 2021 14:38:53 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7121e8ad44c2b2b9682d272282f68fd5bc6fe5801afa5cfd4660cd57889dd432`  
		Last Modified: Sat, 27 Mar 2021 14:38:57 GMT  
		Size: 14.9 MB (14880529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8774c750f8ccf62b8401564c73205c14781bc85d6aaf2d82608d9154d4b8d3b`  
		Last Modified: Sat, 27 Mar 2021 14:38:53 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402942ac2d9d339ea9e31d2c6fae4deb8537d3dd0d13606f50b38f81ed954b39`  
		Last Modified: Sat, 27 Mar 2021 14:38:53 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3da7cbe64cd827bf2415be0757c7688cae02e1752c01da8ab3faafdd7488481`  
		Last Modified: Sat, 27 Mar 2021 14:38:53 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d082115294cfaae150a323efcbef45d6805d95eb24b5b11c5874ec9a5cea03`  
		Last Modified: Sun, 28 Mar 2021 08:59:25 GMT  
		Size: 3.2 MB (3164155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f8de40b36cf7e11102317450aaabdc7daf1ac4fe58ee28be2671ab12cf3d8c`  
		Last Modified: Sun, 28 Mar 2021 08:59:24 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a340e4e384d70f19e9f796c1267df7d0601fc85dab88200f4c663cea1b17de`  
		Last Modified: Sun, 28 Mar 2021 08:59:28 GMT  
		Size: 14.1 MB (14098025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:355b8bf0e0c916cf897d189f0335e3fb2bdacc305b192da58235e7b43ba00c35`  
		Last Modified: Sun, 28 Mar 2021 08:59:24 GMT  
		Size: 1.5 KB (1528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3e832a6eb450ed5e28edb8a489281f645d81286c0f268850a3582bc605c6d8`  
		Last Modified: Sun, 28 Mar 2021 08:59:24 GMT  
		Size: 772.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:5-apache` - linux; s390x

```console
$ docker pull phpmyadmin@sha256:9277c951cfa600c46bde759c6f37f19e5e1e80fffe66b64232b5b6078ac8650f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.6 MB (149636323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca368b84ab35136858e25f572ad3f7c0a9dd25d1a5effa13cf864d778f87a766`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:45 GMT
ADD file:df31b107763f0c1cce4527f1e2152ee5b995aa1d062c457c2852bea8dadab8a6 in / 
# Tue, 30 Mar 2021 21:42:46 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:59:29 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 30 Mar 2021 23:59:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 30 Mar 2021 23:59:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:59:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Mar 2021 23:59:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 00:05:08 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 31 Mar 2021 00:05:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 31 Mar 2021 00:05:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 31 Mar 2021 00:05:28 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 31 Mar 2021 00:05:29 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 31 Mar 2021 00:05:30 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 31 Mar 2021 00:05:30 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 31 Mar 2021 00:05:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:05:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 00:05:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 00:18:46 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 00:18:46 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 00:18:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 00:18:47 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 00:18:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 31 Mar 2021 00:18:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:21:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 00:21:10 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:21:11 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 00:21:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 00:21:12 GMT
STOPSIGNAL SIGWINCH
# Wed, 31 Mar 2021 00:21:12 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 31 Mar 2021 00:21:12 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 00:21:12 GMT
EXPOSE 80
# Wed, 31 Mar 2021 00:21:13 GMT
CMD ["apache2-foreground"]
# Wed, 31 Mar 2021 09:20:17 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libbz2-dev         libfreetype6-dev         libjpeg-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 09:20:18 GMT
ENV MAX_EXECUTION_TIME=600
# Wed, 31 Mar 2021 09:20:18 GMT
ENV MEMORY_LIMIT=512M
# Wed, 31 Mar 2021 09:20:19 GMT
ENV UPLOAD_LIMIT=2048K
# Wed, 31 Mar 2021 09:20:20 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly=1';         echo 'session.use_strict_mode=1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen=Off';         echo 'max_execution_time=${MAX_EXECUTION_TIME}';         echo 'max_input_vars=10000';         echo 'memory_limit=${MEMORY_LIMIT}';         echo 'post_max_size=${UPLOAD_LIMIT}';         echo 'upload_max_filesize=${UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Wed, 31 Mar 2021 09:20:20 GMT
ENV VERSION=5.1.0
# Wed, 31 Mar 2021 09:20:20 GMT
ENV SHA256=aa8ccf357f672012384df34e1c2bc70147476761c8458a0dad6233497e142c68
# Wed, 31 Mar 2021 09:20:21 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.1.0/phpMyAdmin-5.1.0-all-languages.tar.xz
# Wed, 31 Mar 2021 09:20:21 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.1.0 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Wed, 31 Mar 2021 09:20:33 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         gnupg         dirmngr     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 09:20:34 GMT
COPY file:74e988fef607090521e63cea57b4c61ab22b3a2a131bc55f0cf4a0d9c36ce65d in /etc/phpmyadmin/config.inc.php 
# Wed, 31 Mar 2021 09:20:34 GMT
COPY file:7a1864d35a5b72dc75fa085c7d09497f417e1ef1eacb8597037c366f1978b5fa in /docker-entrypoint.sh 
# Wed, 31 Mar 2021 09:20:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 31 Mar 2021 09:20:35 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9963ac8f97a3cf1f319e6c80042725f76dce93363a3d6b65e6808e1cd1bcfd7f`  
		Last Modified: Tue, 30 Mar 2021 21:46:19 GMT  
		Size: 25.8 MB (25753755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371213f07fea0a0f872bf0d091f7465c36fa7dda5dd5954941ab4416869b7059`  
		Last Modified: Wed, 31 Mar 2021 00:43:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938cc915f5117d6a5b05f98b4d0e1f7f16367df8d2bdb348a42a011d67843718`  
		Last Modified: Wed, 31 Mar 2021 00:44:02 GMT  
		Size: 64.7 MB (64709509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02470c7dad2d8dd8f8186e20fe6e989a534273373e80b8c45eb2afc1cd562287`  
		Last Modified: Wed, 31 Mar 2021 00:43:52 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3485ab85c5274ee04249aaf6f7cbaf25dd5c97ae61220a875947a11c43d20f`  
		Last Modified: Wed, 31 Mar 2021 00:44:59 GMT  
		Size: 18.5 MB (18524985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87bfc55f9e6134008ac7f8d4c9e0c10d75fafc7eced53b44833709f9b3cdb193`  
		Last Modified: Wed, 31 Mar 2021 00:44:54 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f096a4ea4985b6139b3aafc8fe206683fbb09651b97e3543a6a0da99a1fe1c9`  
		Last Modified: Wed, 31 Mar 2021 00:44:53 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1c5007697ed618c3632ac3e5e479d71ffe86844f974dd97eb5f3d7fa9d2c54`  
		Last Modified: Wed, 31 Mar 2021 00:47:35 GMT  
		Size: 10.7 MB (10670600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0507d530194f595bd77ec95fa11d7946f86c6ea1d09c7b52ab6fb72b1fd9bf`  
		Last Modified: Wed, 31 Mar 2021 00:47:31 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e86a80ca4007c82bf87c2c0abe40c0af540ebbab9e69bbe111ea3b60819ebde`  
		Last Modified: Wed, 31 Mar 2021 00:47:33 GMT  
		Size: 13.1 MB (13051275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834f12807de495de9664d835a1e0135ad5ec899baf051d027e19f53a4dbdaf19`  
		Last Modified: Wed, 31 Mar 2021 00:47:31 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03928ee863e1205fcdc461e2a3f9df20b0fd5ac91997b00d84d5ed6462188ba0`  
		Last Modified: Wed, 31 Mar 2021 00:47:31 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba23d890ab93bac4c9123a45ef71d671b9922544efb3a0418d5d9e851c71311`  
		Last Modified: Wed, 31 Mar 2021 00:47:31 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6f5ad5c28bf6287bce9f6020e7cbcbc8d7a3e5bf938a85adcc2bc11742085e`  
		Last Modified: Wed, 31 Mar 2021 09:22:37 GMT  
		Size: 2.8 MB (2826793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e543a5bf28decc5ffaa63d52fae81e24e2f4500b024140af3fd0885ace416b83`  
		Last Modified: Wed, 31 Mar 2021 09:22:36 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b6e2e4877674a196f4c4997603a7ebc2b419081c09dc4d4e1512fbcf4043e`  
		Last Modified: Wed, 31 Mar 2021 09:22:39 GMT  
		Size: 14.1 MB (14091161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed8e625cde3965a3a7aa901eace53367b75eb343ed368fa8fc625b9a4062ae2`  
		Last Modified: Wed, 31 Mar 2021 09:22:37 GMT  
		Size: 1.5 KB (1527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712a5ca49a28e6ac74cd8516903ab21c0259a91bd3111e4cd299e237b20a25bf`  
		Last Modified: Wed, 31 Mar 2021 09:22:36 GMT  
		Size: 772.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
