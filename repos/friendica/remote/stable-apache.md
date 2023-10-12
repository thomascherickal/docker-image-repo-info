## `friendica:stable-apache`

```console
$ docker pull friendica@sha256:7c6ec6ed89ab96df6c5a43316c6a4d11feda8059e9bbd51a93ad8187de06fe34
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

### `friendica:stable-apache` - linux; amd64

```console
$ docker pull friendica@sha256:39c53f0e680cf108df3631ed4c4a4924fc77473a1ef24cdcbf9cc0ba17ae5e4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.0 MB (253976193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f4458755c82bb6127925e5ec3922bd3cfe5b0819a00aa4f62dca9e1678bba5b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 04:56:03 GMT
ADD file:7eb149bcaba1d7dcab06b3f9a0615ca459e9cb28459a0864f92b0037f270ba66 in / 
# Wed, 20 Sep 2023 04:56:03 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 17:32:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 17:32:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 17:33:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 17:33:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 17:33:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 17:36:23 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 17:36:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 17:36:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 17:36:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 17:36:33 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 17:36:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 17:36:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 17:36:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 19:43:51 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 19:43:51 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 19:43:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 19:43:51 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 19:44:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 19:44:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 19:46:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 19:46:58 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 19:46:58 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 19:46:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 19:46:59 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 19:46:59 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 19:46:59 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 19:46:59 GMT
EXPOSE 80
# Wed, 20 Sep 2023 19:46:59 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 06:52:52 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 21 Sep 2023 06:52:52 GMT
ENV GOSU_VERSION=1.14
# Thu, 21 Sep 2023 06:53:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Oct 2023 02:16:20 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-6.0.1;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Oct 2023 02:16:20 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 06 Oct 2023 02:16:20 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 06 Oct 2023 02:16:21 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 06 Oct 2023 02:16:21 GMT
VOLUME [/var/www/html]
# Fri, 06 Oct 2023 02:16:21 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 06 Oct 2023 02:16:22 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 06 Oct 2023 02:16:22 GMT
ENV FRIENDICA_VERSION=2023.05
# Fri, 06 Oct 2023 02:16:22 GMT
ENV FRIENDICA_ADDONS=2023.05
# Fri, 06 Oct 2023 02:16:22 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=333e63c0aaea24a072c21393de3a1ac5b66e6cb25158db668417b842bedcdee7
# Fri, 06 Oct 2023 02:16:22 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=6b6f486532a995f67bf6bc0d459ee371a2bfd2ba9b95c84dac49193cdfe76ea8
# Fri, 06 Oct 2023 02:16:45 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Oct 2023 02:16:46 GMT
COPY multi:ecba68c67f63e55d0b2b18cd57f1ecbe17d7d27bf9cb241b343fd490f8745145 in / 
# Fri, 06 Oct 2023 02:16:46 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 06 Oct 2023 02:16:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 06 Oct 2023 02:16:46 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:7dbc1adf280e1aa588c033eaa746aa6db327ee16be705740f81741f5e6945c86`  
		Last Modified: Wed, 20 Sep 2023 05:01:05 GMT  
		Size: 31.4 MB (31417711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b9708f27825ba238246d858727fd21c567ca18fb96a94796a6f6178db0de04`  
		Last Modified: Wed, 20 Sep 2023 20:11:14 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231b648539d7ae8139fbedfd8825a254b9d58408a98c355916a5c25bb4212d7`  
		Last Modified: Wed, 20 Sep 2023 20:11:27 GMT  
		Size: 91.6 MB (91632209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a8193022d3d0b2af1e75d1fd37d6f90660dad2536d49d8096003b8e0cbe1a0`  
		Last Modified: Wed, 20 Sep 2023 20:11:14 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d026a84e3b88ea61c40e22ed7e2cad6699d70af8b80ff3c03427c297d0ed29a`  
		Last Modified: Wed, 20 Sep 2023 20:11:45 GMT  
		Size: 19.2 MB (19248150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:954034b3a164067e9b2e95633301cc81f4691880785f87945bca30466da307ee`  
		Last Modified: Wed, 20 Sep 2023 20:11:42 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603ee144b85aa935d6429eedef40c5d6dc997fc874f06c348734d7a684c1208`  
		Last Modified: Wed, 20 Sep 2023 20:11:42 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd17aafc5e8929a57a231b17ae94f81a1c168bc74e8f43ccf85e84792f8ad19`  
		Last Modified: Wed, 20 Sep 2023 20:24:05 GMT  
		Size: 11.2 MB (11162318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9029a81a2e8d35f15080e349d35465aa07166947ac51d31c878cc634c8024545`  
		Last Modified: Wed, 20 Sep 2023 20:24:02 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81068f7f5100945864a6a72ba10d7086e86fac647f13ead3d3b10cb3fb96a8c3`  
		Last Modified: Wed, 20 Sep 2023 20:24:04 GMT  
		Size: 10.8 MB (10779802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbd0e046031754ccc5bdf9577eb43bddc291f889ab4a60e4545c126f9fd78e8`  
		Last Modified: Wed, 20 Sep 2023 20:24:02 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b25a72d1106efb367679e89114eeef5a138c7ab984a6be15288c56556b731e`  
		Last Modified: Wed, 20 Sep 2023 20:24:02 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fddc2d64f77fad2a858e0085aff38474ac648c9c11db49385a468cb74d8da166`  
		Last Modified: Wed, 20 Sep 2023 20:24:02 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc19310eafd9b915784560f75f68b9418b57a3b3fdb8857e72884af0a42ff51`  
		Last Modified: Thu, 21 Sep 2023 07:00:15 GMT  
		Size: 15.6 MB (15583170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e266e95cddf50bb07470d6da92be5336b86c22b2e42ec537106a2ef8047385d6`  
		Last Modified: Thu, 21 Sep 2023 07:00:14 GMT  
		Size: 1.3 MB (1296641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81f80c27438b578aa8ccd1b0ceac7663b1670a21a5a8e67abe9d22859a87c6d`  
		Last Modified: Fri, 06 Oct 2023 02:23:48 GMT  
		Size: 18.2 MB (18156280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b82986b4100b485b08ec95a01241b4455c627d87dab1ea111464b48c6101d2`  
		Last Modified: Fri, 06 Oct 2023 02:23:43 GMT  
		Size: 645.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8eecf9781731f5a7650b03a00abed3c6b476257b79f508cd06a86f2f85cc4b`  
		Last Modified: Fri, 06 Oct 2023 02:23:43 GMT  
		Size: 538.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88accab5a624dad86010a0723b05f8e3791e80c03d20988f0d007cf9faf7064`  
		Last Modified: Fri, 06 Oct 2023 02:23:49 GMT  
		Size: 54.7 MB (54689091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be177813289e71a0ce3376f457f93f0b94cd4c64bffb1a25a803a344fa3fd87c`  
		Last Modified: Fri, 06 Oct 2023 02:23:43 GMT  
		Size: 3.1 KB (3137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ba177cb671f5c1d56219e2c60133c4bf521159175cc207cde2e866595fc185`  
		Last Modified: Fri, 06 Oct 2023 02:23:43 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-apache` - linux; arm variant v5

```console
$ docker pull friendica@sha256:fabeeeb6f8dabad91156dfa721ba44112cdcb4dc3b99963506953d330bef93af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.5 MB (229474073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de779bf8fa55aeb51c1e0ccb8e683ecef67c2371091afc67c6233cc21cba5556`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:59 GMT
ADD file:01d6efe5a08019fcf00cfd0af4d6d61c6d4e43fd98cbb0054e82e8a78275573f in / 
# Wed, 11 Oct 2023 17:37:59 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 22:41:33 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Oct 2023 22:41:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Oct 2023 22:41:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 22:42:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Oct 2023 22:42:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 11 Oct 2023 22:44:40 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 Oct 2023 22:44:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 Oct 2023 22:44:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 Oct 2023 22:44:52 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 Oct 2023 22:44:53 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 Oct 2023 22:44:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:44:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 22:44:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Oct 2023 23:57:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 11 Oct 2023 23:57:24 GMT
ENV PHP_VERSION=8.0.30
# Wed, 11 Oct 2023 23:57:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 11 Oct 2023 23:57:24 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 11 Oct 2023 23:57:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Oct 2023 23:57:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:02:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 12 Oct 2023 00:02:45 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:02:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 12 Oct 2023 00:02:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 12 Oct 2023 00:02:47 GMT
STOPSIGNAL SIGWINCH
# Thu, 12 Oct 2023 00:02:47 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 12 Oct 2023 00:02:47 GMT
WORKDIR /var/www/html
# Thu, 12 Oct 2023 00:02:47 GMT
EXPOSE 80
# Thu, 12 Oct 2023 00:02:48 GMT
CMD ["apache2-foreground"]
# Thu, 12 Oct 2023 10:47:29 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 12 Oct 2023 10:47:29 GMT
ENV GOSU_VERSION=1.14
# Thu, 12 Oct 2023 10:47:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 12 Oct 2023 10:50:09 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-6.0.1;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:50:09 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 12 Oct 2023 10:50:09 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 12 Oct 2023 10:50:10 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 12 Oct 2023 10:50:10 GMT
VOLUME [/var/www/html]
# Thu, 12 Oct 2023 10:50:10 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 12 Oct 2023 10:50:10 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Thu, 12 Oct 2023 10:50:11 GMT
ENV FRIENDICA_VERSION=2023.05
# Thu, 12 Oct 2023 10:50:11 GMT
ENV FRIENDICA_ADDONS=2023.05
# Thu, 12 Oct 2023 10:50:11 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=333e63c0aaea24a072c21393de3a1ac5b66e6cb25158db668417b842bedcdee7
# Thu, 12 Oct 2023 10:50:11 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=6b6f486532a995f67bf6bc0d459ee371a2bfd2ba9b95c84dac49193cdfe76ea8
# Thu, 12 Oct 2023 10:50:38 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 10:50:39 GMT
COPY multi:ecba68c67f63e55d0b2b18cd57f1ecbe17d7d27bf9cb241b343fd490f8745145 in / 
# Thu, 12 Oct 2023 10:50:39 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Thu, 12 Oct 2023 10:50:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 10:50:40 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5419c984dacdb9784c03bde904accd013b4e056c627102949c262726f4cae135`  
		Last Modified: Wed, 11 Oct 2023 17:41:31 GMT  
		Size: 28.9 MB (28921245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e93d766f8d2582d9775399569ea38818302f806f5912c837431500790ced0d38`  
		Last Modified: Thu, 12 Oct 2023 00:16:53 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196a02faf69b274cf220b14c571c546ff9b8ed622d62420acd8b9078082875bc`  
		Last Modified: Thu, 12 Oct 2023 00:17:13 GMT  
		Size: 73.7 MB (73691001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b110edef76ac2d702c9f1a1d2519bccc67c69a961e3c46c864842c82c964f328`  
		Last Modified: Thu, 12 Oct 2023 00:16:53 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d002adf85550197cd394378881b9a819fc7a488399a9c920a9febc8aa4df450`  
		Last Modified: Thu, 12 Oct 2023 00:17:36 GMT  
		Size: 18.6 MB (18558775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283f688aed7faf2342e38739c5336cd29946f830dd76f5f8dcfd776088158aa7`  
		Last Modified: Thu, 12 Oct 2023 00:17:30 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcd849974f54cd80355342ee34fb7c78fd8889b8e932f3415621670878e8458`  
		Last Modified: Thu, 12 Oct 2023 00:17:30 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8cbf54db2aaf2b620affeab515550ff8bf01ec0e39155a9b0f66f6a6ff310b`  
		Last Modified: Thu, 12 Oct 2023 00:24:41 GMT  
		Size: 11.2 MB (11161570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668a4125dac45b48c65940464eb79e120f1935a432bc9d159e2148a41f3e87e9`  
		Last Modified: Thu, 12 Oct 2023 00:24:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa00096d0c74a6ab234fc0d1c668236608c18364c131bdb55da59e5881bb388b`  
		Last Modified: Thu, 12 Oct 2023 00:24:41 GMT  
		Size: 9.8 MB (9800668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b88b0c1552ab87e1195b9ecd566445b14094cf8c4da66b1eedfe60ef22c5fb3`  
		Last Modified: Thu, 12 Oct 2023 00:24:39 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1845bd10797353276f2475a57413d71087dc4625af3a4da9facbc85e7f7cc36`  
		Last Modified: Thu, 12 Oct 2023 00:24:38 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e447021f0b0986beba8cbc442e0dbcd28f9b420aee29e1df0e68563b263c2e7b`  
		Last Modified: Thu, 12 Oct 2023 00:24:38 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6e9312c96b5d855ff6a508051caae239dab686d732a2f62d6219bf3ebf3b98`  
		Last Modified: Thu, 12 Oct 2023 10:55:07 GMT  
		Size: 15.5 MB (15480523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cd5a1365d95e33947a3f7e8b57e53c52f81a813f0cfe6450ff95a509b32f09`  
		Last Modified: Thu, 12 Oct 2023 10:55:04 GMT  
		Size: 1.3 MB (1259946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e84ccdfb5d65fffdfecb64f70b7d20149e955935f27428d2e9ca0e85901d3c`  
		Last Modified: Thu, 12 Oct 2023 10:55:07 GMT  
		Size: 15.9 MB (15901963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb49235bcc77506eb1ecb1ed09320d700b8adbe9c995448c342e5426fb26b063`  
		Last Modified: Thu, 12 Oct 2023 10:55:02 GMT  
		Size: 645.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a594485798a78b5aa3e8ec742c93d252cc86df048fcffc114707252b1225b66a`  
		Last Modified: Thu, 12 Oct 2023 10:55:02 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ae792f35c2d29511724b257b429a31a54a80dbe946e823b8ea7be429975b6f`  
		Last Modified: Thu, 12 Oct 2023 10:55:11 GMT  
		Size: 54.7 MB (54687553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158dd1eecc300e14c54739431d00f2e036fa7435f99f30dea7058719085eddf4`  
		Last Modified: Thu, 12 Oct 2023 10:55:02 GMT  
		Size: 3.1 KB (3136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3558bc83b3fb56f7117f783a273f3bd819a90a489a7ca232d5a415702e40ee`  
		Last Modified: Thu, 12 Oct 2023 10:55:02 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-apache` - linux; arm variant v7

```console
$ docker pull friendica@sha256:d58d7e2fe2c20f9bbbcb681b59cb56b8c8ded7abe7c1ac82fe71038b2395e887
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.7 MB (220676537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea5ef534d1202a51e5ba487aea8d289ed2fcfc5e91c5a616f30a55cc2a373a90`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:29 GMT
ADD file:0d1753bfedd7193184780166819d0407867a22d82804c0045274f1f13afecac0 in / 
# Wed, 11 Oct 2023 17:42:29 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:28:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Oct 2023 19:28:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Oct 2023 19:29:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:29:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Oct 2023 19:29:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 11 Oct 2023 19:32:06 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 Oct 2023 19:32:06 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 Oct 2023 19:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 Oct 2023 19:32:16 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 Oct 2023 19:32:17 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 Oct 2023 19:32:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 19:32:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Oct 2023 19:32:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Oct 2023 21:04:34 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 11 Oct 2023 21:04:34 GMT
ENV PHP_VERSION=8.0.30
# Wed, 11 Oct 2023 21:04:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 11 Oct 2023 21:04:34 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 11 Oct 2023 21:04:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 Oct 2023 21:04:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:07:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 Oct 2023 21:07:02 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:07:03 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 Oct 2023 21:07:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 Oct 2023 21:07:03 GMT
STOPSIGNAL SIGWINCH
# Wed, 11 Oct 2023 21:07:03 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 11 Oct 2023 21:07:03 GMT
WORKDIR /var/www/html
# Wed, 11 Oct 2023 21:07:03 GMT
EXPOSE 80
# Wed, 11 Oct 2023 21:07:04 GMT
CMD ["apache2-foreground"]
# Thu, 12 Oct 2023 04:31:28 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 12 Oct 2023 04:31:28 GMT
ENV GOSU_VERSION=1.14
# Thu, 12 Oct 2023 04:31:42 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 12 Oct 2023 04:34:31 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-6.0.1;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 04:34:31 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 12 Oct 2023 04:34:31 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 12 Oct 2023 04:34:31 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 12 Oct 2023 04:34:32 GMT
VOLUME [/var/www/html]
# Thu, 12 Oct 2023 04:34:32 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 12 Oct 2023 04:34:32 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Thu, 12 Oct 2023 04:34:32 GMT
ENV FRIENDICA_VERSION=2023.05
# Thu, 12 Oct 2023 04:34:32 GMT
ENV FRIENDICA_ADDONS=2023.05
# Thu, 12 Oct 2023 04:34:32 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=333e63c0aaea24a072c21393de3a1ac5b66e6cb25158db668417b842bedcdee7
# Thu, 12 Oct 2023 04:34:33 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=6b6f486532a995f67bf6bc0d459ee371a2bfd2ba9b95c84dac49193cdfe76ea8
# Thu, 12 Oct 2023 04:34:58 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 04:34:59 GMT
COPY multi:ecba68c67f63e55d0b2b18cd57f1ecbe17d7d27bf9cb241b343fd490f8745145 in / 
# Thu, 12 Oct 2023 04:34:59 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Thu, 12 Oct 2023 04:34:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 12 Oct 2023 04:35:00 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bb9c59b28e9fb9c31ffdb002ca9a6656677eee093c8093fcbea8818e927df70a`  
		Last Modified: Wed, 11 Oct 2023 17:47:06 GMT  
		Size: 26.6 MB (26579008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a870f1e3a42421045ea94a74346c756dc23980a6eebee738ab3246fa81d3b417`  
		Last Modified: Wed, 11 Oct 2023 21:26:32 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6262879acde0f15e138f54ee86a74d1877308791d1c970711e23d8269ef4a3`  
		Last Modified: Wed, 11 Oct 2023 21:26:48 GMT  
		Size: 69.3 MB (69322692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51b63c57139f0e92fd27c08d2803b24490e3fc7edd48349bd9b4cbeffea6b5f`  
		Last Modified: Wed, 11 Oct 2023 21:26:31 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7a8a287b95f8fde32eb0edf4447a2c7e997b649bbe396a898ea35f3df3651b`  
		Last Modified: Wed, 11 Oct 2023 21:27:07 GMT  
		Size: 18.0 MB (18017808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85214cabeb78774b100bf35b74b2a9401015b5033d9e256f13c0ef8c357487bb`  
		Last Modified: Wed, 11 Oct 2023 21:27:03 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dddef0e73a4bd87189b3d87f55c1e6a63324ce10c87009d8c629e9789a541e`  
		Last Modified: Wed, 11 Oct 2023 21:27:03 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b36b9b1f02a2b3cca261136809fb061588d290415ebf378738db6877bc56f8b`  
		Last Modified: Wed, 11 Oct 2023 21:35:27 GMT  
		Size: 11.2 MB (11161534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4230c7e87280cdaa7fdc2c4f6546cc6205cf5763e469ca9e8a81a838853fb4f7`  
		Last Modified: Wed, 11 Oct 2023 21:35:24 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d1e931819ffe6c31597e74a641d48e5c8b72a509a1b58d6ded406a74b18c8a`  
		Last Modified: Wed, 11 Oct 2023 21:35:26 GMT  
		Size: 9.3 MB (9311695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38002eaae5c150bbedb732471cb4bb85c47d81442f9b700e0443bfa58a5f5c76`  
		Last Modified: Wed, 11 Oct 2023 21:35:24 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f861d39ff4806a24070ffe6c98340bfb9710f77a20efec6d5e393ef7209c4b48`  
		Last Modified: Wed, 11 Oct 2023 21:35:24 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8120adb948ffaed92eba055223486c25388dfa6b279d91484f050c1385c0f168`  
		Last Modified: Wed, 11 Oct 2023 21:35:24 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e7f6838a0ad682e99075101b5382978283fec5ade6bce818965229d423221c`  
		Last Modified: Thu, 12 Oct 2023 04:39:56 GMT  
		Size: 15.6 MB (15553704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fe4215a71215c754014d74e94b09d3ddccd3c07932736ac3b92a242413c407`  
		Last Modified: Thu, 12 Oct 2023 04:39:54 GMT  
		Size: 1.3 MB (1253073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7a8df1dd015aaffe1b4c8772efb42b7deae4805cfa41a01900e545b3856590`  
		Last Modified: Thu, 12 Oct 2023 04:39:57 GMT  
		Size: 14.8 MB (14778814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e4ef5d20d9c04033606f69f95bc42f8961805a9e46158f3007a847d7d15642`  
		Last Modified: Thu, 12 Oct 2023 04:39:51 GMT  
		Size: 640.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9953ae1de27d80eea92b6d4b4b9f7a40be28b9874ee9944cd5704c4fda3ffc0f`  
		Last Modified: Thu, 12 Oct 2023 04:39:51 GMT  
		Size: 540.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a6d8ca79c73293f0dabab29af62c9bd1562e74b3c2c821f4a793660771cc5d`  
		Last Modified: Thu, 12 Oct 2023 04:40:02 GMT  
		Size: 54.7 MB (54687385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809e3b8f3703e0fad462aeabdda7886f58639ecbbc4a4246107001a02352d3f5`  
		Last Modified: Thu, 12 Oct 2023 04:39:52 GMT  
		Size: 3.1 KB (3137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27668ad7b728b19d980390c6454bc96f03febee9c7ddfaf321a2c707907407b`  
		Last Modified: Thu, 12 Oct 2023 04:39:51 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-apache` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:aa45118377040c620289002b66004032519033c3fd3eaee132100397eb42d791
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.6 MB (244595522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:086049e36b8ce12b344dc91a4da5f3203668b949c7fac0edb8f1fe3a8d14de50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:28 GMT
ADD file:024479be439b4ecb37c939e68673adc72955f3345ca0e809bd13e897709e59e4 in / 
# Wed, 20 Sep 2023 02:44:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:08:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 03:08:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 03:08:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 03:08:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 03:08:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 03:11:48 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 03:11:48 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 03:11:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 03:11:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 03:11:57 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 03:11:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:11:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:11:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 05:41:17 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 05:41:17 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 05:41:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 05:41:17 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 05:41:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 05:41:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:43:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 05:43:21 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:43:21 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 05:43:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 05:43:21 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 05:43:21 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:43:22 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 05:43:22 GMT
EXPOSE 80
# Wed, 20 Sep 2023 05:43:22 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 19:04:29 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Wed, 20 Sep 2023 19:04:29 GMT
ENV GOSU_VERSION=1.14
# Wed, 20 Sep 2023 19:04:38 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Oct 2023 01:13:26 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-6.0.1;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Oct 2023 01:13:26 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 06 Oct 2023 01:13:27 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 06 Oct 2023 01:13:27 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 06 Oct 2023 01:13:27 GMT
VOLUME [/var/www/html]
# Fri, 06 Oct 2023 01:13:28 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 06 Oct 2023 01:13:28 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 06 Oct 2023 01:13:28 GMT
ENV FRIENDICA_VERSION=2023.05
# Fri, 06 Oct 2023 01:13:28 GMT
ENV FRIENDICA_ADDONS=2023.05
# Fri, 06 Oct 2023 01:13:28 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=333e63c0aaea24a072c21393de3a1ac5b66e6cb25158db668417b842bedcdee7
# Fri, 06 Oct 2023 01:13:28 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=6b6f486532a995f67bf6bc0d459ee371a2bfd2ba9b95c84dac49193cdfe76ea8
# Fri, 06 Oct 2023 01:13:50 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Oct 2023 01:13:51 GMT
COPY multi:ecba68c67f63e55d0b2b18cd57f1ecbe17d7d27bf9cb241b343fd490f8745145 in / 
# Fri, 06 Oct 2023 01:13:51 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 06 Oct 2023 01:13:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 06 Oct 2023 01:13:51 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:fc521c5b98350f6fd8c72ace1e48558bb7b53cb3db201a2a3b42095401cd02f1`  
		Last Modified: Wed, 20 Sep 2023 02:48:13 GMT  
		Size: 30.1 MB (30062869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011d119a94c0f59e8eabde01f2b7a4da9d92360102426dcaad9d1d0be4b4092c`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c2e7320620034b78e6c4122bdaf225b766ba582397845df17e1ca60098d29c`  
		Last Modified: Wed, 20 Sep 2023 06:01:20 GMT  
		Size: 86.9 MB (86929113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff55be7dadd795271386506373641b927cc6f05b8efda3e6ff839f8419b6b1`  
		Last Modified: Wed, 20 Sep 2023 06:01:09 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db4302c1b3aba16628a8226cbf7e2005246794ffae23f531d4b1f22a5f1ca78`  
		Last Modified: Wed, 20 Sep 2023 06:01:37 GMT  
		Size: 19.2 MB (19170297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e803e16a6eafe2f883ecb377a60f60c91aaf73ce231424cf1a48e5e1434e9b19`  
		Last Modified: Wed, 20 Sep 2023 06:01:34 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd1d1c8a7b06ce97002de91f78a98a9436fe9afd488362c77d57314628bea87`  
		Last Modified: Wed, 20 Sep 2023 06:01:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3acd7f626948ddc7750c59e9098839c63f9e1459db4250e6cff74abd28abbc`  
		Last Modified: Wed, 20 Sep 2023 06:15:48 GMT  
		Size: 11.2 MB (11161577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107920f9866c5422ee08481254c83a7d975d367cb86a1df05a834079cd65a3a8`  
		Last Modified: Wed, 20 Sep 2023 06:15:45 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0996a83f7a62c924d9c4d81e0a7ee67d93f901eef18f6fd9b3794ade5d688e61`  
		Last Modified: Wed, 20 Sep 2023 06:15:47 GMT  
		Size: 10.2 MB (10236572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2502ee4ecfe2b4c38a7ea146db1e73e9dfdc1035ba69a62ae8374e338b6522`  
		Last Modified: Wed, 20 Sep 2023 06:15:45 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b42be930116eb2f7b8f750e601a4053809b2259e9ed4a8f62c6e425db8eab5b`  
		Last Modified: Wed, 20 Sep 2023 06:15:45 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b188b30b85e72274daacd1efd120a6ee92ac05c8c6eeea83a1cb30afd21135f5`  
		Last Modified: Wed, 20 Sep 2023 06:15:45 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beab7d3d5b3a6736d0ee8b09676c926ffddb5257eaee36437b5ead199bcc0720`  
		Last Modified: Wed, 20 Sep 2023 19:10:31 GMT  
		Size: 15.3 MB (15345906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b6f3b67ce389682b587e34e00958952e1e843a6660ff4b023b0d7d000a3b70`  
		Last Modified: Wed, 20 Sep 2023 19:10:30 GMT  
		Size: 1.2 MB (1223580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a509b773634a0be023b732895904c9b6cf8200fe14bf0ead4925134899c51184`  
		Last Modified: Fri, 06 Oct 2023 01:19:26 GMT  
		Size: 15.8 MB (15766702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8db9a165d738c679d49ead3c37c0a3f05ea32dd3bd900ee34ff66f05705e66`  
		Last Modified: Fri, 06 Oct 2023 01:19:22 GMT  
		Size: 641.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5a56dd6bf1fd3ed26ff127031a17141527089d4b3e927bf4bc100ef51f8746`  
		Last Modified: Fri, 06 Oct 2023 01:19:22 GMT  
		Size: 539.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fadae5a86d57296c007df43bbf4f86b9fadcd430381313010069cd06be1548`  
		Last Modified: Fri, 06 Oct 2023 01:19:27 GMT  
		Size: 54.7 MB (54688106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b4ae8205490dd25ded033c1c0391368c3afb9b69ebd300d5b700472771aa46`  
		Last Modified: Fri, 06 Oct 2023 01:19:22 GMT  
		Size: 3.1 KB (3136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf88122fbeb3de61a58f3076c29191e4e5920fc0b16ad48aa202550f7ee263fa`  
		Last Modified: Fri, 06 Oct 2023 01:19:22 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-apache` - linux; 386

```console
$ docker pull friendica@sha256:45357016e61e7dc3b0349a04e2a45d039c00361dbe4dd19a9540294055687013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **256.4 MB (256426180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c01862db67cefeb9254bf7c2c8ed52c03047af5c2f15b4654f26c3c309358b04`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 00:42:18 GMT
ADD file:51db29acb4893b446fcf8a93f7fa809201b49d6ea62a009ab14002cafd3ac4a8 in / 
# Wed, 20 Sep 2023 00:42:18 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 01:21:34 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 01:21:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 01:22:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 01:22:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 01:22:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 01:27:56 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 01:27:56 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 01:28:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 01:28:11 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 01:28:12 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 01:28:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 01:28:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 01:28:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 06:14:40 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 06:14:41 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 06:14:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 06:14:41 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 06:14:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 06:14:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:20:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 06:20:00 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:20:01 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 06:20:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 06:20:01 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 06:20:02 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 06:20:02 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 06:20:02 GMT
EXPOSE 80
# Wed, 20 Sep 2023 06:20:02 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 05:34:41 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 21 Sep 2023 05:34:42 GMT
ENV GOSU_VERSION=1.14
# Thu, 21 Sep 2023 05:34:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Oct 2023 01:49:39 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-6.0.1;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Oct 2023 01:49:39 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 06 Oct 2023 01:49:39 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 06 Oct 2023 01:49:40 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 06 Oct 2023 01:49:40 GMT
VOLUME [/var/www/html]
# Fri, 06 Oct 2023 01:49:41 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 06 Oct 2023 01:49:41 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 06 Oct 2023 01:49:41 GMT
ENV FRIENDICA_VERSION=2023.05
# Fri, 06 Oct 2023 01:49:41 GMT
ENV FRIENDICA_ADDONS=2023.05
# Fri, 06 Oct 2023 01:49:41 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=333e63c0aaea24a072c21393de3a1ac5b66e6cb25158db668417b842bedcdee7
# Fri, 06 Oct 2023 01:49:41 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=6b6f486532a995f67bf6bc0d459ee371a2bfd2ba9b95c84dac49193cdfe76ea8
# Fri, 06 Oct 2023 01:50:09 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Oct 2023 01:50:10 GMT
COPY multi:ecba68c67f63e55d0b2b18cd57f1ecbe17d7d27bf9cb241b343fd490f8745145 in / 
# Fri, 06 Oct 2023 01:50:10 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 06 Oct 2023 01:50:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 06 Oct 2023 01:50:10 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:091eb56f13f4be91ea9416e1b67e2c1f228b5e023f447dda2d3f5c56e57ff871`  
		Last Modified: Wed, 20 Sep 2023 00:47:36 GMT  
		Size: 32.4 MB (32397092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072459cfd581346ed5003a3895e56398debbd9b5bc065ce76657ae644b6673b0`  
		Last Modified: Wed, 20 Sep 2023 06:57:22 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02823bdeb40504f3286193851dadde3a5ecebd3f69e46b0e54b2caa3d7de8d8d`  
		Last Modified: Wed, 20 Sep 2023 06:57:45 GMT  
		Size: 92.7 MB (92723518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0441d7f8c9c59d27aae552adce64da332f052ebdd3933b61654f0c1e59819133`  
		Last Modified: Wed, 20 Sep 2023 06:57:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fe1792330d2ef3c5ad46a354ef851bd3abd4ed3af02564b4fa0350804b7657`  
		Last Modified: Wed, 20 Sep 2023 06:58:10 GMT  
		Size: 19.7 MB (19737227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227c60e6580fdaab7d2dd0485719dd5398023313891d228a1e2120b28689a746`  
		Last Modified: Wed, 20 Sep 2023 06:58:02 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7dfa4f58f93f200dc90e8cc29f3062bc8c064832da286723fe9f9bc2500adc`  
		Last Modified: Wed, 20 Sep 2023 06:58:02 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7d77186d847b8e6cf2aeff12350fb919a5952286c77828b2be73ce56323198`  
		Last Modified: Wed, 20 Sep 2023 07:14:45 GMT  
		Size: 11.2 MB (11161583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a14a13b6a7d3a32c8dd24be91c4d22539067faddede9636cf2341b8e067668cd`  
		Last Modified: Wed, 20 Sep 2023 07:14:41 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a600e6110bdaff864917a3f7c87e1112ebfc8ee1607651e0893cd2502894bd`  
		Last Modified: Wed, 20 Sep 2023 07:14:45 GMT  
		Size: 11.0 MB (10986064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597c7970f9cf86ba8d7588e0c633a1931037f8b1031e18218e515606c1f9dd81`  
		Last Modified: Wed, 20 Sep 2023 07:14:41 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627e40f3a8c819e6dc1fb29914efcaef55b12e5c2af2cb13b1f051321a36069a`  
		Last Modified: Wed, 20 Sep 2023 07:14:42 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1648c62825293ee76d4e509439cf257b411504036426153914036330fe201038`  
		Last Modified: Wed, 20 Sep 2023 07:14:41 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3fc265b21f68b79c2cb307b7fbdd79229e57ffad7d7fddf695ffa385e2785f`  
		Last Modified: Thu, 21 Sep 2023 05:43:32 GMT  
		Size: 16.1 MB (16050065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97db9b63dd252c391552d5d60ec426b84132b0acef0baab2a9555edb0165b69`  
		Last Modified: Thu, 21 Sep 2023 05:43:30 GMT  
		Size: 1.3 MB (1262441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb53716e17c8af74f7a49b155c95bae2f2da39229d53572d492d08d15de5dfdc`  
		Last Modified: Fri, 06 Oct 2023 02:00:04 GMT  
		Size: 17.4 MB (17409115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9800384c2568e0beaa30c5cd80614284bbd6f37f4a3269c8bef36e4c7068e2`  
		Last Modified: Fri, 06 Oct 2023 01:59:58 GMT  
		Size: 641.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b32aef7a9da13c65d398ac7962481f28d32836870be27a8ccec2cb4459e408`  
		Last Modified: Fri, 06 Oct 2023 01:59:58 GMT  
		Size: 534.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba93cca9cbbed75b35ec2f9a92be3e4b6384dbf6ae05ca07567560d166d0a4c`  
		Last Modified: Fri, 06 Oct 2023 02:00:08 GMT  
		Size: 54.7 MB (54688270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6553def3014a1dc5e389f34a2fde7562ac965d61180e1f05469e3370413ee0`  
		Last Modified: Fri, 06 Oct 2023 01:59:58 GMT  
		Size: 3.1 KB (3136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2deb1fbec3c9ae2e90ca638d2c1de0123db816db0962073a599258c486e08b`  
		Last Modified: Fri, 06 Oct 2023 01:59:57 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-apache` - linux; mips64le

```console
$ docker pull friendica@sha256:d6d07880f8463a5c5532b3a913389cd087e136ef0d13f4f06da83039f44f408d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227428944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc11699c325730639276c2c39761b324150e3b6d290233d21b41be37086cc2dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 03:11:15 GMT
ADD file:28a15ec61fcc8eb66f514312583089fecc600fe3b84fdbe3bf5692f05d946bff in / 
# Wed, 20 Sep 2023 03:11:20 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:15:26 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 11:15:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 11:17:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:17:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 11:17:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 11:32:16 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 11:32:19 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 11:33:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 11:33:22 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 11:33:28 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 11:33:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 11:33:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 11:33:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 20:34:43 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 20:34:47 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 20:34:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 20:34:54 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 20:35:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 20:35:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 20:49:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 20:49:10 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 20:49:16 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 20:49:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 20:49:24 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 20:49:27 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 20:49:31 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 20:49:34 GMT
EXPOSE 80
# Wed, 20 Sep 2023 20:49:38 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 21:40:02 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 21 Sep 2023 21:40:05 GMT
ENV GOSU_VERSION=1.14
# Thu, 21 Sep 2023 21:40:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Oct 2023 02:48:28 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-6.0.1;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Oct 2023 02:48:32 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 06 Oct 2023 02:48:36 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 06 Oct 2023 02:48:42 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 06 Oct 2023 02:48:46 GMT
VOLUME [/var/www/html]
# Fri, 06 Oct 2023 02:48:53 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 06 Oct 2023 02:48:57 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 06 Oct 2023 02:49:01 GMT
ENV FRIENDICA_VERSION=2023.05
# Fri, 06 Oct 2023 02:49:05 GMT
ENV FRIENDICA_ADDONS=2023.05
# Fri, 06 Oct 2023 02:49:09 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=333e63c0aaea24a072c21393de3a1ac5b66e6cb25158db668417b842bedcdee7
# Fri, 06 Oct 2023 02:49:13 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=6b6f486532a995f67bf6bc0d459ee371a2bfd2ba9b95c84dac49193cdfe76ea8
# Fri, 06 Oct 2023 02:50:35 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Oct 2023 02:50:43 GMT
COPY multi:ecba68c67f63e55d0b2b18cd57f1ecbe17d7d27bf9cb241b343fd490f8745145 in / 
# Fri, 06 Oct 2023 02:50:50 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 06 Oct 2023 02:50:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 06 Oct 2023 02:51:02 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:191c4163c9a486a5811472bd51ed6737ccd2265795539d3f557712be2f3a2742`  
		Last Modified: Wed, 20 Sep 2023 03:22:25 GMT  
		Size: 29.6 MB (29634617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc960e41a801e89295461ac99f820dbab8a34438027cac615788448d8dc39775`  
		Last Modified: Wed, 20 Sep 2023 21:21:57 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554c8598c1f78d4c03a0b310d815cd8d339d4abc974f56243ccf4ae24dacf8c7`  
		Last Modified: Wed, 20 Sep 2023 21:22:47 GMT  
		Size: 71.8 MB (71811613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46940f42fce14c2a1d7dd19803ac3218c981367186ac1299ef35087231d2f19f`  
		Last Modified: Wed, 20 Sep 2023 21:21:56 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9952fb3d22a86c6751bf1c42a221b6ebe38dea99179405aee7f8454fc91630`  
		Last Modified: Wed, 20 Sep 2023 21:23:18 GMT  
		Size: 18.9 MB (18947020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aedffb1b2a689151865842648cb7dd15f5a213452d1b4a12c3ff1e5b600a5c`  
		Last Modified: Wed, 20 Sep 2023 21:23:05 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d41c0009ad116720b87401563bc43a6dd13e4814b7e85022973c5fa8288f3bf`  
		Last Modified: Wed, 20 Sep 2023 21:23:05 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0e57a34d86c9e1cb49313d22ce504078b7278702328ca924217d26c43908c5`  
		Last Modified: Wed, 20 Sep 2023 21:42:38 GMT  
		Size: 10.9 MB (10943978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb92975902f46f60c2868b4952aaa5dc775bd76057a6b963b9ebd5dd79d7de7`  
		Last Modified: Wed, 20 Sep 2023 21:42:33 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c582ecae6b4d4c288d73fcee507976f1109c98bcec2725eb548035951168f59`  
		Last Modified: Wed, 20 Sep 2023 21:42:41 GMT  
		Size: 9.9 MB (9923339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4043379124611f09889a0de73c52cf71e8e5aff041a4312c91aafeb5006aab`  
		Last Modified: Wed, 20 Sep 2023 21:42:33 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df74870ac153231d400e3c9428bf7f3bb48e78c7ac3f5df87c4da75486546d9b`  
		Last Modified: Wed, 20 Sep 2023 21:42:33 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5238397653a4cff5c89f9850db44abe77a2c1f9033824b6fdb0d9c21c09ce4`  
		Last Modified: Wed, 20 Sep 2023 21:42:32 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6d05a4c30d976a3fd65ff31181839e0152085af0bbece8e7a25998abaa5eaa`  
		Last Modified: Thu, 21 Sep 2023 22:13:08 GMT  
		Size: 15.0 MB (15047794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc2effa021229deea39cc41eee009af6f69c51928f3b81476164a74da921ac9`  
		Last Modified: Thu, 21 Sep 2023 22:13:01 GMT  
		Size: 947.5 KB (947465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c6bd0c5db4e6b7d594dd67b3534fc7bc057a1304d6bc74ac01b00f0896113f`  
		Last Modified: Fri, 06 Oct 2023 03:10:08 GMT  
		Size: 15.7 MB (15726987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7618abafc4582404214fe6681825b4498299f8fbf83c5cb51c16b30132165ac`  
		Last Modified: Fri, 06 Oct 2023 03:09:56 GMT  
		Size: 608.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbec7a954e20c53de762bd78252078ca196614a20cbf02b51d57d866222b6a6c`  
		Last Modified: Fri, 06 Oct 2023 03:09:56 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7da730598bfe8d0801bce00fdb1e23728825413074891d30dbee52b8a0daa04`  
		Last Modified: Fri, 06 Oct 2023 03:10:26 GMT  
		Size: 54.4 MB (54435438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3508f79da233875e6ab65d8dc283fd68d12b168acb3293c20e498ac4879a4683`  
		Last Modified: Fri, 06 Oct 2023 03:09:56 GMT  
		Size: 3.1 KB (3136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbfaa0da782f0e254b8926e7fdb80bc4a684816b9f951075e78cef66d87561d`  
		Last Modified: Fri, 06 Oct 2023 03:09:56 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-apache` - linux; ppc64le

```console
$ docker pull friendica@sha256:f8ed8b2867a3588e7db3e5893e176e2118572ec6e334155800b4184f829949f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.7 MB (253729631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:892e37202d59e06f63b4ca007f80a585deca1b75367ad4de3a4da43004133fac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 07:53:28 GMT
ADD file:906774443118f59963ef3b425ff702af4588c1cf1d7c32f6f72fff8b1af50339 in / 
# Wed, 20 Sep 2023 07:53:30 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 21:23:00 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 21:23:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 21:23:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 21:23:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 21:23:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 21:28:39 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 21:28:40 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 21:29:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 21:29:07 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 21:29:09 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 21:29:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 21:29:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 21:29:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 21 Sep 2023 00:16:39 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Thu, 21 Sep 2023 00:16:39 GMT
ENV PHP_VERSION=8.0.30
# Thu, 21 Sep 2023 00:16:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Thu, 21 Sep 2023 00:16:40 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Thu, 21 Sep 2023 00:17:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Sep 2023 00:17:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 21 Sep 2023 00:21:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Sep 2023 00:21:21 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 21 Sep 2023 00:21:22 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Sep 2023 00:21:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Sep 2023 00:21:22 GMT
STOPSIGNAL SIGWINCH
# Thu, 21 Sep 2023 00:21:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 21 Sep 2023 00:21:23 GMT
WORKDIR /var/www/html
# Thu, 21 Sep 2023 00:21:23 GMT
EXPOSE 80
# Thu, 21 Sep 2023 00:21:23 GMT
CMD ["apache2-foreground"]
# Thu, 21 Sep 2023 09:14:09 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 21 Sep 2023 09:14:10 GMT
ENV GOSU_VERSION=1.14
# Thu, 21 Sep 2023 09:14:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Fri, 06 Oct 2023 02:51:43 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-6.0.1;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Oct 2023 02:51:46 GMT
ENV PHP_MEMORY_LIMIT=512M
# Fri, 06 Oct 2023 02:51:47 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Fri, 06 Oct 2023 02:51:51 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 06 Oct 2023 02:51:54 GMT
VOLUME [/var/www/html]
# Fri, 06 Oct 2023 02:51:57 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Fri, 06 Oct 2023 02:51:58 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Fri, 06 Oct 2023 02:51:59 GMT
ENV FRIENDICA_VERSION=2023.05
# Fri, 06 Oct 2023 02:51:59 GMT
ENV FRIENDICA_ADDONS=2023.05
# Fri, 06 Oct 2023 02:52:00 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=333e63c0aaea24a072c21393de3a1ac5b66e6cb25158db668417b842bedcdee7
# Fri, 06 Oct 2023 02:52:00 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=6b6f486532a995f67bf6bc0d459ee371a2bfd2ba9b95c84dac49193cdfe76ea8
# Fri, 06 Oct 2023 02:53:15 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Fri, 06 Oct 2023 02:53:20 GMT
COPY multi:ecba68c67f63e55d0b2b18cd57f1ecbe17d7d27bf9cb241b343fd490f8745145 in / 
# Fri, 06 Oct 2023 02:53:21 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Fri, 06 Oct 2023 02:53:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 06 Oct 2023 02:53:22 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e64bfb4d4b8bfd61a4dccfc651ce802e40087cdf6029b3cbf1710fa529e70fcb`  
		Last Modified: Wed, 20 Sep 2023 08:50:44 GMT  
		Size: 35.3 MB (35291079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127f8046f674eab50dc75f55e6cef7a793000dbd8b772da271cdb68306f0ca3e`  
		Last Modified: Thu, 21 Sep 2023 00:33:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc649c20d315ba9f23db7f5d652600aabaf9708e72867362741332bd158a432`  
		Last Modified: Thu, 21 Sep 2023 00:34:10 GMT  
		Size: 86.6 MB (86636811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f3fdde26ce3630f5912d8c9fc88cb49870bda0d82b8686cca2f40a42963827`  
		Last Modified: Thu, 21 Sep 2023 00:33:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbc663291d6000412079723212b5e5a2d3c42420a02d098d9585f6e668b98a5`  
		Last Modified: Thu, 21 Sep 2023 00:34:31 GMT  
		Size: 20.5 MB (20463819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f6ef81e1828442813778867428dd30fbc070f4cd52db2b477d47758ca231b1e`  
		Last Modified: Thu, 21 Sep 2023 00:34:27 GMT  
		Size: 481.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7efbe3dd0dee66401b2bf78b02c599b0cf3678eee10597a331d79e991c0285`  
		Last Modified: Thu, 21 Sep 2023 00:34:26 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bebdd7571baf01885ee80603c39aac8e86cf31b8e6fc2f11bc0a140eec5705`  
		Last Modified: Thu, 21 Sep 2023 00:48:49 GMT  
		Size: 11.2 MB (11162251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4b708d0008646eaa28300848e5aa15f1f054f54a9828ec8b48166ca58d0e71`  
		Last Modified: Thu, 21 Sep 2023 00:48:46 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba083a7821cbadce525cecb15b137cdf91b4a8dda363d0f6d84dd13b251834b`  
		Last Modified: Thu, 21 Sep 2023 00:48:50 GMT  
		Size: 11.1 MB (11144675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f1f48ea507315e567e28927a8501d37d0d61de651b358f69c31a682534b035`  
		Last Modified: Thu, 21 Sep 2023 00:48:46 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dab93a7301279a42258289e2a35c7c44f536223daead04920e5703f6cbb03eb`  
		Last Modified: Thu, 21 Sep 2023 00:48:46 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65d58b9da85d038b48b66f70f72d53c47ecf8ce627a45b0c5374e026cf0fc6a`  
		Last Modified: Thu, 21 Sep 2023 00:48:46 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f107af48c2bfd959ceb8a3352cd1dbe1ab536cff9ef42ae756a3a1bd286dc8`  
		Last Modified: Thu, 21 Sep 2023 09:34:07 GMT  
		Size: 15.5 MB (15477841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4102abb7e3a926a9b2f828aa0041722e912624a363775b591e12cb9ae741e809`  
		Last Modified: Thu, 21 Sep 2023 09:34:05 GMT  
		Size: 1.2 MB (1196262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4326924e700aceecd23a676019d8ae673323e77dc4e922a28c456f8fd14e13a5`  
		Last Modified: Fri, 06 Oct 2023 03:09:44 GMT  
		Size: 17.7 MB (17655225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ab82814d43629ef78bdf34aa5746db19c939f0418ecf8b6e0fc668f0deb8d1`  
		Last Modified: Fri, 06 Oct 2023 03:09:37 GMT  
		Size: 643.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153b4e842180d6b0f714a43d6c2c98a83e49eace74c4fde41c69145da77d3997`  
		Last Modified: Fri, 06 Oct 2023 03:09:37 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53934fd0e3f22c28ad4bdcbb4189d7cdaf795bfff2d59db80419a075e4ef9f6`  
		Last Modified: Fri, 06 Oct 2023 03:09:48 GMT  
		Size: 54.7 MB (54690828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6412d1647d529c6726d0b72d9dcbd6fdae053d4bf20f5269e49406bf079080`  
		Last Modified: Fri, 06 Oct 2023 03:09:37 GMT  
		Size: 3.1 KB (3136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b4df6c849e3d7890ab5f4ce0eb10b2ee08e31772a085525d49908adbf9fb56`  
		Last Modified: Fri, 06 Oct 2023 03:09:37 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:stable-apache` - linux; s390x

```console
$ docker pull friendica@sha256:2f77c3cc2d047a5c1efb470b1c4c4314f14322d1a601319cd5102cb8b0580c31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.1 MB (228145541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19d79efab88efcab344a95a4082e7482101addffb1806c1e81f27e746d1040ef`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 20 Sep 2023 02:54:54 GMT
ADD file:02a97e0d5f41f84ac0284849646284fa41b5e324d24f4d95bb1e2419899da811 in / 
# Wed, 20 Sep 2023 02:54:57 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 03:28:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 20 Sep 2023 03:28:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 20 Sep 2023 03:28:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 03:28:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 20 Sep 2023 03:28:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 20 Sep 2023 03:31:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 20 Sep 2023 03:31:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 20 Sep 2023 03:32:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 1777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 20 Sep 2023 03:32:03 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 20 Sep 2023 03:32:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 20 Sep 2023 03:32:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:32:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 20 Sep 2023 03:32:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 20 Sep 2023 05:48:23 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4 39B641343D8C104B2B146DC3F9C39DC0B9698544
# Wed, 20 Sep 2023 05:48:23 GMT
ENV PHP_VERSION=8.0.30
# Wed, 20 Sep 2023 05:48:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.30.tar.xz.asc
# Wed, 20 Sep 2023 05:48:23 GMT
ENV PHP_SHA256=216ab305737a5d392107112d618a755dc5df42058226f1670e9db90e77d777d9
# Wed, 20 Sep 2023 05:48:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 20 Sep 2023 05:48:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:50:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 20 Sep 2023 05:50:33 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:50:33 GMT
RUN docker-php-ext-enable sodium
# Wed, 20 Sep 2023 05:50:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 20 Sep 2023 05:50:33 GMT
STOPSIGNAL SIGWINCH
# Wed, 20 Sep 2023 05:50:33 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Wed, 20 Sep 2023 05:50:34 GMT
WORKDIR /var/www/html
# Wed, 20 Sep 2023 05:50:34 GMT
EXPOSE 80
# Wed, 20 Sep 2023 05:50:34 GMT
CMD ["apache2-foreground"]
# Wed, 20 Sep 2023 13:27:32 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Wed, 20 Sep 2023 13:27:32 GMT
ENV GOSU_VERSION=1.14
# Wed, 20 Sep 2023 13:27:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Mon, 09 Oct 2023 15:55:06 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev         libgmp-dev         libmagickcore-6.q16-6-extra     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap         gmp     ;         pecl install apcu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-6.0.1;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2023 15:55:08 GMT
ENV PHP_MEMORY_LIMIT=512M
# Mon, 09 Oct 2023 15:55:08 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Mon, 09 Oct 2023 15:55:09 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Mon, 09 Oct 2023 15:55:09 GMT
VOLUME [/var/www/html]
# Mon, 09 Oct 2023 15:55:10 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Mon, 09 Oct 2023 15:55:11 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Mon, 09 Oct 2023 15:55:12 GMT
ENV FRIENDICA_VERSION=2023.05
# Mon, 09 Oct 2023 15:55:12 GMT
ENV FRIENDICA_ADDONS=2023.05
# Mon, 09 Oct 2023 15:55:12 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=333e63c0aaea24a072c21393de3a1ac5b66e6cb25158db668417b842bedcdee7
# Mon, 09 Oct 2023 15:55:12 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=6b6f486532a995f67bf6bc0d459ee371a2bfd2ba9b95c84dac49193cdfe76ea8
# Mon, 09 Oct 2023 16:01:07 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Mon, 09 Oct 2023 16:01:17 GMT
COPY multi:ecba68c67f63e55d0b2b18cd57f1ecbe17d7d27bf9cb241b343fd490f8745145 in / 
# Mon, 09 Oct 2023 16:01:17 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Mon, 09 Oct 2023 16:01:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 09 Oct 2023 16:01:18 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:d2d51167e651784cce0bd658d0c2caa328adef8ccf264d8c09860a95bc2a2fc6`  
		Last Modified: Wed, 20 Sep 2023 03:00:22 GMT  
		Size: 29.7 MB (29653129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a057c520bd7a3264de619d98cb953fb2d172c0b7aea904b0b97aa130e5b12a31`  
		Last Modified: Wed, 20 Sep 2023 06:00:12 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdfba7ead31b2aac27140ca57aa96b4c0c37731ebc4757a7a1266b8da684d13`  
		Last Modified: Wed, 20 Sep 2023 06:00:22 GMT  
		Size: 71.6 MB (71631627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e1fc5603884e36dafccd7be7c611ce804bc1f7a48f7cebccf662b64d887d4b`  
		Last Modified: Wed, 20 Sep 2023 06:00:12 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7a7acda4271f62e8855bb8a12789848d0eead9e96e22022e7ebf5e8b06704a`  
		Last Modified: Wed, 20 Sep 2023 06:00:35 GMT  
		Size: 19.1 MB (19077505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109a74993364fe1681f26da5aa6d00cc0b69c9be66656cc21b2f874aa5555128`  
		Last Modified: Wed, 20 Sep 2023 06:00:32 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e53251a566b8028f68bfa3dab63725647038865cff84949e92c27d0ef3159c5`  
		Last Modified: Wed, 20 Sep 2023 06:00:32 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879c1795edeb4a6e6a0144f8a22ebb84b7a9ccfd052b64f8c56bfab2778219f1`  
		Last Modified: Wed, 20 Sep 2023 06:10:06 GMT  
		Size: 11.2 MB (11161271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b0297afe1ed459769ad73e64a01535c978716adce4d0eb98b0ddc7a7c55adc`  
		Last Modified: Wed, 20 Sep 2023 06:10:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be6dcd198efde2768f049fcd5a42e4670170c2ff65ebf51541b1175db428b4e`  
		Last Modified: Wed, 20 Sep 2023 06:10:05 GMT  
		Size: 9.9 MB (9928647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060181c7469ec1a2cf99556aebffa51bc38858d1542f3225fc86f4336a09bb3d`  
		Last Modified: Wed, 20 Sep 2023 06:10:03 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a0e6a87344fb26dcb133684434969b14e6d2cbcb243ab610aedcdfe2af8f65`  
		Last Modified: Wed, 20 Sep 2023 06:10:03 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a30f4e1403966ac8604390089e0ce604ae1b2ce1b53d17a48a1d1b48f5a20b01`  
		Last Modified: Wed, 20 Sep 2023 06:10:03 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7c83873ccbf974202f653e541ee2f9d45214caf76e20e8e10d72529f8fe5fe`  
		Last Modified: Wed, 20 Sep 2023 13:33:28 GMT  
		Size: 15.0 MB (14981716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b32a5fee0b4249f9edf217bd20d57c63c82073223608133fde379bc04d93d9`  
		Last Modified: Wed, 20 Sep 2023 13:33:27 GMT  
		Size: 1.3 MB (1258261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc486b783f36343573b4eec5a1ba16a45c1bf2c12b4dd7c20214c22cddeb09e`  
		Last Modified: Mon, 09 Oct 2023 22:56:04 GMT  
		Size: 15.8 MB (15755311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1566f54db04a9bbeab232fb59237f6f2d5a654951f3228de30061b2e9d6ce8`  
		Last Modified: Mon, 09 Oct 2023 22:56:00 GMT  
		Size: 643.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8dade11ff2bd57a82341fd0a3cf1b1fff96be74ec06fd7be6ccd550b64891a3`  
		Last Modified: Mon, 09 Oct 2023 22:56:02 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd180a77b01bd1c31f3992d6661839456f6e2dec7f7be04026f09917bfc54d`  
		Last Modified: Mon, 09 Oct 2023 22:56:11 GMT  
		Size: 54.7 MB (54687253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25488c5d27f34b093003b9c5d202ea1bff03f6ed7070de1d2a57a13ffdea78e5`  
		Last Modified: Mon, 09 Oct 2023 22:56:00 GMT  
		Size: 3.1 KB (3137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494ed86dd5e9a7e968dc7eec72510b893c0665e6589affc79b65aae64694da76`  
		Last Modified: Mon, 09 Oct 2023 22:56:00 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
