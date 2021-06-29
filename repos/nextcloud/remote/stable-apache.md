## `nextcloud:stable-apache`

```console
$ docker pull nextcloud@sha256:5c736834bffe4657f918fbb0212912693e79bf2959e8a2450f45e7493d7f1ecf
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

### `nextcloud:stable-apache` - linux; amd64

```console
$ docker pull nextcloud@sha256:019cf6f76f63a5f118b61565960c21059c0e999d1d563a067e66f404c2bdb0b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.9 MB (296922374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fad924df0823d63ac7adde0b2e36bf58b3f875d9c6d5eee3f30d2a571f95f5e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 11:48:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 11:48:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 11:48:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 11:48:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 11:48:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 11:55:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 11:55:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 11:55:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 11:55:53 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 11:55:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 11:55:55 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 11:55:55 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 11:55:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 11:55:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 11:55:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 12:46:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 23 Jun 2021 12:46:56 GMT
ENV PHP_VERSION=7.4.20
# Wed, 23 Jun 2021 12:46:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 23 Jun 2021 12:46:56 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Mon, 28 Jun 2021 21:39:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 21:39:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:44:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 21:44:48 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:44:51 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 21:44:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 21:44:51 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 21:44:52 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:44:52 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 21:44:53 GMT
EXPOSE 80
# Mon, 28 Jun 2021 21:44:53 GMT
CMD ["apache2-foreground"]
# Tue, 29 Jun 2021 04:26:12 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 29 Jun 2021 04:26:13 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 29 Jun 2021 04:26:13 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 29 Jun 2021 04:29:11 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 04:29:12 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 29 Jun 2021 04:29:12 GMT
VOLUME [/var/www/html]
# Tue, 29 Jun 2021 04:29:13 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 29 Jun 2021 04:37:26 GMT
ENV NEXTCLOUD_VERSION=20.0.10
# Tue, 29 Jun 2021 04:38:11 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 04:38:13 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 29 Jun 2021 04:38:14 GMT
COPY multi:bb22a87f07ec65f9db22db69c1e13d98d1b6e10d12cf7747d547023b06cd53c6 in /usr/src/nextcloud/config/ 
# Tue, 29 Jun 2021 04:38:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 04:38:15 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b85dd8f01492a64ab518247894d5b93db91b5ef9c770b601b37f612278b602`  
		Last Modified: Wed, 23 Jun 2021 13:53:31 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8589b26a90be6577309788924232d8900e0e44f0a7fb4ca01c32c6467578a27d`  
		Last Modified: Wed, 23 Jun 2021 13:53:50 GMT  
		Size: 76.7 MB (76680976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5af5d6419462987bdb2cd60de0729dcf0c35933ca87692f2eb9ca1ae292a642`  
		Last Modified: Wed, 23 Jun 2021 13:53:31 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614ec6f0b8d6a562071e6a2584ca97b4237364aa3b78b00aa6c601a00c80d019`  
		Last Modified: Wed, 23 Jun 2021 13:54:26 GMT  
		Size: 18.7 MB (18679261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b28f3797fbefaacc6339a39139cd689c6038bdbe1ee96bd947d58397be3538`  
		Last Modified: Wed, 23 Jun 2021 13:54:22 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bcb7d2e6b049343069918b727a239aa0ae67500a2f20744af37dd6c89d90d9`  
		Last Modified: Wed, 23 Jun 2021 13:54:22 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aaa379b3e64ec978b15500be6afceea9013b530b98a0e73165358859be183e1`  
		Last Modified: Tue, 29 Jun 2021 00:46:32 GMT  
		Size: 10.7 MB (10683997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d533abc0d2def8c43e6d54b377a762c9dfb2e95481307ad5335e529b60d363`  
		Last Modified: Tue, 29 Jun 2021 00:46:28 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073fc0e59151f4a4b744b265c027a4692219992cf959606ddbdf8b8227b71845`  
		Last Modified: Tue, 29 Jun 2021 00:46:32 GMT  
		Size: 13.8 MB (13841305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb495bf170975779cb3b386cfa951522c40a000f01d9f712718515b2c82e5234`  
		Last Modified: Tue, 29 Jun 2021 00:46:28 GMT  
		Size: 2.3 KB (2279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1db301acce363d1945fd51dd6465dccf579067a73ee45c0f10db617595c800f`  
		Last Modified: Tue, 29 Jun 2021 00:46:28 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5572477d34e8c54adc39ceafea9b09ebb961ef09f3de1035c33b8d33b7df7c0e`  
		Last Modified: Tue, 29 Jun 2021 00:46:28 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9839d9c386801c3c0d1f07326c49959b370cf90e25cebebed477165ab9d40410`  
		Last Modified: Tue, 29 Jun 2021 04:44:10 GMT  
		Size: 1.7 MB (1659726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce56b0542405345f8a1e35d4ff845fefed928a7c646e0f40afe1608662686c8f`  
		Last Modified: Tue, 29 Jun 2021 04:44:14 GMT  
		Size: 15.7 MB (15683237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614e221407e6327452136b8a4ecde009cd52cf77584b34e62d57a21f6f6bd187`  
		Last Modified: Tue, 29 Jun 2021 04:44:06 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025161e582ddfe75ebcceaa76799b3ac6a78d09aba019e7ab5f88dc12a2f344f`  
		Last Modified: Tue, 29 Jun 2021 04:44:06 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee326eb551c4eec631c5711e6e802cc2bcfe791ca602d999d7d58a86a8d3991`  
		Last Modified: Tue, 29 Jun 2021 04:46:12 GMT  
		Size: 132.5 MB (132536757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4229b8e930fd16f673ff7d7437d6624906fb48e4c1b3a2fe05ed78cec26c6109`  
		Last Modified: Tue, 29 Jun 2021 04:45:52 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900cf7e35b0418d40cdd74f570d3d5e0c9613451c603b8958de2289d58d150ee`  
		Last Modified: Tue, 29 Jun 2021 04:45:52 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable-apache` - linux; arm variant v5

```console
$ docker pull nextcloud@sha256:23e3451f4a92810cb9ec51c869e0ca2f6b709abedf1011c9924c1acbf78c78f4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.7 MB (273737300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca82a9c600211ce2473a372710635ef762c3f023d16a1d5466d44b445a962602`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 06:34:32 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 06:34:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 06:35:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 06:35:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 06:35:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 06:41:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 06:41:08 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 06:41:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 06:41:33 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 06:41:35 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 06:41:35 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 06:41:35 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 06:41:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 06:41:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 06:41:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 07:26:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 23 Jun 2021 07:26:02 GMT
ENV PHP_VERSION=7.4.20
# Wed, 23 Jun 2021 07:26:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 23 Jun 2021 07:26:03 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Mon, 28 Jun 2021 19:44:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 19:44:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:48:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 19:48:13 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:48:15 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 19:48:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 19:48:16 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 19:48:16 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 19:48:17 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 19:48:17 GMT
EXPOSE 80
# Mon, 28 Jun 2021 19:48:18 GMT
CMD ["apache2-foreground"]
# Tue, 29 Jun 2021 00:38:18 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 29 Jun 2021 00:38:18 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 29 Jun 2021 00:38:19 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 29 Jun 2021 00:45:24 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 00:45:26 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 29 Jun 2021 00:45:27 GMT
VOLUME [/var/www/html]
# Tue, 29 Jun 2021 00:45:29 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 29 Jun 2021 00:55:44 GMT
ENV NEXTCLOUD_VERSION=20.0.10
# Tue, 29 Jun 2021 00:57:04 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 00:57:06 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 29 Jun 2021 00:57:08 GMT
COPY multi:bb22a87f07ec65f9db22db69c1e13d98d1b6e10d12cf7747d547023b06cd53c6 in /usr/src/nextcloud/config/ 
# Tue, 29 Jun 2021 00:57:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 00:57:09 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4201a900b66f4e05c8ee53ef7ecdffa56d4cfc141826c4899ba2c7ea1565c3`  
		Last Modified: Wed, 23 Jun 2021 08:37:06 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8759f5b6f404f221d7035198880caf6e5b60d43c01daf59b9c7ff32e8ba5038f`  
		Last Modified: Wed, 23 Jun 2021 08:37:51 GMT  
		Size: 58.8 MB (58820428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bee84cde96b6e1abd89640d87273fd846cad74593b3ec8bdd0167bb76f06398`  
		Last Modified: Wed, 23 Jun 2021 08:37:06 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d04a75937c26e6facc2a34e28c4f30008fb2c8c38d4a6109ab3bd73a1a4d516`  
		Last Modified: Wed, 23 Jun 2021 08:38:40 GMT  
		Size: 18.0 MB (18026172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ecd491048519ab1e7d82a3cf53d86795ba9b3b230f90332de7efe0d76f16cd`  
		Last Modified: Wed, 23 Jun 2021 08:38:29 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b63bc3f991d218876d985827b11cbce08ca267e836215529cbbfbd0a0abf7b`  
		Last Modified: Wed, 23 Jun 2021 08:38:29 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9546f38d4a0ad55e546a4e9128f913ba10e5d7c0eba6d20124edfbe5ff5207e6`  
		Last Modified: Mon, 28 Jun 2021 21:04:34 GMT  
		Size: 10.7 MB (10682079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f96422e21ac525e34217914d20472d3de7b88cdedc3ede93b0e2545f8202e8a`  
		Last Modified: Mon, 28 Jun 2021 21:04:30 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e63d11cb66bcdd147461ebf1fcf391c5bef2dbe7e6f46b1c70e4bb22359a8e`  
		Last Modified: Mon, 28 Jun 2021 21:04:37 GMT  
		Size: 12.9 MB (12925136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be569f4a31534d2bcfc160dd2fc4c001fa03d31c81a64e8768fb4f2db421168`  
		Last Modified: Mon, 28 Jun 2021 21:04:30 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96562a47756fb732c58c88dbe44879741a07146639a4940d5f52c237e56d2c36`  
		Last Modified: Mon, 28 Jun 2021 21:04:30 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee014d2d48ee22c313f00792bd84f176a4bb461c5f1136a8c376ddfea63a1a6f`  
		Last Modified: Mon, 28 Jun 2021 21:04:30 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443151059d94236b9af7e1a1511fd7f4dcd5e2a1b882bc403c2b5df7e4a83f0`  
		Last Modified: Tue, 29 Jun 2021 01:05:31 GMT  
		Size: 1.6 MB (1597227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4703852cdbb46ee01cf1ac726d8d942ac7b058461b2e26433109efd68208e511`  
		Last Modified: Tue, 29 Jun 2021 01:05:39 GMT  
		Size: 14.3 MB (14261669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8991237f55fb30ea1a385a40cfb91213f27c0c963a33e09362384f0dd38e0ad`  
		Last Modified: Tue, 29 Jun 2021 01:05:28 GMT  
		Size: 596.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d007c8b6d1cab2a0b1e90ab74625c708c7f8f98eedee1d44740420f969e784b0`  
		Last Modified: Tue, 29 Jun 2021 01:05:28 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f82b1e4d05393253426449a8f8f4d26d564a97828b34d44c5784cad3ec53e78`  
		Last Modified: Tue, 29 Jun 2021 01:10:11 GMT  
		Size: 132.5 MB (132534370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3d6b969de8ce58a1cb4ba2d2f13068eeb37a41322fd8cc8eeb47db294a0e44`  
		Last Modified: Tue, 29 Jun 2021 01:08:43 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7b4874abf65ffafc4faaa95ac3976a62dc7eee1d0615eaf89d7f625d2fae37`  
		Last Modified: Tue, 29 Jun 2021 01:08:43 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable-apache` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:0f98af011e86d02b7dede7437f54133b2302e27f75c6c8a66aedaa60284ab597
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.9 MB (269866925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d33d94b34e44ff01f819dc488f9c05a960f81fc46a2580cb5797c33fb3665a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:21:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 08:21:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 08:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:22:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 08:22:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 08:27:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 08:27:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 08:27:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 08:27:27 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 08:27:28 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 08:27:29 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 08:27:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 08:27:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:27:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:27:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 09:44:25 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 23 Jun 2021 09:44:25 GMT
ENV PHP_VERSION=7.4.20
# Wed, 23 Jun 2021 09:44:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 23 Jun 2021 09:44:26 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Mon, 28 Jun 2021 21:16:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 21:16:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:20:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 21:20:38 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:20:40 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 21:20:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 21:20:41 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 21:20:41 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:20:42 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 21:20:42 GMT
EXPOSE 80
# Mon, 28 Jun 2021 21:20:42 GMT
CMD ["apache2-foreground"]
# Tue, 29 Jun 2021 07:32:01 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 29 Jun 2021 07:32:01 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 29 Jun 2021 07:32:02 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 29 Jun 2021 07:38:37 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 07:38:39 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 29 Jun 2021 07:38:39 GMT
VOLUME [/var/www/html]
# Tue, 29 Jun 2021 07:38:41 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 29 Jun 2021 07:55:00 GMT
ENV NEXTCLOUD_VERSION=20.0.10
# Tue, 29 Jun 2021 07:56:18 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 07:56:21 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 29 Jun 2021 07:56:24 GMT
COPY multi:bb22a87f07ec65f9db22db69c1e13d98d1b6e10d12cf7747d547023b06cd53c6 in /usr/src/nextcloud/config/ 
# Tue, 29 Jun 2021 07:56:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 07:56:24 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9600bb4c83e3ef3465228eed7d6e9dfed7dc9078d2ab47f0bbdc8ccd6cb2b4`  
		Last Modified: Wed, 23 Jun 2021 11:51:40 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e4b7395146be79190767115c26cc6b70ac8d5af36c4a7acf9de1f34d06b41d7`  
		Last Modified: Wed, 23 Jun 2021 11:52:18 GMT  
		Size: 59.5 MB (59514051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3641f6e3173b95d08e8b4ec00f48cb7e09d9813f88a086a422173594dfc93ddd`  
		Last Modified: Wed, 23 Jun 2021 11:51:40 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7d1aa9268ffe2596e041fe0130bbdc37fb7e587a9b8d7c5346360e2f27b41d`  
		Last Modified: Wed, 23 Jun 2021 11:53:09 GMT  
		Size: 17.5 MB (17481801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d56adf5c38075c402f8bf5f30dee3d2dd1d1f5c327b12641f29af33f5ba950a`  
		Last Modified: Wed, 23 Jun 2021 11:52:58 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17bf5eeb5d260e70dda8e6cf6bf12b837eca9e5650117ad4e659861a5ecc31f5`  
		Last Modified: Wed, 23 Jun 2021 11:52:58 GMT  
		Size: 518.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cbfcb4ea88d4b49a4284ce12b90b824f9b7d900b24f02e000f44605c539063e`  
		Last Modified: Mon, 28 Jun 2021 23:40:52 GMT  
		Size: 10.7 MB (10682127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cb9152f0d1f8e555ebe86c42f1805781c50b10913629d15047dbcff18b166c`  
		Last Modified: Mon, 28 Jun 2021 23:40:47 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83ab0721e4c9479657e33a58bf27be9718c3ede5c5d19313b58aca855829d4e`  
		Last Modified: Mon, 28 Jun 2021 23:40:56 GMT  
		Size: 12.2 MB (12224232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc2068c3c1454f983493a79ffabeaa607385f9f76f0e93b8abf6ebee25ecad9`  
		Last Modified: Mon, 28 Jun 2021 23:40:47 GMT  
		Size: 2.3 KB (2280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545719806bafaa902b49be4719a058e95c8a251cf28d1bc78c53c69e2bba938a`  
		Last Modified: Mon, 28 Jun 2021 23:40:47 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dded5cc0d9b2cde2ba09113433fa5c6f248cd0a8c88aecc2df2b7273094a8db`  
		Last Modified: Mon, 28 Jun 2021 23:40:47 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7e66a1e80ceacfc9c1d9b563576f9375b4df6d08031b38be32c672084b9dd7`  
		Last Modified: Tue, 29 Jun 2021 08:10:35 GMT  
		Size: 1.4 MB (1449464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e1d38a695bee40b30ed643dc39f227c627d09e985d86f0e605c75b16469ce81`  
		Last Modified: Tue, 29 Jun 2021 08:10:42 GMT  
		Size: 13.2 MB (13223359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b3294eeeef3d874ba89d1403a2ff16e12a6314e38401a5cefb71d56de1fccd`  
		Last Modified: Tue, 29 Jun 2021 08:10:32 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6417eb82e1be00577a98bc783b6b47426829cf865214a82625c23a6b17dfe86`  
		Last Modified: Tue, 29 Jun 2021 08:10:32 GMT  
		Size: 595.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758ccd07ef9ebe1ac94199d087548188622b40366d770d51131cb3848d81164b`  
		Last Modified: Tue, 29 Jun 2021 08:16:52 GMT  
		Size: 132.5 MB (132534550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92eabf7a7cdfa54ef4163a75c0a03d83c5eb60b61be3363787a38bc2def87f62`  
		Last Modified: Tue, 29 Jun 2021 08:15:24 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4e7e08dd7ded5419e202ebaf15bcfba14cd564e8607b4bcb11d2229020e101`  
		Last Modified: Tue, 29 Jun 2021 08:15:24 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable-apache` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:67a75ed2da9eb6303e1fc6a7ab3c8e55aecfcec50d2ff83426fa6603f5b658c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.4 MB (287388849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad6ed97e68360d9e10fc4ee0f0a17a8bee9b2b4a5730066f3a4b813ae9f282a0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 08:48:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 08:48:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 08:48:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 08:48:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 08:48:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 08:53:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 08:53:47 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 08:53:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 08:53:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 08:53:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:53:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 08:53:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 09:33:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 23 Jun 2021 09:33:08 GMT
ENV PHP_VERSION=7.4.20
# Wed, 23 Jun 2021 09:33:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 23 Jun 2021 09:33:08 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Mon, 28 Jun 2021 21:09:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 21:09:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:11:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 21:11:37 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:11:38 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 21:11:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 21:11:38 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 21:11:38 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:11:39 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 21:11:39 GMT
EXPOSE 80
# Mon, 28 Jun 2021 21:11:39 GMT
CMD ["apache2-foreground"]
# Tue, 29 Jun 2021 02:30:24 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 29 Jun 2021 02:30:25 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 29 Jun 2021 02:30:25 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 29 Jun 2021 02:32:46 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 02:32:47 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 29 Jun 2021 02:32:47 GMT
VOLUME [/var/www/html]
# Tue, 29 Jun 2021 02:32:48 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 29 Jun 2021 02:40:00 GMT
ENV NEXTCLOUD_VERSION=20.0.10
# Tue, 29 Jun 2021 02:40:42 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 02:40:44 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 29 Jun 2021 02:40:45 GMT
COPY multi:bb22a87f07ec65f9db22db69c1e13d98d1b6e10d12cf7747d547023b06cd53c6 in /usr/src/nextcloud/config/ 
# Tue, 29 Jun 2021 02:40:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 02:40:45 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce6585fd70baac65871dafb05b7f408940165f163c30d7e0f9ec3518709e908`  
		Last Modified: Wed, 23 Jun 2021 10:25:12 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab6c01ccebb7fc71b44dfe6966672e34b47ea5e22d53a11e4481e76243cd44b`  
		Last Modified: Wed, 23 Jun 2021 10:25:24 GMT  
		Size: 70.4 MB (70356352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ed9f96098643713fabf62c17f792254db16c6623e3cec0b4a4ea602af2e742`  
		Last Modified: Wed, 23 Jun 2021 10:25:12 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6852e08c882a542c19980b469e16cebe09c20c56cb6a883fe46d7fa71c77a5bf`  
		Last Modified: Wed, 23 Jun 2021 10:26:10 GMT  
		Size: 18.6 MB (18579813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650d5012e5fa16b3bcc69043ccc3b45a8e75bd3651354579204af7abe7ae4eae`  
		Last Modified: Wed, 23 Jun 2021 10:26:01 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390447f485b4746ca973bb40b4a5ef8edc132fc2fd3b4c1e3681b22c5fa1ca47`  
		Last Modified: Wed, 23 Jun 2021 10:26:01 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4ad8756f988ef34285d2fdf05f5d79c391e27b52e4ade0d3583297f495e814`  
		Last Modified: Mon, 28 Jun 2021 23:02:08 GMT  
		Size: 10.7 MB (10682725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16017909d72b5fc6c769db7f8677e7108b32333880bcab335e0eedc7d645acbf`  
		Last Modified: Mon, 28 Jun 2021 23:02:05 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf60cb8599849ec6b77b66cb0f4d9f1f755064b6a143b38f02376652eebbc090`  
		Last Modified: Mon, 28 Jun 2021 23:02:08 GMT  
		Size: 13.6 MB (13628910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f09fa37d649ba479c6917f5a3cc2ec410603ec75655e91c7bc91c293433e322`  
		Last Modified: Mon, 28 Jun 2021 23:02:05 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4228983b6e1db84c0e9cfb0bfed817b2f5a8b7abbb6740ed64d73f0b9455b7de`  
		Last Modified: Mon, 28 Jun 2021 23:02:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349827697f70e6c2e51e639cc3d0c7a80c41e798679f2878c11fdd7ced3d447`  
		Last Modified: Mon, 28 Jun 2021 23:02:05 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a7a7a128e5f4d8f6ccec6fc2135dbec754d99c0b56441a204c5db47d730f77`  
		Last Modified: Tue, 29 Jun 2021 02:47:16 GMT  
		Size: 1.6 MB (1625903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92414278b9185b0370c0dea16b929c7d5a1cb8ca459b28df9bfe9710be3676f1`  
		Last Modified: Tue, 29 Jun 2021 02:47:18 GMT  
		Size: 14.1 MB (14053476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e527f86305b36b42ad9471f1e93024a5016fc7edc83d444fc87455645a0506`  
		Last Modified: Tue, 29 Jun 2021 02:47:13 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d424d437a47e3801aad90958adf2944797943280343e4e3a1c6f647f44260c1a`  
		Last Modified: Tue, 29 Jun 2021 02:47:12 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed126eca3dd4ee22e9c16ea958d54d002854d82ba862c1579d832a000e919657`  
		Last Modified: Tue, 29 Jun 2021 02:49:28 GMT  
		Size: 132.5 MB (132535421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9bba76072211dc14dedd04b1ef959e2625e219cd6f4b5d678808ced2ccab78`  
		Last Modified: Tue, 29 Jun 2021 02:49:06 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e6cea0222b9ee9924c111e2c5ca74a7fb428240a159535b265ed29e7e67bcd`  
		Last Modified: Tue, 29 Jun 2021 02:49:06 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable-apache` - linux; 386

```console
$ docker pull nextcloud@sha256:83f07cfb18c69f4eaaf1cc885053094d059ae768519ffc236dc15397e7b13a31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.3 MB (302256789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3929f92c6c15a056bdff629af4c7b68b62451c3b6d0c0ee72e36519619d32f44`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 09:40:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 09:40:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 09:40:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 09:40:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 09:40:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 09:49:27 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 09:49:27 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 09:49:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 09:49:44 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 09:49:46 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 09:49:46 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 09:49:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 11:00:35 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 23 Jun 2021 11:00:35 GMT
ENV PHP_VERSION=7.4.20
# Wed, 23 Jun 2021 11:00:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 23 Jun 2021 11:00:36 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Mon, 28 Jun 2021 22:14:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 22:14:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 22:17:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 22:17:57 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 22:18:00 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 22:18:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 22:18:00 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 22:18:01 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 22:18:02 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 22:18:02 GMT
EXPOSE 80
# Mon, 28 Jun 2021 22:18:02 GMT
CMD ["apache2-foreground"]
# Tue, 29 Jun 2021 05:37:52 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 29 Jun 2021 05:37:52 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 29 Jun 2021 05:37:53 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 29 Jun 2021 05:40:41 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 05:40:42 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 29 Jun 2021 05:40:43 GMT
VOLUME [/var/www/html]
# Tue, 29 Jun 2021 05:40:44 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 29 Jun 2021 05:49:26 GMT
ENV NEXTCLOUD_VERSION=20.0.10
# Tue, 29 Jun 2021 05:50:21 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 05:50:22 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 29 Jun 2021 05:50:23 GMT
COPY multi:bb22a87f07ec65f9db22db69c1e13d98d1b6e10d12cf7747d547023b06cd53c6 in /usr/src/nextcloud/config/ 
# Tue, 29 Jun 2021 05:50:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 05:50:24 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:851ded1e6779ac12f2623fa13c3d156987e0e3748e10171438e042c4a18cada8`  
		Last Modified: Wed, 23 Jun 2021 12:27:42 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9108f1298d19c1c39f13396485b32141017e3d97dcc7093d43854940c92b6c`  
		Last Modified: Wed, 23 Jun 2021 12:28:14 GMT  
		Size: 81.2 MB (81230041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a8cc691843125fa492ce4109092746e47e36d222eceef5b59dd10271176374`  
		Last Modified: Wed, 23 Jun 2021 12:27:42 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ce571916f9fd350c507c0b0f4ba7db9c473cb95da721dfeab5acd167c05197`  
		Last Modified: Wed, 23 Jun 2021 12:29:05 GMT  
		Size: 19.1 MB (19115037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abad9c9b3f342c41ff79e0b1832309d795f17e4aaafd51a979891c9c747684c`  
		Last Modified: Wed, 23 Jun 2021 12:28:58 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ecb5db768b6cdd9c3b371c253bc49fc82700b113499943217799b6cf74aab9`  
		Last Modified: Wed, 23 Jun 2021 12:28:58 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae2138f0ab7b1b88b759c919f347f7dd5b1541bf3add860dde8fd4fbc6dea86`  
		Last Modified: Tue, 29 Jun 2021 01:28:19 GMT  
		Size: 10.7 MB (10683335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a27e5f7d8daaef8c3df36f139608623ae4cd4818711fee73ffcbb0c6eed8c9d`  
		Last Modified: Tue, 29 Jun 2021 01:28:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a56b795f1c08704c0a53f94e1e73faa1a02b47786b8ece56c7d68603c5180a5`  
		Last Modified: Tue, 29 Jun 2021 01:28:22 GMT  
		Size: 14.2 MB (14172336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0982b2dd82a754c51bf2b1d4112361847735a82efe791d916ff8312e47513cf6`  
		Last Modified: Tue, 29 Jun 2021 01:28:14 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505d728d0018bdb86deba81916ae10fc757f7bb5fb4a706cfeb61b81382747ef`  
		Last Modified: Tue, 29 Jun 2021 01:28:14 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93774cdda08b87fb748efc09be920d7371caa3ca36ddb82d260b38bafef4bd`  
		Last Modified: Tue, 29 Jun 2021 01:28:15 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a15554874810e8cecad80f5142db4b5ccf80c04049157a6209d70631bccc59`  
		Last Modified: Tue, 29 Jun 2021 05:57:47 GMT  
		Size: 1.7 MB (1683710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f65d6456a9a1323e5fdcc196254044da1e21e3432163a86456577f7f03b209`  
		Last Modified: Tue, 29 Jun 2021 05:57:51 GMT  
		Size: 15.0 MB (15027579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6533d6f5d486af0767c6125c94df8cafd0dff1121c136f375f82a282a3c903a5`  
		Last Modified: Tue, 29 Jun 2021 05:57:44 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf44bb938eb087d649861d92e4fe7b764bdb0b1f4d0506491d3d29b7e58d90a`  
		Last Modified: Tue, 29 Jun 2021 05:57:44 GMT  
		Size: 577.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44faa00bd139ebc5e55ed966cca5fa54ae3c0c468a24ee097d27d15e827d69b7`  
		Last Modified: Tue, 29 Jun 2021 06:00:26 GMT  
		Size: 132.5 MB (132536083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb7bc752f20ad20890ffbf414749d24e1ff4c323b74d7eb09c48e40734187ae`  
		Last Modified: Tue, 29 Jun 2021 05:59:59 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8489d32395048cfcc723b710971116b4f43c322a0aa2f63a1228a9c7ee02039a`  
		Last Modified: Tue, 29 Jun 2021 05:59:59 GMT  
		Size: 2.1 KB (2056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable-apache` - linux; mips64le

```console
$ docker pull nextcloud@sha256:f2636724a7f06ff742ff4a3b18ffbf99c79818eeaf5d0e86b745d609ace3ed61
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.1 MB (278054303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9484048903614bf3616d87f48d1ddc35b6a83ed243a76102361c201478935fa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:29 GMT
ADD file:ca8422268fc66c67d19fd3a33a14a9bd6280ef21404677767ffd561a8ecf6724 in / 
# Wed, 23 Jun 2021 00:09:30 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 02:39:12 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 23 Jun 2021 02:39:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 23 Jun 2021 02:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 02:40:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Jun 2021 02:40:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Jun 2021 02:52:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 23 Jun 2021 02:52:57 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 23 Jun 2021 02:53:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 23 Jun 2021 02:53:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 23 Jun 2021 02:53:26 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 02:53:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Jun 2021 02:53:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Jun 2021 04:33:28 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 23 Jun 2021 04:33:28 GMT
ENV PHP_VERSION=7.4.20
# Wed, 23 Jun 2021 04:33:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Wed, 23 Jun 2021 04:33:29 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Mon, 28 Jun 2021 21:00:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 28 Jun 2021 21:00:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:08:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 28 Jun 2021 21:08:31 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:08:33 GMT
RUN docker-php-ext-enable sodium
# Mon, 28 Jun 2021 21:08:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 28 Jun 2021 21:08:34 GMT
STOPSIGNAL SIGWINCH
# Mon, 28 Jun 2021 21:08:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Mon, 28 Jun 2021 21:08:35 GMT
WORKDIR /var/www/html
# Mon, 28 Jun 2021 21:08:35 GMT
EXPOSE 80
# Mon, 28 Jun 2021 21:08:35 GMT
CMD ["apache2-foreground"]
# Tue, 29 Jun 2021 00:49:50 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Tue, 29 Jun 2021 00:49:51 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 29 Jun 2021 00:49:51 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 29 Jun 2021 00:57:42 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 00:57:44 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 29 Jun 2021 00:57:45 GMT
VOLUME [/var/www/html]
# Tue, 29 Jun 2021 00:57:47 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 29 Jun 2021 01:09:20 GMT
ENV NEXTCLOUD_VERSION=20.0.10
# Tue, 29 Jun 2021 01:11:08 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Jun 2021 01:11:11 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Tue, 29 Jun 2021 01:11:13 GMT
COPY multi:bb22a87f07ec65f9db22db69c1e13d98d1b6e10d12cf7747d547023b06cd53c6 in /usr/src/nextcloud/config/ 
# Tue, 29 Jun 2021 01:11:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Jun 2021 01:11:14 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:4b9d1870c33c63bfde89c401b4af9582fbbff99d4036171a7a456706bf805d6d`  
		Last Modified: Wed, 23 Jun 2021 00:15:49 GMT  
		Size: 25.8 MB (25812890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c90d345f251f9a0ec80cf41b5f35febb67c1c989281d9e68b2aeefee1c00143`  
		Last Modified: Wed, 23 Jun 2021 05:55:09 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6bf25841fee636dffd0610ecca37bade0d96a921f21482eda088538659d329a`  
		Last Modified: Wed, 23 Jun 2021 05:55:57 GMT  
		Size: 61.4 MB (61404106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b88a019f1da6587ce2665903b08be861bc197f91d09bfbfb6e62a368de4a231`  
		Last Modified: Wed, 23 Jun 2021 05:55:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e208dcf88dd78c21b0c19c351345924790c3caa4bbca1580e2e289d738c874ab`  
		Last Modified: Wed, 23 Jun 2021 05:56:42 GMT  
		Size: 18.6 MB (18611849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe3845bbf14eccd94071a1ab8d234fe05503b03c7d92b53ed1643a1ca33d9a4`  
		Last Modified: Wed, 23 Jun 2021 05:56:29 GMT  
		Size: 436.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8ec3aa526d170c9dd2f45b8bd19f5f8f080e143f30ba8431c0e6d9105ec4d0c`  
		Last Modified: Wed, 23 Jun 2021 05:56:29 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d38724202c2e9cc9176cddaefb0c6673dbadee6836192bdeeb523a10d1b013fc`  
		Last Modified: Mon, 28 Jun 2021 22:28:50 GMT  
		Size: 10.7 MB (10681368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d8131779978bc34649a0eb121bf9c0e3a72a7763b349b02a4efd8b5a6ad8c9`  
		Last Modified: Mon, 28 Jun 2021 22:28:43 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594107c42a984d9eecb939d08931f4135712fcacb727a9caf7077827b4e2a641`  
		Last Modified: Mon, 28 Jun 2021 22:28:55 GMT  
		Size: 13.1 MB (13147823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7318d498f16319e51d21946d668dca5ac88c4395a240fe4d554e3ad48f538d`  
		Last Modified: Mon, 28 Jun 2021 22:28:43 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea081015d41cc15cc02772f1ad550d3cf86155142a8e0ba55243d4659de09afc`  
		Last Modified: Mon, 28 Jun 2021 22:28:43 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d9b8bcbd21953aedd155a3c253e3a528602f6dde6a66ad028b942f2c900e11`  
		Last Modified: Mon, 28 Jun 2021 22:28:43 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee5372da567327900098d5a0054e653797c7e805ef3bb46b5105591e79eef9`  
		Last Modified: Tue, 29 Jun 2021 01:18:21 GMT  
		Size: 1.8 MB (1763803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e708cbe62d3e8feb4c75b4659939526fadc48aac896c41ee5f5b9d0af9eb1c`  
		Last Modified: Tue, 29 Jun 2021 01:18:31 GMT  
		Size: 14.1 MB (14087027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87038b5795dc5ff7e592c1cf6894c750ea695a8f23955e10e375116c3d9dec0c`  
		Last Modified: Tue, 29 Jun 2021 01:18:17 GMT  
		Size: 565.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84abeab57cb9d4241420d124ef4d2aa896a1bb97d3ab1e9e9e2fee00525f1741`  
		Last Modified: Tue, 29 Jun 2021 01:18:17 GMT  
		Size: 582.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc1516fe3da96f86d81ded03a66c05061cb132ac3c02ceac2f78b020040a5c9`  
		Last Modified: Tue, 29 Jun 2021 01:22:39 GMT  
		Size: 132.5 MB (132534307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d34a411bdb0fc99fa6897a841a7e67dc9ac5f4e8040c3c8a2b0e54fcf8edde`  
		Last Modified: Tue, 29 Jun 2021 01:21:19 GMT  
		Size: 2.6 KB (2631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c514d284f17c03083b66c5ec88881e11716f4a536bbfb935cfb7d5000e78c2b`  
		Last Modified: Tue, 29 Jun 2021 01:21:19 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable-apache` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:7f17ad7674012b8f4d73561fcf3f52a55c5e6116569e4ccd4345f78e8e5a8f81
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.5 MB (308536803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca348b0edba301e9f6dec64b869ab2724fa29b22d55652650819fb59952be5d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:38 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Wed, 23 Jun 2021 00:30:46 GMT
CMD ["bash"]
# Sat, 26 Jun 2021 04:04:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 26 Jun 2021 04:04:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 26 Jun 2021 04:09:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Jun 2021 04:09:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 26 Jun 2021 04:09:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 26 Jun 2021 04:24:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 26 Jun 2021 04:24:28 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 26 Jun 2021 04:26:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 26 Jun 2021 04:26:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 26 Jun 2021 04:26:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 26 Jun 2021 04:26:47 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 26 Jun 2021 04:26:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 26 Jun 2021 04:26:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 04:27:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 04:27:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 26 Jun 2021 06:47:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 26 Jun 2021 06:47:53 GMT
ENV PHP_VERSION=7.4.20
# Sat, 26 Jun 2021 06:47:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Sat, 26 Jun 2021 06:48:02 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Sat, 26 Jun 2021 06:49:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 26 Jun 2021 06:49:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 26 Jun 2021 06:57:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 26 Jun 2021 06:57:11 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Sat, 26 Jun 2021 06:57:22 GMT
RUN docker-php-ext-enable sodium
# Sat, 26 Jun 2021 06:57:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 26 Jun 2021 06:57:31 GMT
STOPSIGNAL SIGWINCH
# Sat, 26 Jun 2021 06:57:32 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 26 Jun 2021 06:57:36 GMT
WORKDIR /var/www/html
# Sat, 26 Jun 2021 06:57:39 GMT
EXPOSE 80
# Sat, 26 Jun 2021 06:57:48 GMT
CMD ["apache2-foreground"]
# Sun, 27 Jun 2021 14:22:01 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sun, 27 Jun 2021 14:22:03 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 27 Jun 2021 14:22:05 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 27 Jun 2021 14:36:13 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 27 Jun 2021 14:36:21 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 27 Jun 2021 14:36:24 GMT
VOLUME [/var/www/html]
# Sun, 27 Jun 2021 14:36:33 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Sun, 27 Jun 2021 15:03:55 GMT
ENV NEXTCLOUD_VERSION=20.0.10
# Sun, 27 Jun 2021 15:08:47 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 27 Jun 2021 15:08:53 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Sun, 27 Jun 2021 15:08:57 GMT
COPY multi:bb22a87f07ec65f9db22db69c1e13d98d1b6e10d12cf7747d547023b06cd53c6 in /usr/src/nextcloud/config/ 
# Sun, 27 Jun 2021 15:09:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 27 Jun 2021 15:09:14 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bede12a66c305ed12d280c6b7a6022061a73d9568433f643b06ec9893f790c0`  
		Last Modified: Sat, 26 Jun 2021 09:01:49 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b569ead47e80d494e6f64ea9e5b97bcc6a4d42355effc0aedead32f63c7ba733`  
		Last Modified: Sat, 26 Jun 2021 09:03:27 GMT  
		Size: 82.3 MB (82291015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b0e4b30eb84311f540a9331dfc8db99c35e188d1fc36e8862ed80fd320c431`  
		Last Modified: Sat, 26 Jun 2021 09:01:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0be226e932ae202655cabfbdf039de068fd0668bc10270960d28e04010caf9d`  
		Last Modified: Sat, 26 Jun 2021 09:04:48 GMT  
		Size: 19.8 MB (19818544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a6a8c2dc286478f193e642b39db64063501e03463223f793d17bf4b4d548a4`  
		Last Modified: Sat, 26 Jun 2021 09:04:35 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d8e7e98a0047f2938ddec0785e0b8a93b3b086bfd03f29c6d1a903ec5bfd69`  
		Last Modified: Sat, 26 Jun 2021 09:04:35 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931c67ae16a088c696ca4de739b4373c144383c23e33eeca0711ccb7a871ae00`  
		Last Modified: Sat, 26 Jun 2021 09:10:18 GMT  
		Size: 10.7 MB (10684121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822b6d5f0572a3d630fb8d07ded49c30aed0345c4c6c5489b8d8f4c0ca05f6eb`  
		Last Modified: Sat, 26 Jun 2021 09:10:11 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c62991100e1f2c2fc856fc83d7059c1fbcb12b0bd1226f2b319637cf2e6fd3a`  
		Last Modified: Sat, 26 Jun 2021 09:10:27 GMT  
		Size: 14.9 MB (14882100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:555f79c2120d673f292a061a5cdcc31e327e088fa9a47fd01b86e7213638df3d`  
		Last Modified: Sat, 26 Jun 2021 09:10:11 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e69fdd91ed5a20714126b3cd839a8799b3a3306ff654f2f163f645e9dab43`  
		Last Modified: Sat, 26 Jun 2021 09:10:11 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe96c712db820d2fe2df747bca19d4f7d47cec51d885312e83e99acf963edd2`  
		Last Modified: Sat, 26 Jun 2021 09:10:11 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0fa171b8b4dedf423841dfe608c2516a7be4fb9ca3730e375c8bfead49fe52`  
		Last Modified: Sun, 27 Jun 2021 15:26:58 GMT  
		Size: 1.8 MB (1827453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d548876e97dfdbf5c83f56c2df4b62335d1fb3de4cb679d46b5022f99c744c93`  
		Last Modified: Sun, 27 Jun 2021 15:27:16 GMT  
		Size: 15.9 MB (15928961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b23768728924b3c41dce9ae67acdee2e49e5c9654af387810f8066614cf671`  
		Last Modified: Sun, 27 Jun 2021 15:26:54 GMT  
		Size: 597.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5008ef2e2a3954b99b371e2e0c37b97a4bfc4b32111f554cf514ca2f4e90d70b`  
		Last Modified: Sun, 27 Jun 2021 15:26:54 GMT  
		Size: 583.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94093d2af3141340c08baac822cfcd5ae1debc37c200ac7aab0224130ceb989e`  
		Last Modified: Sun, 27 Jun 2021 15:38:29 GMT  
		Size: 132.5 MB (132539711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54158c1bcfbf60938e93a33c5fb09d5ac73094c31845188a2786baf6d1746357`  
		Last Modified: Sun, 27 Jun 2021 15:35:52 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ab0068d5c00e079d74de7543acdcba9f903b8ee08ca96eac93f7b4e4306fed`  
		Last Modified: Sun, 27 Jun 2021 15:35:52 GMT  
		Size: 2.1 KB (2061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:stable-apache` - linux; s390x

```console
$ docker pull nextcloud@sha256:912149c7800ef9310fb6bfa7dbf8fe82c43062415cc60e1d13b7d3a02d9da08f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.1 MB (281055385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b1e33653a5a8d198ac0d8811c876e7dc4dcc4ee07991ef502d3be72b7314c87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:28 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Tue, 22 Jun 2021 23:42:29 GMT
CMD ["bash"]
# Sat, 26 Jun 2021 00:09:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 26 Jun 2021 00:09:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 26 Jun 2021 00:10:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 26 Jun 2021 00:10:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 26 Jun 2021 00:10:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 26 Jun 2021 00:13:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 26 Jun 2021 00:13:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 26 Jun 2021 00:14:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 26 Jun 2021 00:14:08 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 26 Jun 2021 00:14:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 26 Jun 2021 00:14:09 GMT
ENV PHP_EXTRA_BUILD_DEPS=apache2-dev
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--with-apxs2 --disable-cgi
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 26 Jun 2021 00:14:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 26 Jun 2021 01:06:45 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 26 Jun 2021 01:06:46 GMT
ENV PHP_VERSION=7.4.20
# Sat, 26 Jun 2021 01:06:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.20.tar.xz.asc
# Sat, 26 Jun 2021 01:06:47 GMT
ENV PHP_SHA256=1fa46ca6790d780bf2cb48961df65f0ca3640c4533f0bca743cd61b71cb66335
# Sat, 26 Jun 2021 01:06:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 26 Jun 2021 01:06:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 26 Jun 2021 01:09:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 26 Jun 2021 01:09:39 GMT
COPY multi:e4407f0002276f00cc93b01e48696c1f677a5f7d3d194b3a84bec1cc5e733bcb in /usr/local/bin/ 
# Sat, 26 Jun 2021 01:09:40 GMT
RUN docker-php-ext-enable sodium
# Sat, 26 Jun 2021 01:09:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 26 Jun 2021 01:09:41 GMT
STOPSIGNAL SIGWINCH
# Sat, 26 Jun 2021 01:09:41 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 26 Jun 2021 01:09:42 GMT
WORKDIR /var/www/html
# Sat, 26 Jun 2021 01:09:42 GMT
EXPOSE 80
# Sat, 26 Jun 2021 01:09:42 GMT
CMD ["apache2-foreground"]
# Sun, 27 Jun 2021 14:19:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         busybox-static     ;     rm -rf /var/lib/apt/lists/*;         mkdir -p /var/spool/cron/crontabs;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Sun, 27 Jun 2021 14:19:45 GMT
ENV PHP_MEMORY_LIMIT=512M
# Sun, 27 Jun 2021 14:19:46 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Sun, 27 Jun 2021 14:22:56 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         libcurl4-openssl-dev         libevent-dev         libfreetype6-dev         libicu-dev         libjpeg-dev         libldap2-dev         libmcrypt-dev         libmemcached-dev         libpng-dev         libpq-dev         libxml2-dev         libmagickwand-dev         libzip-dev         libwebp-dev         libgmp-dev     ;         debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";     docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap --with-libdir="lib/$debMultiarch";     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;     rm -r /tmp/pear;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Sun, 27 Jun 2021 14:22:58 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/nextcloud.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Sun, 27 Jun 2021 14:22:59 GMT
VOLUME [/var/www/html]
# Sun, 27 Jun 2021 14:23:00 GMT
RUN a2enmod headers rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Sun, 27 Jun 2021 14:31:28 GMT
ENV NEXTCLOUD_VERSION=20.0.10
# Sun, 27 Jun 2021 14:32:17 GMT
RUN set -ex;     fetchDeps="         gnupg         dirmngr     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Sun, 27 Jun 2021 14:32:31 GMT
COPY multi:5c7d3e21c40c6f3326b9c24bb148355014771883d3bc821f8ada4fed6795cbb4 in / 
# Sun, 27 Jun 2021 14:32:33 GMT
COPY multi:bb22a87f07ec65f9db22db69c1e13d98d1b6e10d12cf7747d547023b06cd53c6 in /usr/src/nextcloud/config/ 
# Sun, 27 Jun 2021 14:32:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 27 Jun 2021 14:32:33 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61297595675dd5f94c60485ec6670e0d45420c73a569aebae232822f3805f5f4`  
		Last Modified: Sat, 26 Jun 2021 02:18:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ab5f68c432394e6815ad9808418b4300224b46b5898a0f90a1fedbfdf9ca7f`  
		Last Modified: Sat, 26 Jun 2021 02:18:46 GMT  
		Size: 64.7 MB (64710315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6def165c1dbb7cd43c8e70e00b2ec5aa53eae70056635c2ff93bdaf25ec061ef`  
		Last Modified: Sat, 26 Jun 2021 02:18:36 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b3e7236868c26c00547364caef50791abcea8d5a62d4fac4ff00f1acf28308`  
		Last Modified: Sat, 26 Jun 2021 02:19:14 GMT  
		Size: 18.5 MB (18525085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae502a4e5daabc91e5f674004c64396c939ee72f05af0b913531fd51c79a37e`  
		Last Modified: Sat, 26 Jun 2021 02:19:11 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c27e0c3d22fb08edda2488324e9cbcd02f8ff31f5bad766bdd1470e2ea7048`  
		Last Modified: Sat, 26 Jun 2021 02:19:11 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff862c3409a15e67fe100d54f446334d5e5088289a37bdff8a33d011f183253`  
		Last Modified: Sat, 26 Jun 2021 02:23:45 GMT  
		Size: 10.7 MB (10682460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9c17fdaf1feff3ea85fcf200ba2ce45434c548bb319dfb927f15a2c373ab96`  
		Last Modified: Sat, 26 Jun 2021 02:23:43 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ca6185f7686020a3571e52291db369da8bbf6bd35f821f4bd876562f660a98`  
		Last Modified: Sat, 26 Jun 2021 02:23:45 GMT  
		Size: 13.1 MB (13058175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a624e858b66340791f7bcfbbf96d93cdf5bb24f90362935edaeab2d4132561d`  
		Last Modified: Sat, 26 Jun 2021 02:23:43 GMT  
		Size: 2.3 KB (2276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ba4e686bbef14443fc43681122dc2b6d8ac52c391b77152b20b7fad62e4175`  
		Last Modified: Sat, 26 Jun 2021 02:23:43 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d168f29ad3eb612cea0fc38f50baa5d27c6dea1525eb86c02a97e49ce4f7d9`  
		Last Modified: Sat, 26 Jun 2021 02:23:43 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c8397796c70ac5a99b47f84321ff1d07a7c179695592f54c94fffe18a9b256`  
		Last Modified: Sun, 27 Jun 2021 14:39:38 GMT  
		Size: 1.6 MB (1618861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b913232a4d2f987f9f6e3646ca0a80932c80e5b75f715f4a0125b1405fcb1020`  
		Last Modified: Sun, 27 Jun 2021 14:39:39 GMT  
		Size: 14.2 MB (14153559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc92a783730f789297ba0b8ee5c3b0a7a9a15067f376a3e0bdbb7cbc44b2852d`  
		Last Modified: Sun, 27 Jun 2021 14:39:36 GMT  
		Size: 598.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e001532e9135e9428ff0e124a1478a8461394bf68ca99f8b5007649cb44dc616`  
		Last Modified: Sun, 27 Jun 2021 14:39:36 GMT  
		Size: 579.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c61a9be193f01adf460708a21b12bdbd99616cbf0b51467791363a7f0647ea8`  
		Last Modified: Sun, 27 Jun 2021 14:41:06 GMT  
		Size: 132.5 MB (132534959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1449e2c61ddc96678fb421f3b2080e16eaa55001c5821462927b99881d1b5d9e`  
		Last Modified: Sun, 27 Jun 2021 14:40:51 GMT  
		Size: 2.6 KB (2630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8106b2848291a517dd3093bf51a4cfaf662f0f0ea8ba30456c7eb7f215403f3`  
		Last Modified: Sun, 27 Jun 2021 14:40:51 GMT  
		Size: 2.1 KB (2058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
