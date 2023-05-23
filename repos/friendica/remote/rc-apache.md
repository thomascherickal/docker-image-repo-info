## `friendica:rc-apache`

```console
$ docker pull friendica@sha256:c057fbc336b08d3fdf6f31a1ef6a5c2ef6f68b7268ba095022ebf0ae8d307ce5
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

### `friendica:rc-apache` - linux; amd64

```console
$ docker pull friendica@sha256:9ce4fb51fff5a7051ffcd695fb87e32ec0902c146a4fa74fae084171a829d814
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.1 MB (216117947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fab7291191f387acb153f8129d61c1785215bf025af59ec15a8a26535334f88`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 May 2023 23:46:59 GMT
ADD file:a2378c1b12e95db69e24b9d347441678c6f23239292cce3c822b1524992b6ec4 in / 
# Tue, 02 May 2023 23:47:00 GMT
CMD ["bash"]
# Wed, 03 May 2023 04:37:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 03 May 2023 04:37:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 03 May 2023 04:37:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 04:37:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 03 May 2023 04:37:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 03 May 2023 04:41:02 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 03 May 2023 04:41:02 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 03 May 2023 04:41:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 03 May 2023 04:41:12 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 03 May 2023 04:41:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 03 May 2023 04:41:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 04:41:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 04:41:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 03 May 2023 06:27:02 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 03 May 2023 06:27:02 GMT
ENV PHP_VERSION=8.0.28
# Wed, 03 May 2023 06:27:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 03 May 2023 06:27:02 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 03 May 2023 06:27:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 03 May 2023 06:27:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 03 May 2023 06:30:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 03 May 2023 06:30:08 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 03 May 2023 06:30:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 03 May 2023 06:30:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 03 May 2023 06:30:09 GMT
STOPSIGNAL SIGWINCH
# Wed, 03 May 2023 06:30:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 03 May 2023 06:30:09 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 06:30:09 GMT
EXPOSE 80
# Wed, 03 May 2023 06:30:09 GMT
CMD ["apache2-foreground"]
# Thu, 04 May 2023 03:16:50 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 04 May 2023 03:16:50 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:17:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:19:33 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 03:19:33 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 04 May 2023 03:19:33 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 04 May 2023 03:19:34 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 04 May 2023 03:19:34 GMT
VOLUME [/var/www/html]
# Thu, 04 May 2023 03:19:34 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 04 May 2023 03:19:34 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 19 May 2023 19:19:43 GMT
ENV FRIENDICA_VERSION=2023.05-rc
# Fri, 19 May 2023 19:19:43 GMT
ENV FRIENDICA_ADDONS=2023.05-rc
# Fri, 19 May 2023 19:19:53 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;
# Fri, 19 May 2023 19:19:53 GMT
COPY multi:ab2651ad89391d4b701d7103fef240fe05356134f6401e4784d200f8bded3dd8 in / 
# Fri, 19 May 2023 19:19:53 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 19 May 2023 19:19:53 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Fri, 19 May 2023 19:19:53 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9e3ea8720c6de96cc9ad544dddc695a3ab73f5581c5d954e0504cc4f80fb5e5c`  
		Last Modified: Tue, 02 May 2023 23:50:22 GMT  
		Size: 31.4 MB (31403516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07353b772b5e325bf0abf03512cfaebe590a14a0858cf0ec2740b5ab055a31a7`  
		Last Modified: Wed, 03 May 2023 06:50:49 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908153120ba6d8988feadd5f6a8c68a281970ad001ac3be0f5bc9dc030b5c4d`  
		Last Modified: Wed, 03 May 2023 06:51:01 GMT  
		Size: 91.6 MB (91635527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8681ad2eeea6fa7d3aed97bcd471bddff6b4932f405ecb84452c3d2522390e2a`  
		Last Modified: Wed, 03 May 2023 06:50:49 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92711ce78973323920b717b53e3a3e197c7b958c6e1a1be2a69b72718519c96a`  
		Last Modified: Wed, 03 May 2023 06:51:31 GMT  
		Size: 19.2 MB (19248134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1c5be6427ed0108e9859238ab41d37f43b792c65758e165f1cb957e7c4ab45`  
		Last Modified: Wed, 03 May 2023 06:51:28 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d02a81768ed9803772d4654c2b55b24c54d1200a872fccc3b689b8dd84cebd9`  
		Last Modified: Wed, 03 May 2023 06:51:28 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d674a0135f85fa25714f9d22cc061f1e3743cd2274d0446b1943113027bb67a5`  
		Last Modified: Wed, 03 May 2023 07:01:33 GMT  
		Size: 11.1 MB (11142906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d87d03598175bfd15a7f8d90700ae62943df3c9be72b1434b7df1506e42bd32`  
		Last Modified: Wed, 03 May 2023 07:01:30 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8c2df9b69e488567399d647cb6e6cb0fe697131f891fb5210a5a9c91e24910`  
		Last Modified: Wed, 03 May 2023 07:01:32 GMT  
		Size: 10.8 MB (10775910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacfb138e3c154e9bd1ba67b86c7eebf6ab10d180f6e8ede5073b9e3c608c6e3`  
		Last Modified: Wed, 03 May 2023 07:01:31 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db2528ade336d6a364955db7f8f00b611f66e103ccebbc0ff8ce392861dbae7`  
		Last Modified: Wed, 03 May 2023 07:01:30 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beeef66f0c04e387386a2642675efa5b32bf6a5d69e9abe09896e07828508758`  
		Last Modified: Wed, 03 May 2023 07:01:30 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df939ca79b7491123ac0a9be39b1176dfa20edf1ce5c0801e7922549ef2a590`  
		Last Modified: Thu, 04 May 2023 03:23:49 GMT  
		Size: 15.6 MB (15558223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a5d46030eabebd5bd2c4c95934fd8cbba7b9ef4165cd51c3dc06f66d6fa863`  
		Last Modified: Thu, 04 May 2023 03:23:47 GMT  
		Size: 1.3 MB (1296661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055fec86bd3274c04367eb927e3cce6a7b1ecbe2e7d46c59c4f9a9221f86fb06`  
		Last Modified: Thu, 04 May 2023 03:23:50 GMT  
		Size: 17.9 MB (17852119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6808a56c84fa1e743c1cf0a3035bc4f68d6bab69878c2c076ec29b475765803`  
		Last Modified: Thu, 04 May 2023 03:23:45 GMT  
		Size: 640.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1596aaa2bb3153b58680e13a5ab820030b66fd9153f6784cab0ecc4c10b8443b`  
		Last Modified: Thu, 04 May 2023 03:23:45 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f23a8fc58efdbea33d9b73052391b71f534de334b52a58cd3937fbd7e8c2269`  
		Last Modified: Fri, 19 May 2023 19:21:18 GMT  
		Size: 17.2 MB (17193480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bdc85d73cbdf8200894590c5de763ec0d79cb0c82f063981c363406175dfd3a`  
		Last Modified: Fri, 19 May 2023 19:21:17 GMT  
		Size: 3.8 KB (3773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1efd708d2fc6d281a3082ac17f4791cf06a90616c357d629086d25d76c403f`  
		Last Modified: Fri, 19 May 2023 19:21:16 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:rc-apache` - linux; arm variant v5

```console
$ docker pull friendica@sha256:430bb041a4adcd55a0742759d819a0fc3eff35277b6c9288c9f5984e211a2d8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.4 MB (191357339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b63d9b07a869e762606abea7e761c30460fb9ac9f9d017ec885d12d496e1730`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 May 2023 22:48:53 GMT
ADD file:ca82c0d9094c1022a00b5f2157a02e1a9032aafc357a41c76c6b60bd74d25395 in / 
# Tue, 02 May 2023 22:48:53 GMT
CMD ["bash"]
# Wed, 03 May 2023 04:52:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 03 May 2023 04:52:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 03 May 2023 04:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 04:53:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 03 May 2023 04:53:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 03 May 2023 04:57:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 03 May 2023 04:57:06 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 03 May 2023 04:57:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 03 May 2023 04:57:18 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 03 May 2023 04:57:19 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 03 May 2023 04:57:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 04:57:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 04:57:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 03 May 2023 05:50:22 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 03 May 2023 05:50:22 GMT
ENV PHP_VERSION=8.0.28
# Wed, 03 May 2023 05:50:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 03 May 2023 05:50:23 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 03 May 2023 05:50:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 03 May 2023 05:50:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 03 May 2023 05:52:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 03 May 2023 05:52:53 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 03 May 2023 05:52:53 GMT
RUN docker-php-ext-enable sodium
# Wed, 03 May 2023 05:52:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 03 May 2023 05:52:54 GMT
STOPSIGNAL SIGWINCH
# Wed, 03 May 2023 05:52:54 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 03 May 2023 05:52:54 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 05:52:54 GMT
EXPOSE 80
# Wed, 03 May 2023 05:52:54 GMT
CMD ["apache2-foreground"]
# Wed, 03 May 2023 13:49:45 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Wed, 03 May 2023 13:49:46 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 May 2023 13:49:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 May 2023 13:52:21 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 13:52:21 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 03 May 2023 13:52:21 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 03 May 2023 13:52:22 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 03 May 2023 13:52:22 GMT
VOLUME [/var/www/html]
# Wed, 03 May 2023 13:52:22 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 03 May 2023 13:52:22 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 19 May 2023 19:49:24 GMT
ENV FRIENDICA_VERSION=2023.05-rc
# Fri, 19 May 2023 19:49:24 GMT
ENV FRIENDICA_ADDONS=2023.05-rc
# Fri, 19 May 2023 19:49:36 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;
# Fri, 19 May 2023 19:49:36 GMT
COPY multi:ab2651ad89391d4b701d7103fef240fe05356134f6401e4784d200f8bded3dd8 in / 
# Fri, 19 May 2023 19:49:36 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 19 May 2023 19:49:36 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Fri, 19 May 2023 19:49:37 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:eb6ee5d3f82142e70aca665cea92048b1a46ff1aa5c5be47a04c27a471470c07`  
		Last Modified: Tue, 02 May 2023 22:51:25 GMT  
		Size: 28.9 MB (28903418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85385d8a3476710ef72295538768f9c56689b7564ab9659e81ba54b2c44cd6ac`  
		Last Modified: Wed, 03 May 2023 05:58:33 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1055ef3089b9a2f598b1acf9be9ce3f9c8ca52737a33b747346c1d95163280eb`  
		Last Modified: Wed, 03 May 2023 05:58:46 GMT  
		Size: 73.7 MB (73687109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bce127d0f710a63a0c4f56d4db41b96c20ef29e12706dd814ad1791a03d4e78`  
		Last Modified: Wed, 03 May 2023 05:58:33 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5128568fc52dd737c8c7c6e4619d2d953f7823880670051fb58a3cd97f4f142f`  
		Last Modified: Wed, 03 May 2023 05:59:16 GMT  
		Size: 18.5 MB (18548530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3ea7ea903f65a529fc14b10916ebd2596aeab47d1938317742b4cd4879d69b`  
		Last Modified: Wed, 03 May 2023 05:59:12 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8260da688e16d2b01fda95e7d18674e0b415261617c9ab6ec78996b1015add03`  
		Last Modified: Wed, 03 May 2023 05:59:12 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e76a169e6ba8a3e3fa7f4510c18d739df1adf4d3de5b44ce809c14a02c698cc`  
		Last Modified: Wed, 03 May 2023 06:05:05 GMT  
		Size: 11.1 MB (11141296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5ed44202b7b045f43835747f11b56474ccd9c1e83ebaa98741ed10d200a399`  
		Last Modified: Wed, 03 May 2023 06:05:02 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89de207f7d4ba17c653c634e4645598d0f0bac9abf00dc4db20c2e39e62b238`  
		Last Modified: Wed, 03 May 2023 06:05:04 GMT  
		Size: 9.8 MB (9789589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df160b9595aa81059b8be0fe49ef1bd2cb78353b666323f3d66c9a3a9a7a91c9`  
		Last Modified: Wed, 03 May 2023 06:05:02 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fefb5eb7f12946eb453da70ce480698e71416940a3633834a62df88031739e`  
		Last Modified: Wed, 03 May 2023 06:05:02 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f3d926634d167a3b8af714426dae5fa317bee0feadb23e96d0b8f9d0cd67b1`  
		Last Modified: Wed, 03 May 2023 06:05:02 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3345b36a1c9b594359a9c32ba0dfba1d4d6b43970e8991854e4123f74d85273`  
		Last Modified: Wed, 03 May 2023 13:56:39 GMT  
		Size: 15.4 MB (15449326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a96614eea8970e1515b01d63d17eb944994ca377617a61df3ced4e00306417`  
		Last Modified: Wed, 03 May 2023 13:56:38 GMT  
		Size: 1.3 MB (1259289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482adbf13e872dfa850c0ad26ab04223a28f3992a0a91e01f5a4bbe3c8fdf417`  
		Last Modified: Wed, 03 May 2023 13:56:40 GMT  
		Size: 15.6 MB (15597411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d66a05a7849035e539bd61e2ceca4ba047137779ff0be90d3085ff8cbf5b5e9`  
		Last Modified: Wed, 03 May 2023 13:56:35 GMT  
		Size: 642.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce9fd9c53616fca4d2e8197733d20d9b36fe392759aba1ba78b9377a7c44ef5`  
		Last Modified: Wed, 03 May 2023 13:56:35 GMT  
		Size: 537.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a3483e9e2eded9ae2111b1131ec28140727e19e3019a938c6737cb27fe30e9`  
		Last Modified: Fri, 19 May 2023 19:50:41 GMT  
		Size: 17.0 MB (16969901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25f259ca3c2c88498898bc7dac21b2ecfe9f4e4d07a3867151564bf3b68529d`  
		Last Modified: Fri, 19 May 2023 19:50:40 GMT  
		Size: 3.8 KB (3773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbd6ceabddc0991a181f371654e54d162bafec1fc31da98d900337c0a4d990e`  
		Last Modified: Fri, 19 May 2023 19:50:39 GMT  
		Size: 946.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:rc-apache` - linux; arm variant v7

```console
$ docker pull friendica@sha256:3087736a5b55b1c606513231a30cecb06e25c120d7c301319864cb56ec96f42e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182483388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cfb5ded72eac4ebf6c1a42fe08f95d5c8ffbfd4edbacc21385d5a0fddf931d3`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 May 2023 23:47:57 GMT
ADD file:69d82e947b50a0f0ec610822ffe7c23ec1f6eb41bc17068502380f827cbcce40 in / 
# Tue, 02 May 2023 23:47:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 06:02:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 03 May 2023 06:02:40 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 03 May 2023 06:02:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 06:02:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 03 May 2023 06:02:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 03 May 2023 06:05:32 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 03 May 2023 06:05:32 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 03 May 2023 06:05:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 03 May 2023 06:05:44 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 03 May 2023 06:05:44 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 03 May 2023 06:05:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 06:05:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 06:05:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 03 May 2023 07:27:11 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 03 May 2023 07:27:12 GMT
ENV PHP_VERSION=8.0.28
# Wed, 03 May 2023 07:27:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 03 May 2023 07:27:12 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 03 May 2023 07:27:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 03 May 2023 07:27:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 03 May 2023 07:29:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 03 May 2023 07:29:29 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 03 May 2023 07:29:30 GMT
RUN docker-php-ext-enable sodium
# Wed, 03 May 2023 07:29:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 03 May 2023 07:29:30 GMT
STOPSIGNAL SIGWINCH
# Wed, 03 May 2023 07:29:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 03 May 2023 07:29:30 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 07:29:30 GMT
EXPOSE 80
# Wed, 03 May 2023 07:29:30 GMT
CMD ["apache2-foreground"]
# Thu, 04 May 2023 03:19:53 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 04 May 2023 03:19:53 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:20:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:22:38 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 03:22:38 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 04 May 2023 03:22:38 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 04 May 2023 03:22:38 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 04 May 2023 03:22:39 GMT
VOLUME [/var/www/html]
# Thu, 04 May 2023 03:22:39 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 04 May 2023 03:22:39 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 19 May 2023 19:09:46 GMT
ENV FRIENDICA_VERSION=2023.05-rc
# Fri, 19 May 2023 19:09:46 GMT
ENV FRIENDICA_ADDONS=2023.05-rc
# Fri, 19 May 2023 19:09:58 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;
# Fri, 19 May 2023 19:09:58 GMT
COPY multi:ab2651ad89391d4b701d7103fef240fe05356134f6401e4784d200f8bded3dd8 in / 
# Fri, 19 May 2023 19:09:58 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 19 May 2023 19:09:58 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Fri, 19 May 2023 19:09:58 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9c7c4e67baad3ce38491ce8c1ffaa9ca9ce37409270ce53ab3472054f35d097e`  
		Last Modified: Tue, 02 May 2023 23:51:30 GMT  
		Size: 26.6 MB (26564648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4223092dddf6040b9cb3d66826248ca3c50557af6320203e8a40b6e549bb0f2c`  
		Last Modified: Wed, 03 May 2023 07:46:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922e3f7fe606e6c4954d1d9e944c9f9e610ff10a76127e6d51a955e8cc42772b`  
		Last Modified: Wed, 03 May 2023 07:46:36 GMT  
		Size: 69.3 MB (69320181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3bf68a94eff4021eeb6ae2522f556ef8567c37e2fb6f1155469a278208edf3`  
		Last Modified: Wed, 03 May 2023 07:46:25 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70939fb624f471cb7fcaaa48c91697a6b8745045cfa06a955b53b7517a5f26c3`  
		Last Modified: Wed, 03 May 2023 07:47:00 GMT  
		Size: 18.0 MB (18007946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc2479125a48d14056528c5be7d389f2fb2b0977398a03fc50730f41f2944a26`  
		Last Modified: Wed, 03 May 2023 07:46:57 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c698e83c34140865f214984aca5d4ab163aa1df710e78e5df4fb286f2043e9e`  
		Last Modified: Wed, 03 May 2023 07:46:57 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec47d452f87cbba6f5ae35c1fd030c19586505f76e8fcf458454aeba80ee7f78`  
		Last Modified: Wed, 03 May 2023 07:56:55 GMT  
		Size: 11.1 MB (11141282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6495a9c7d22df04ddff3164fc71c9fbdb6595ebc60f3d6116c81c8f7d587c8f`  
		Last Modified: Wed, 03 May 2023 07:56:52 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da2dd95f296a4dc85bb83446f32f041abad42bb387a84ee0d507b46b8bcd343a`  
		Last Modified: Wed, 03 May 2023 07:56:55 GMT  
		Size: 9.3 MB (9306020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc8940b12102a6d233e3524fcb02ba54a16281339ed467b935de9b4b6e5b648`  
		Last Modified: Wed, 03 May 2023 07:56:53 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:567f7483c19ceab3fe882715c6b265b824ce685bc99b6e4e8608d758ca24d0f6`  
		Last Modified: Wed, 03 May 2023 07:56:52 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad0ffb8c0cbe0fb433b890d6297282ef5e7cc7d962e91c60065e77c7a401a92`  
		Last Modified: Wed, 03 May 2023 07:56:53 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82ef89dced54f23e766632cbbf3d3ed6e59477fefba70c8babd676ee8986a89`  
		Last Modified: Thu, 04 May 2023 03:26:32 GMT  
		Size: 15.5 MB (15523387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55264ee0a0a1df8f5caf2d8598237beaee3c5214b4d5aef05c2913435f076f30`  
		Last Modified: Thu, 04 May 2023 03:26:31 GMT  
		Size: 1.3 MB (1252297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614050b6881d273cbfa10a30a7872efe48434c47af5f9ba4a9849d60b43b7abf`  
		Last Modified: Thu, 04 May 2023 03:26:33 GMT  
		Size: 14.5 MB (14490038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbc64b649fff03894fd5a051c0b47b839150719334ba35a94607ba5c0c4246f2`  
		Last Modified: Thu, 04 May 2023 03:26:29 GMT  
		Size: 639.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1de8ede073b9c45f2077b924c37c69eb2d6d151250149a277f0dfb165c3386e`  
		Last Modified: Thu, 04 May 2023 03:26:29 GMT  
		Size: 535.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94a1eccef2940a9e5d544903efc07acdb189b41ccaff68d6c39b27322c33872`  
		Last Modified: Fri, 19 May 2023 19:11:19 GMT  
		Size: 16.9 MB (16866122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a8d1458cac1dfc9872b93af8dd42a8ca185c5974e25f2ea54258d685b73232`  
		Last Modified: Fri, 19 May 2023 19:11:17 GMT  
		Size: 3.8 KB (3773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b051732ebd1cb1ee1ecddc04ed0228c4db05e9e5139009c4d3b70ffb49a9789c`  
		Last Modified: Fri, 19 May 2023 19:11:17 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:rc-apache` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:707fa51dc702866d2f98d6710d9c09d21693674da88272d5f60c39e59ce41406
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.5 MB (206520739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76126e51f5b78503d9c7fd997f81fd8b976a7890c204ec7402e8c45986090dbd`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 03 May 2023 00:22:49 GMT
ADD file:66d4d9078579608530442620145336062a293cc19f159b154a63a1bcdcce3f4c in / 
# Wed, 03 May 2023 00:22:50 GMT
CMD ["bash"]
# Wed, 03 May 2023 03:52:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 03 May 2023 03:52:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 03 May 2023 03:52:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 03:52:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 03 May 2023 03:52:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 03 May 2023 03:56:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 03 May 2023 03:56:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 03 May 2023 03:56:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 03 May 2023 03:56:14 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 03 May 2023 03:56:14 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 03 May 2023 03:56:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 03:56:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 03:56:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 03 May 2023 05:33:29 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 03 May 2023 05:33:29 GMT
ENV PHP_VERSION=8.0.28
# Wed, 03 May 2023 05:33:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 03 May 2023 05:33:29 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 03 May 2023 05:33:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 03 May 2023 05:33:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 03 May 2023 05:35:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 03 May 2023 05:35:36 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 03 May 2023 05:35:37 GMT
RUN docker-php-ext-enable sodium
# Wed, 03 May 2023 05:35:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 03 May 2023 05:35:37 GMT
STOPSIGNAL SIGWINCH
# Wed, 03 May 2023 05:35:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 03 May 2023 05:35:37 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 05:35:37 GMT
EXPOSE 80
# Wed, 03 May 2023 05:35:37 GMT
CMD ["apache2-foreground"]
# Wed, 03 May 2023 23:41:37 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Wed, 03 May 2023 23:41:38 GMT
ENV GOSU_VERSION=1.14
# Wed, 03 May 2023 23:41:46 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 03 May 2023 23:43:51 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 23:43:51 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 03 May 2023 23:43:52 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 03 May 2023 23:43:52 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 03 May 2023 23:43:52 GMT
VOLUME [/var/www/html]
# Wed, 03 May 2023 23:43:53 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 03 May 2023 23:43:53 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 19 May 2023 20:00:50 GMT
ENV FRIENDICA_VERSION=2023.05-rc
# Fri, 19 May 2023 20:00:50 GMT
ENV FRIENDICA_ADDONS=2023.05-rc
# Fri, 19 May 2023 20:00:54 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;
# Fri, 19 May 2023 20:00:55 GMT
COPY multi:ab2651ad89391d4b701d7103fef240fe05356134f6401e4784d200f8bded3dd8 in / 
# Fri, 19 May 2023 20:00:55 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 19 May 2023 20:00:55 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Fri, 19 May 2023 20:00:55 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:b5d25b35c1dbfa256bea3dd164b2048d6c7f8074a555213c493c36f07bf4c559`  
		Last Modified: Wed, 03 May 2023 00:25:53 GMT  
		Size: 30.1 MB (30052733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3582e155c24272674265389c3b317b84bec7ca237a6761ee690aed30a1c5ec9`  
		Last Modified: Wed, 03 May 2023 05:50:53 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313de6edf03aac188b999f642b424cdc014f9f45e218d5ad620a727ef81fa7e1`  
		Last Modified: Wed, 03 May 2023 05:51:02 GMT  
		Size: 86.9 MB (86928311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a576c500430404ceffd53e7ce6f2898b260e011e85c77bdabd75342c1a6a54`  
		Last Modified: Wed, 03 May 2023 05:50:53 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249c4246fc75d4a1eefb130895fc367d8150e7076da4e329f94094a45c81cf4e`  
		Last Modified: Wed, 03 May 2023 05:51:26 GMT  
		Size: 19.2 MB (19170211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dbc677cfb25a8634144c25b4c4f43c1173f08ca1eb16b4f3ae53aa11bc62040`  
		Last Modified: Wed, 03 May 2023 05:51:24 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca53ccc29d8c43aeff9c96a48096d009ccf0ee902bf0b5076defe39003f2a0e`  
		Last Modified: Wed, 03 May 2023 05:51:24 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81fde7a89e62b6048c9cb62c2ffe6af63c3083044645e382ea6a6ad99c1cac5`  
		Last Modified: Wed, 03 May 2023 06:01:01 GMT  
		Size: 11.1 MB (11142070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65465ad9ad827553311e6e589e563ab48e70b441b6a369b15163ab326c3a62b3`  
		Last Modified: Wed, 03 May 2023 06:00:59 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7f5fcc23917c72adb8430fc98e44fa15e6f0487bc44078a92955a1bb6adfa8`  
		Last Modified: Wed, 03 May 2023 06:01:00 GMT  
		Size: 10.2 MB (10233356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2e89a0acdeb3cb212a47433f7ccdaf15b941e51127926df285895723e903b4`  
		Last Modified: Wed, 03 May 2023 06:00:59 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56acc6a80c81b29997974b32b1455395b67a8602e8f6e2a28932dfb7ab58eea2`  
		Last Modified: Wed, 03 May 2023 06:00:59 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03cfc6f00bd090afde0726e6b7a4fe9caaca71065629f4ef636659f988f96052`  
		Last Modified: Wed, 03 May 2023 06:00:59 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b376ef14f1505593eae27f2c768de6e2dd69d5b14d65cabdc1288320e38f6a`  
		Last Modified: Wed, 03 May 2023 23:47:17 GMT  
		Size: 15.3 MB (15321501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f732cf67463ac8d2eb9f01780ca80f17720013ba2ec064f6b63f8442f9244f27`  
		Last Modified: Wed, 03 May 2023 23:47:16 GMT  
		Size: 1.2 MB (1223571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35ea9d103b537e8a1a73cdd955166e7a2925b192703a52e74f5beac1c0abfe2`  
		Last Modified: Wed, 03 May 2023 23:47:17 GMT  
		Size: 15.4 MB (15449085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af98d0e1cadc0f8302deeb581b15ec183a225544a5bb22fe173285379971aa5`  
		Last Modified: Wed, 03 May 2023 23:47:14 GMT  
		Size: 639.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7dc98385aba23ec4789d2933d11871ff6fd25979ef8b4d727d77b15cef2eec`  
		Last Modified: Wed, 03 May 2023 23:47:14 GMT  
		Size: 534.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c82d00d29e452dab242816629ef584e35c5776da6e7327d32c95081108cfad`  
		Last Modified: Fri, 19 May 2023 20:02:11 GMT  
		Size: 17.0 MB (16988450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94771d4c5a3bb53f18851065050d3e26c3e604f569802579236259db8d9d965`  
		Last Modified: Fri, 19 May 2023 20:02:11 GMT  
		Size: 3.8 KB (3773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dd6d9b239943b475bb00f40c81bb971f0161770604a93caf7eddc6e393701f`  
		Last Modified: Fri, 19 May 2023 20:02:10 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:rc-apache` - linux; 386

```console
$ docker pull friendica@sha256:c42511b9b97479c645ca7ce5a561f889192c16fb32b5505d14ca6de11f350465
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.3 MB (219321777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:978c39b098905eacf2ab9af445440c28894509b969135556f3ca13ec642b8509`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 03 May 2023 00:00:58 GMT
ADD file:caea439e2dbe0148904e3b9a0c5a843d2d0b7c196725d2b41790594e64dcdce8 in / 
# Wed, 03 May 2023 00:00:58 GMT
CMD ["bash"]
# Wed, 03 May 2023 08:55:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 03 May 2023 08:55:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 03 May 2023 08:56:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 08:56:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 03 May 2023 08:56:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 03 May 2023 09:01:39 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 03 May 2023 09:01:39 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 03 May 2023 09:01:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 03 May 2023 09:01:51 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 03 May 2023 09:01:52 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 03 May 2023 09:01:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 09:01:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 09:01:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 03 May 2023 11:50:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 03 May 2023 11:50:10 GMT
ENV PHP_VERSION=8.0.28
# Wed, 03 May 2023 11:50:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 03 May 2023 11:50:10 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 03 May 2023 11:50:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 03 May 2023 11:50:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 03 May 2023 11:55:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 03 May 2023 11:55:17 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 03 May 2023 11:55:17 GMT
RUN docker-php-ext-enable sodium
# Wed, 03 May 2023 11:55:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 03 May 2023 11:55:17 GMT
STOPSIGNAL SIGWINCH
# Wed, 03 May 2023 11:55:18 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 03 May 2023 11:55:18 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 11:55:18 GMT
EXPOSE 80
# Wed, 03 May 2023 11:55:18 GMT
CMD ["apache2-foreground"]
# Thu, 04 May 2023 02:37:39 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 04 May 2023 02:37:39 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 02:37:51 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 02:40:45 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 02:40:45 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 04 May 2023 02:40:45 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 04 May 2023 02:40:46 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 04 May 2023 02:40:46 GMT
VOLUME [/var/www/html]
# Thu, 04 May 2023 02:40:47 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 04 May 2023 02:40:47 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 19 May 2023 19:40:24 GMT
ENV FRIENDICA_VERSION=2023.05-rc
# Fri, 19 May 2023 19:40:24 GMT
ENV FRIENDICA_ADDONS=2023.05-rc
# Fri, 19 May 2023 19:40:33 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;
# Fri, 19 May 2023 19:40:33 GMT
COPY multi:ab2651ad89391d4b701d7103fef240fe05356134f6401e4784d200f8bded3dd8 in / 
# Fri, 19 May 2023 19:40:34 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 19 May 2023 19:40:34 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Fri, 19 May 2023 19:40:34 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:10b34014bd1c165cc57a10e7492f17dce658513b7329319fe6c193c85bf752db`  
		Last Modified: Wed, 03 May 2023 00:05:12 GMT  
		Size: 32.4 MB (32388208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e767304c8a25a06c5180cd0487b1d298c8eb93b9276d7f8a33605daeec5deed`  
		Last Modified: Wed, 03 May 2023 12:27:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8469e5ef909b43afbcce2cb261155375a3b3f423dadb11383bf91b8d037358f`  
		Last Modified: Wed, 03 May 2023 12:28:07 GMT  
		Size: 92.7 MB (92719962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d946dbb11b755f5978864d6cb1f395dc513c314f5d182df53bd573895bbeb7a5`  
		Last Modified: Wed, 03 May 2023 12:27:47 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924158f9311822c03627e43631de70ccf581b97a0430f7b72985bb4724547e87`  
		Last Modified: Wed, 03 May 2023 12:28:33 GMT  
		Size: 19.7 MB (19737280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace747d85a92d8e6182f02d61b25843d51b0e593121c7df2951fb700f4a49e55`  
		Last Modified: Wed, 03 May 2023 12:28:29 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cb964761efe81d0142e55a3784ad2802e32884c20d5859d2443482372701fa`  
		Last Modified: Wed, 03 May 2023 12:28:29 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec181025602d9b5319276036182dbc708b01d9aded2dd675b4aa55cde30c47e1`  
		Last Modified: Wed, 03 May 2023 12:39:45 GMT  
		Size: 11.1 MB (11142130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a49f575098ae44e020f1a87fb77d00c18a184bb0e3f84b24b039fb7d77dd9c4`  
		Last Modified: Wed, 03 May 2023 12:39:42 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039fde4b9a9f6169c1fc4921bde107d911adcada5692a370757606639ba3aa61`  
		Last Modified: Wed, 03 May 2023 12:39:45 GMT  
		Size: 11.0 MB (10981835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c632c1ff89860bcb0f45db1a4f4c20d69335bbc952f5f0846d8fe973c3e7e59e`  
		Last Modified: Wed, 03 May 2023 12:39:42 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b9f84b019d6bb5293bd7f47e4b19403d92268537a602bd895016170654cfbc`  
		Last Modified: Wed, 03 May 2023 12:39:42 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceebd725582d8d670a68d1a4f739676d4ea5bc3dc5e808783581d802c69621c7`  
		Last Modified: Wed, 03 May 2023 12:39:42 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fc85a1a30624577f021ba77c35dba994e4cb826fc6ff47c9aa729b7caf4e65`  
		Last Modified: Thu, 04 May 2023 02:45:36 GMT  
		Size: 16.0 MB (16027260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b7930fb605911f3d4716e2e02e19d5e79129ff80817339d5cd04157e578dda`  
		Last Modified: Thu, 04 May 2023 02:45:34 GMT  
		Size: 1.3 MB (1262448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c1a90735a5896ca7a9bd4a84b52d641e2bedf0d443b9d5c939a8c709c5b096`  
		Last Modified: Thu, 04 May 2023 02:45:38 GMT  
		Size: 17.1 MB (17120707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f3e1b04e92ce19c097491346f1ff35fa1afd5051a58d93961e2512dada0dd2`  
		Last Modified: Thu, 04 May 2023 02:45:31 GMT  
		Size: 640.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50504bb9714753c43e7cc0b4c6f41d0d19f29baac92c47e5eda42e1832980c08`  
		Last Modified: Thu, 04 May 2023 02:45:31 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a37cd078ed5cc31dd1b08a8f9cdc3559d0a4fb96677834bb27f962acdd4e12`  
		Last Modified: Fri, 19 May 2023 19:41:59 GMT  
		Size: 17.9 MB (17930471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a40397ef50b7e2419cc33460cfde127326ab47d3f840cd9946d90a1ade23bda`  
		Last Modified: Fri, 19 May 2023 19:41:57 GMT  
		Size: 3.8 KB (3773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0190c6a9c8360adec0636f61b380644acc440a6805f4ed91d6bac86b6e3c5f3`  
		Last Modified: Fri, 19 May 2023 19:41:57 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:rc-apache` - linux; mips64le

```console
$ docker pull friendica@sha256:5f50caac6b41b5af66f10018c0a7dba2466ee7ba961957e9651d3487f844f094
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.3 MB (189295166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:344d7cb550ca880816583696b60b50939966503d3fc39c40019b29541f713eb2`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 May 2023 23:49:45 GMT
ADD file:c3427ec4e3a2c988fdd372b529660d45ee105e317d6a964ce96f8f9009a3c21e in / 
# Tue, 02 May 2023 23:49:49 GMT
CMD ["bash"]
# Wed, 03 May 2023 00:10:52 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 03 May 2023 00:10:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 03 May 2023 00:12:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 00:12:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 03 May 2023 00:12:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 03 May 2023 00:27:42 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 03 May 2023 00:27:46 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 03 May 2023 00:28:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 03 May 2023 00:28:49 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 03 May 2023 00:28:55 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 03 May 2023 00:28:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 00:29:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 00:29:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 03 May 2023 04:19:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 03 May 2023 04:19:51 GMT
ENV PHP_VERSION=8.0.28
# Wed, 03 May 2023 04:19:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 03 May 2023 04:19:58 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 03 May 2023 04:20:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 03 May 2023 04:20:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 03 May 2023 04:34:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 03 May 2023 04:34:22 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 03 May 2023 04:34:28 GMT
RUN docker-php-ext-enable sodium
# Wed, 03 May 2023 04:34:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 03 May 2023 04:34:36 GMT
STOPSIGNAL SIGWINCH
# Wed, 03 May 2023 04:34:39 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 03 May 2023 04:34:43 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 04:34:46 GMT
EXPOSE 80
# Wed, 03 May 2023 04:34:50 GMT
CMD ["apache2-foreground"]
# Thu, 04 May 2023 03:14:03 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 04 May 2023 03:14:07 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 03:14:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 03:26:12 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 03:26:16 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 04 May 2023 03:26:19 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 04 May 2023 03:26:25 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 04 May 2023 03:26:29 GMT
VOLUME [/var/www/html]
# Thu, 04 May 2023 03:26:36 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 04 May 2023 03:26:40 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 19 May 2023 19:08:52 GMT
ENV FRIENDICA_VERSION=2023.05-rc
# Fri, 19 May 2023 19:08:56 GMT
ENV FRIENDICA_ADDONS=2023.05-rc
# Fri, 19 May 2023 19:09:36 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;
# Fri, 19 May 2023 19:09:40 GMT
COPY multi:ab2651ad89391d4b701d7103fef240fe05356134f6401e4784d200f8bded3dd8 in / 
# Fri, 19 May 2023 19:09:44 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 19 May 2023 19:09:48 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Fri, 19 May 2023 19:09:52 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:498edd615f8781385e0d5246e189d80b5caceb207fe26608a12605d0a823d4df`  
		Last Modified: Tue, 02 May 2023 23:58:10 GMT  
		Size: 29.6 MB (29623482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9f275f462bc69ed3d423529b2c61717acf92ae94079820567546a9be7dfc90`  
		Last Modified: Wed, 03 May 2023 05:03:18 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144d8ba9239413b7073602141f7770aa1ecefc91eea8b88d6bef1e57cd24e721`  
		Last Modified: Wed, 03 May 2023 05:04:11 GMT  
		Size: 72.0 MB (72018435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926473715e8c6e64ac6be14864c39343324c6cd9496c16cf520fac2ee94cafda`  
		Last Modified: Wed, 03 May 2023 05:03:17 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287b54b2fc0e2ddfd944a13aed3214414be47643ec0dd994e526c66d6164caab`  
		Last Modified: Wed, 03 May 2023 05:04:50 GMT  
		Size: 18.9 MB (18947010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9724b961784537f2a20fe86f36e2cc87ce7aee7c70f18e9010c2d4814cc66346`  
		Last Modified: Wed, 03 May 2023 05:04:37 GMT  
		Size: 439.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceec3ed73b30dcb9b15eb29224da2ee99fb658f743acf7882099046b54abcfb9`  
		Last Modified: Wed, 03 May 2023 05:04:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa294dd9cb7acdd34bfd09030ddf7a0d00a16111f3ad9f688b6f2c4bb056b26d`  
		Last Modified: Wed, 03 May 2023 05:14:02 GMT  
		Size: 10.9 MB (10924998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a607e98d99007bf96413f2ad1cb7e69cde0acd7e7c5cff3fbc960ddac55c04`  
		Last Modified: Wed, 03 May 2023 05:13:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed4c0e57644198ca9bd4401abdf0019689bf2caebd1ffcf6ed37f72161ca0d4a`  
		Last Modified: Wed, 03 May 2023 05:14:05 GMT  
		Size: 9.9 MB (9918380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b622a28ca466bd596b22441ea5b01b979ab702c9b702ab256984a8d8f2eb1b30`  
		Last Modified: Wed, 03 May 2023 05:13:58 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebbbbabf7e4a7fe2dfafe45d6af125bc5f55608536ea28eb8f2cd8381ab449c`  
		Last Modified: Wed, 03 May 2023 05:13:57 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4959048198b901ca03321edcb663e86ab50d9b97910ec9abb98610dd36146a34`  
		Last Modified: Wed, 03 May 2023 05:13:57 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729ec9ee2b76988ccb561cb54040f677d807bb74b25e9de370f407ff0f224493`  
		Last Modified: Thu, 04 May 2023 03:46:03 GMT  
		Size: 15.0 MB (15024015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7494c87a310d97cdbe37473db450af64ba07381837f2a4a4c1b161656719fdfc`  
		Last Modified: Thu, 04 May 2023 03:45:56 GMT  
		Size: 947.5 KB (947500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87b33e75b5538d32903230c9e88329612a470ed5cd241ee11b888199566f553`  
		Last Modified: Thu, 04 May 2023 03:46:06 GMT  
		Size: 15.4 MB (15405157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44afe2bbc359b8c56acc4011d0de8163cff19a1f6e35509f79f20401d19449ec`  
		Last Modified: Thu, 04 May 2023 03:45:53 GMT  
		Size: 612.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c72aec62f0ca2de9adf63085c268b70205aede0eb7484475c516705bb0b7d2`  
		Last Modified: Thu, 04 May 2023 03:45:54 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66780a79f745a8132508ec8045b7add73f217f05f37b527de31deb6334f3d91`  
		Last Modified: Fri, 19 May 2023 19:12:51 GMT  
		Size: 16.5 MB (16474851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8e271ddbabb08c8da41bcbb394efc69275ad074bd4eb883f2c0ba05dd0eef2`  
		Last Modified: Fri, 19 May 2023 19:12:44 GMT  
		Size: 3.8 KB (3774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03857961156c2669697ac28ae7673ac3355a03ee019d825ca0c325dc392d3e72`  
		Last Modified: Fri, 19 May 2023 19:12:44 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:rc-apache` - linux; ppc64le

```console
$ docker pull friendica@sha256:9bfbab716a050fe25b85d66fd543702b65f0e8c9a4d8fa1120b534c31b0d5da2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.1 MB (216117938 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b093d299d1e9bc7ddecf5d0185662c488c8f7b3f454fa2a9435b4aa9520107fb`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 03 May 2023 00:31:50 GMT
ADD file:ee3b3c43add645e1a2078f2a6e8544d223abf2754eb8039cbbc2cbdb911b49bb in / 
# Wed, 03 May 2023 00:31:52 GMT
CMD ["bash"]
# Wed, 03 May 2023 06:59:15 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 03 May 2023 06:59:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 03 May 2023 07:00:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 07:00:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 03 May 2023 07:00:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 03 May 2023 07:05:25 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 03 May 2023 07:05:25 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 03 May 2023 07:05:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 03 May 2023 07:05:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 03 May 2023 07:05:53 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 03 May 2023 07:05:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 07:05:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 03 May 2023 07:05:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 03 May 2023 08:26:29 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 03 May 2023 08:26:29 GMT
ENV PHP_VERSION=8.0.28
# Wed, 03 May 2023 08:26:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 03 May 2023 08:26:30 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 03 May 2023 08:26:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 03 May 2023 08:26:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 03 May 2023 08:31:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 03 May 2023 08:31:19 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 03 May 2023 08:31:21 GMT
RUN docker-php-ext-enable sodium
# Wed, 03 May 2023 08:31:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 03 May 2023 08:31:23 GMT
STOPSIGNAL SIGWINCH
# Wed, 03 May 2023 08:31:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 03 May 2023 08:31:25 GMT
WORKDIR /var/www/html
# Wed, 03 May 2023 08:31:26 GMT
EXPOSE 80
# Wed, 03 May 2023 08:31:27 GMT
CMD ["apache2-foreground"]
# Thu, 04 May 2023 08:06:36 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 04 May 2023 08:06:37 GMT
ENV GOSU_VERSION=1.14
# Thu, 04 May 2023 08:07:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 04 May 2023 08:13:10 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 08:13:11 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 04 May 2023 08:13:11 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 04 May 2023 08:13:12 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 04 May 2023 08:13:13 GMT
VOLUME [/var/www/html]
# Thu, 04 May 2023 08:13:15 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 04 May 2023 08:13:15 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 19 May 2023 19:16:49 GMT
ENV FRIENDICA_VERSION=2023.05-rc
# Fri, 19 May 2023 19:16:49 GMT
ENV FRIENDICA_ADDONS=2023.05-rc
# Fri, 19 May 2023 19:17:12 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;
# Fri, 19 May 2023 19:17:14 GMT
COPY multi:ab2651ad89391d4b701d7103fef240fe05356134f6401e4784d200f8bded3dd8 in / 
# Fri, 19 May 2023 19:17:15 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 19 May 2023 19:17:15 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Fri, 19 May 2023 19:17:16 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e39c6de44f96d2720b144cbaa9e763eac60a69222a96279f3962e8a701fb17ac`  
		Last Modified: Wed, 03 May 2023 00:36:56 GMT  
		Size: 35.3 MB (35280910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20bccc47384e79d6ab7c10c3eb8337f748e92318727cd43299e1acc121c8a6a3`  
		Last Modified: Wed, 03 May 2023 08:42:06 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c6b95d1f286a638f31ec2a11270e8db85c1c105b3ea97bd589725cbf56207f`  
		Last Modified: Wed, 03 May 2023 08:42:30 GMT  
		Size: 86.6 MB (86634643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b409adc42e9a9872675518e3bd6a1dfe2afc2eb0a918e614a2739abccd4ca062`  
		Last Modified: Wed, 03 May 2023 08:42:05 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2dc55b06b53d18eca789c75f4c6481afd7c6bdf071e6a9faed73102bb5d248`  
		Last Modified: Wed, 03 May 2023 08:43:00 GMT  
		Size: 20.5 MB (20463865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c99c2da17d1ba093f3a3c35e4678f14046afd50005e3c1b473be99971da670`  
		Last Modified: Wed, 03 May 2023 08:42:56 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d048ef0a01a953cfdd6e57cce47bef05bf65faad8fa4a4225a6308040207f2f`  
		Last Modified: Wed, 03 May 2023 08:42:56 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aabb3d4d48cdcba28134beb0385da6c55be617361be5d4d3aac66e21845e9ac`  
		Last Modified: Wed, 03 May 2023 08:50:33 GMT  
		Size: 11.1 MB (11142828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08026c603120f7ba90567ccf5df98b02de9f3e0b8851e5f89c23fd5f6db46c07`  
		Last Modified: Wed, 03 May 2023 08:50:29 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ed27df75ef52231ce6cd5fad4d54624306db959bf5e6c667e08b488dad715e`  
		Last Modified: Wed, 03 May 2023 08:50:33 GMT  
		Size: 11.1 MB (11139980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f756f8cefea95628d2e776d1ca7de6dd8299def750dc3c4d7f226bbb11d53f9f`  
		Last Modified: Wed, 03 May 2023 08:50:30 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2636ae3c5da61b62ea6f909cf5c14a618cf4048900270808e05d9613aca99f3`  
		Last Modified: Wed, 03 May 2023 08:50:29 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9322bb255f086aa69b54220c6db07d06d37590fc226ecc114bf92e1041a6bfc`  
		Last Modified: Wed, 03 May 2023 08:50:30 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a6596adf108c22aaee375824935cbea1014e3607f6f34642d505cbac770e3f`  
		Last Modified: Thu, 04 May 2023 08:24:06 GMT  
		Size: 15.4 MB (15448367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0420603b9072616db953e4bf0144c011b097e5e5b1382e07c9026b5a2e29b8ce`  
		Last Modified: Thu, 04 May 2023 08:24:01 GMT  
		Size: 1.2 MB (1196283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fe241f2e49373aa0b8aad5af1262a02a827cdf2876924fcb6c8c663955a659`  
		Last Modified: Thu, 04 May 2023 08:24:05 GMT  
		Size: 17.3 MB (17305114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10561591af7ce0c08eeb6001d7f3d78252d6de6c11a87bf73c25fb1e0c391601`  
		Last Modified: Thu, 04 May 2023 08:23:58 GMT  
		Size: 644.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c3f5c624bebbbd1745bbea68d93f7508a4cbe4f7446f898be6afc108e5683c`  
		Last Modified: Thu, 04 May 2023 08:23:58 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee07316a6dc70d0e3d76c17c053a476b59d757b3b2c8585c9ea82755af64220d`  
		Last Modified: Fri, 19 May 2023 19:19:35 GMT  
		Size: 17.5 MB (17494458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721010479dc158d1fa4004271fc3383b94166b5cfacdfcce764c7199dc5e6c00`  
		Last Modified: Fri, 19 May 2023 19:19:32 GMT  
		Size: 3.8 KB (3773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6620226eff6fa929009424ca00b6ec68131ee9cebefd9394611eca0ac8788b0a`  
		Last Modified: Fri, 19 May 2023 19:19:32 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:rc-apache` - linux; s390x

```console
$ docker pull friendica@sha256:eb6270f3d2a6717a664be58fce8fb7a1e5e9bedcc9662057ae6bc471e2377b89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189615637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f0ea27f4d8746b2dacf2fb794f561aead5cfb572360898babe524aed33d2334`
-	Entrypoint: `["\/entrypoint-dev.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 23 May 2023 00:42:52 GMT
ADD file:23b1e12559302529556a94a1d4098dbdb454e263265258b940c2b2d23a97c121 in / 
# Tue, 23 May 2023 00:42:54 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:07:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 23 May 2023 01:07:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 23 May 2023 01:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 01:07:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 23 May 2023 01:07:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 23 May 2023 01:10:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 23 May 2023 01:10:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 23 May 2023 01:10:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 23 May 2023 01:10:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 23 May 2023 01:10:36 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 23 May 2023 01:10:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 23 May 2023 01:10:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 23 May 2023 01:10:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 23 May 2023 01:29:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 23 May 2023 01:29:47 GMT
ENV PHP_VERSION=8.0.28
# Tue, 23 May 2023 01:29:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Tue, 23 May 2023 01:29:47 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Tue, 23 May 2023 01:29:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 May 2023 01:29:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 23 May 2023 01:31:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 23 May 2023 01:31:51 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 23 May 2023 01:31:52 GMT
RUN docker-php-ext-enable sodium
# Tue, 23 May 2023 01:31:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 23 May 2023 01:31:52 GMT
STOPSIGNAL SIGWINCH
# Tue, 23 May 2023 01:31:52 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 23 May 2023 01:31:52 GMT
WORKDIR /var/www/html
# Tue, 23 May 2023 01:31:52 GMT
EXPOSE 80
# Tue, 23 May 2023 01:31:52 GMT
CMD ["apache2-foreground"]
# Tue, 23 May 2023 06:12:17 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Tue, 23 May 2023 06:12:17 GMT
ENV GOSU_VERSION=1.14
# Tue, 23 May 2023 06:12:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 23 May 2023 06:13:54 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 06:13:55 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 23 May 2023 06:13:55 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 23 May 2023 06:13:55 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 23 May 2023 06:13:55 GMT
VOLUME [/var/www/html]
# Tue, 23 May 2023 06:13:56 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 23 May 2023 06:13:56 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Tue, 23 May 2023 06:16:45 GMT
ENV FRIENDICA_VERSION=2023.05-rc
# Tue, 23 May 2023 06:16:45 GMT
ENV FRIENDICA_ADDONS=2023.05-rc
# Tue, 23 May 2023 06:16:50 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;
# Tue, 23 May 2023 06:16:50 GMT
COPY multi:ab2651ad89391d4b701d7103fef240fe05356134f6401e4784d200f8bded3dd8 in / 
# Tue, 23 May 2023 06:16:50 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Tue, 23 May 2023 06:16:50 GMT
ENTRYPOINT ["/entrypoint-dev.sh"]
# Tue, 23 May 2023 06:16:51 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9c24ec455bdb6a9ad0d033c7cce8e71dd5bdbbe53a86d5feeb8d4cb7804fb8e5`  
		Last Modified: Tue, 23 May 2023 00:45:47 GMT  
		Size: 29.6 MB (29642170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d27dd5cb9d12b69f6b3a8ef6420e891e00651a39048f108f65bca58f76426e`  
		Last Modified: Tue, 23 May 2023 01:37:50 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c98bc8f44cf54884e2d9ff3ea62429882b6c2f1acb86c14341b903b8a6e2df`  
		Last Modified: Tue, 23 May 2023 01:38:00 GMT  
		Size: 71.6 MB (71630003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74336822dfa7773e397173bf2693f4155c5902c1d6f82cc0c056b9f8dad792ed`  
		Last Modified: Tue, 23 May 2023 01:37:50 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6453929ef3234fa275df321d07596c5d9b9c9d11f742fec2bd02f55d4e58d6f5`  
		Last Modified: Tue, 23 May 2023 01:38:24 GMT  
		Size: 19.1 MB (19077548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d4dfb9ac6ff0cba5d45b17d9423e603bfbe338045f6b0a02289a6f0ea73d4b`  
		Last Modified: Tue, 23 May 2023 01:38:22 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3c886ef3fb568f6fdba20ebb9783d3d19dc8976f73ea5688ef419d3350de9b`  
		Last Modified: Tue, 23 May 2023 01:38:22 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788c42e49144477f019392a3a6311346a0f3343651241eddfeaac5b95cb69d49`  
		Last Modified: Tue, 23 May 2023 01:40:44 GMT  
		Size: 11.1 MB (11141695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef62f2ad48f405a68d12eb00a75ba7a0b0542f7022b966373984873d048e718`  
		Last Modified: Tue, 23 May 2023 01:40:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816715da9972623090d15b27f7a8961e7b321598611526325c5c2727b3a5db43`  
		Last Modified: Tue, 23 May 2023 01:40:45 GMT  
		Size: 9.9 MB (9923775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c5e9530afb589953609ebae5f88fa00abbf8220b0adc9a5774a8cdbab6cebd`  
		Last Modified: Tue, 23 May 2023 01:40:43 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d899cb2fcb33df12ec1c25c5446236eae8b1c6ddc5e1783175e8771b34c2411d`  
		Last Modified: Tue, 23 May 2023 01:40:43 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf12030bd82715d32aa6be01abf001f8a29911bde2263ce46446a12753ac01fd`  
		Last Modified: Tue, 23 May 2023 01:40:43 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7181d0d6418d209d13829195afacf5a1b9e485b7bedd400420ff2dd407885e37`  
		Last Modified: Tue, 23 May 2023 06:18:01 GMT  
		Size: 15.0 MB (14961407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acee86c35375543ef4f65c5c08b154950cb260f7207cd7f363b173ba77ea3143`  
		Last Modified: Tue, 23 May 2023 06:18:00 GMT  
		Size: 1.3 MB (1258282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55930c5b754b0789667572aa53ec90c0f03213fd6e5c2f7c516eb55274e036f8`  
		Last Modified: Tue, 23 May 2023 06:18:02 GMT  
		Size: 15.4 MB (15414946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862f0dcc9ded131184312f75798c925896d4b0393ab66ac4850235c3e5c4098e`  
		Last Modified: Tue, 23 May 2023 06:17:59 GMT  
		Size: 642.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa836b8430105c5056e8ce23b4958e2c8339e7112a7a4cf8d6e0dcf1b9ad96d`  
		Last Modified: Tue, 23 May 2023 06:17:59 GMT  
		Size: 537.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860b579a09233c3c474a1686bae710908de9b6a32dbc2abc21c16a5e0025f443`  
		Last Modified: Tue, 23 May 2023 06:18:27 GMT  
		Size: 16.6 MB (16554332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c099043a036aa65dadf00561196475a46a5859f58393ac57ee2511e02eedcea`  
		Last Modified: Tue, 23 May 2023 06:18:26 GMT  
		Size: 3.8 KB (3773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155ce6ec35b56c232f62caf9ad1774475824bb4ec7626ef53f17d092f8a5cad1`  
		Last Modified: Tue, 23 May 2023 06:18:26 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
