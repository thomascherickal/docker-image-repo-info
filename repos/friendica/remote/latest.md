## `friendica:latest`

```console
$ docker pull friendica@sha256:98d62600553721a2f93ab4bc48d4fcc6b23ca29301b64023cb12c7893d323476
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

### `friendica:latest` - linux; amd64

```console
$ docker pull friendica@sha256:80be2af8ea13cc0d9cc9a90e465ca4ab88a8b193ed8d011cae678e54600807d4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.6 MB (251615918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01612c3f0d80af0923b99875ae9001672461b3b83c4cdab88599f43a44604b84`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:15:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:15:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:16:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:16:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:16:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:20:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:20:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:20:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:21:00 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:21:00 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:21:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:21:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:21:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 03:21:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 00:46:47 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 00:46:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 00:46:47 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 00:46:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 00:46:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:48:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 00:48:49 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:48:50 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 00:48:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 00:48:50 GMT
STOPSIGNAL SIGWINCH
# Tue, 19 Apr 2022 00:48:50 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 19 Apr 2022 00:48:50 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 00:48:50 GMT
EXPOSE 80
# Tue, 19 Apr 2022 00:48:50 GMT
CMD ["apache2-foreground"]
# Tue, 19 Apr 2022 03:20:44 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Tue, 19 Apr 2022 03:20:45 GMT
ENV GOSU_VERSION=1.14
# Tue, 19 Apr 2022 03:20:55 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 19 Apr 2022 03:22:58 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 03:22:58 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 19 Apr 2022 03:22:58 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 19 Apr 2022 03:22:59 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 19 Apr 2022 03:22:59 GMT
VOLUME [/var/www/html]
# Tue, 19 Apr 2022 03:23:00 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 19 Apr 2022 03:23:00 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Tue, 19 Apr 2022 03:27:36 GMT
ENV FRIENDICA_VERSION=2022.03
# Tue, 19 Apr 2022 03:27:36 GMT
ENV FRIENDICA_ADDONS=2022.03
# Tue, 19 Apr 2022 03:27:37 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Tue, 19 Apr 2022 03:27:37 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Tue, 19 Apr 2022 03:27:58 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 03:27:59 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Tue, 19 Apr 2022 03:27:59 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Tue, 19 Apr 2022 03:27:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Apr 2022 03:27:59 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e86af584f1e1432f2e919354a76a112af1f3146d6b2342e32a496eca57f70a`  
		Last Modified: Tue, 29 Mar 2022 04:17:31 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bd55b3ae5fafd56f7dc3bbd88b11372bda66b4043b9075a626d392863203a5`  
		Last Modified: Tue, 29 Mar 2022 04:17:44 GMT  
		Size: 91.6 MB (91602066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f3a70af964a1258ce68bbae397b3464a892ea2210425230d68ccdfa5e62ab90`  
		Last Modified: Tue, 29 Mar 2022 04:17:31 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5086159710b3ea409b4fa418d18041a81acedf8b2e62b356b16538ac746e49`  
		Last Modified: Tue, 29 Mar 2022 04:18:37 GMT  
		Size: 19.2 MB (19248565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9c764dc190cebd90a1661358ab11342866a47bfc7bf5898df1cf82751a6872`  
		Last Modified: Tue, 29 Mar 2022 04:18:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2bb7a6eead8d367aaf40f9a05e9a63913789cb1a551360a57f142680939a67`  
		Last Modified: Tue, 29 Mar 2022 04:18:34 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1c559f02555236472ee8c78f171bd50508ba846d3b337f23f287e486900b5c`  
		Last Modified: Tue, 19 Apr 2022 01:59:17 GMT  
		Size: 10.8 MB (10758648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a2d369c39af4fd08f05cd9e7b49ae3b8966d560fb8df3adb8752145cbc2b20`  
		Last Modified: Tue, 19 Apr 2022 01:59:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b299432c154c31de9efa811f302516ec76a3be914f9f51dda1798960355b0e0`  
		Last Modified: Tue, 19 Apr 2022 01:59:16 GMT  
		Size: 10.3 MB (10258564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b78c25294b3758de405dbafdc658a74496b70e77669f1f580eb68aab2658fd`  
		Last Modified: Tue, 19 Apr 2022 01:59:14 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c04b6f27ffde497109949fc0003606ec9b3783295b21aab7c83d778b496a208`  
		Last Modified: Tue, 19 Apr 2022 01:59:14 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f13750e2c9eb547b9abb705d283318349f7bb91407f2f160c56a75ac55bc82f`  
		Last Modified: Tue, 19 Apr 2022 01:59:14 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e349d561fcab0c887d46659b832d86556000d88122a6e8e95d15de2d3854d947`  
		Last Modified: Tue, 19 Apr 2022 03:29:44 GMT  
		Size: 15.4 MB (15366648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf39af52db071058bf47923c135d4327ded57defd7ec3ab7fb97ca0023df2e5`  
		Last Modified: Tue, 19 Apr 2022 03:29:43 GMT  
		Size: 1.3 MB (1296444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a02e4671fba809769280177bd69eddcfe56683910af674201f9b3cd545ee25`  
		Last Modified: Tue, 19 Apr 2022 03:29:45 GMT  
		Size: 17.6 MB (17646897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6cf47c3f15b3dc1e97572d4dc4a9ee1b12c520c814ee9a44c205af6d269894`  
		Last Modified: Tue, 19 Apr 2022 03:29:40 GMT  
		Size: 643.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9dc65cb81e3476291e0f02e4f755523faa954af55322860964e983b1abe9bb`  
		Last Modified: Tue, 19 Apr 2022 03:29:40 GMT  
		Size: 542.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13bdf9c57ddbc53e82598c13eced0bac1f0991a0f9f45d54f7cad85762da473`  
		Last Modified: Tue, 19 Apr 2022 03:30:47 GMT  
		Size: 54.0 MB (54048992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a11ed58c3dde5dc3a5e4b8c6d92114657e6b1efea86aa53fa43cffb0744cad4`  
		Last Modified: Tue, 19 Apr 2022 03:30:41 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34158762ef983f108ac167c997239131879d16221170a909b97cf8c4345381bb`  
		Last Modified: Tue, 19 Apr 2022 03:30:41 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; arm variant v5

```console
$ docker pull friendica@sha256:32bf5bdafce5943d1221583ce04bf9a43c8ad6cfffc4d0f3217420050fbcde51
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.8 MB (227816041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562df42dabae893170941ed0b392c9548fe483fa11a2fcd3c410f103b13da68a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:50:37 GMT
ADD file:6b9a30e6ef50a46e87cf9d7f5a491c7951fdb6dd6fab3c9d4a9c3c40f92b8db4 in / 
# Tue, 29 Mar 2022 00:50:38 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:16:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:16:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:17:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:17:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:17:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:23:34 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:23:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:23:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:24:01 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:24:02 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:24:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:24:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:24:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 02:53:45 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 01:23:23 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 01:23:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 01:23:24 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 01:23:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 01:23:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:27:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 01:27:55 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:27:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 01:27:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 01:27:58 GMT
STOPSIGNAL SIGWINCH
# Tue, 19 Apr 2022 01:27:58 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:27:59 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 01:27:59 GMT
EXPOSE 80
# Tue, 19 Apr 2022 01:27:59 GMT
CMD ["apache2-foreground"]
# Tue, 19 Apr 2022 02:56:35 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Tue, 19 Apr 2022 02:56:36 GMT
ENV GOSU_VERSION=1.14
# Tue, 19 Apr 2022 02:57:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 19 Apr 2022 03:03:27 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 03:03:28 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 19 Apr 2022 03:03:28 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 19 Apr 2022 03:03:29 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 19 Apr 2022 03:03:30 GMT
VOLUME [/var/www/html]
# Tue, 19 Apr 2022 03:03:32 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 19 Apr 2022 03:03:32 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Tue, 19 Apr 2022 03:14:57 GMT
ENV FRIENDICA_VERSION=2022.03
# Tue, 19 Apr 2022 03:14:57 GMT
ENV FRIENDICA_ADDONS=2022.03
# Tue, 19 Apr 2022 03:14:57 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Tue, 19 Apr 2022 03:14:58 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Tue, 19 Apr 2022 03:15:44 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 03:15:47 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Tue, 19 Apr 2022 03:15:48 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Tue, 19 Apr 2022 03:15:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Apr 2022 03:15:49 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:9a41aba0a099ec129c20f41f6370b97daa4c3d4d3edc76ea1863bc5f76f9e5e5`  
		Last Modified: Tue, 29 Mar 2022 01:05:21 GMT  
		Size: 28.9 MB (28920513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce46f4c5a9bc9955de9826fb0dff7ec089eacc125544c70af55cf4c30a8e79ba`  
		Last Modified: Tue, 29 Mar 2022 03:37:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c036fb93b9d2bc083de782babbcfb0df052105b14e970e64c6ef75782dde7230`  
		Last Modified: Tue, 29 Mar 2022 03:38:00 GMT  
		Size: 73.7 MB (73683213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57be801222463b9801716ed946fa048154ecd7575d3fdba525981c6d1bcba244`  
		Last Modified: Tue, 29 Mar 2022 03:37:09 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0dfbd691c3d3220988a7ef18e67d783c317a092640aabc8429bbe24563e1c55`  
		Last Modified: Tue, 29 Mar 2022 03:39:20 GMT  
		Size: 18.5 MB (18545967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b6b5a1e6b8a36786ac052aa20f3f03053e1b17a587b4bde699a687ce37420b`  
		Last Modified: Tue, 29 Mar 2022 03:39:09 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12aefd878aa4f2a8a0ce13c03a80714f78c1fccb1cdd16e63f13cd2de0ba97e5`  
		Last Modified: Tue, 29 Mar 2022 03:39:09 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23e6cc5c96a37c19c31088d411f830e8da16b845abc6eae6406ea511f7976b0`  
		Last Modified: Tue, 19 Apr 2022 02:20:29 GMT  
		Size: 10.8 MB (10757388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c2b19988bf56bcd44f4013192a6c2acdd70b8d64ae183eff8bedacf3c6ff9c`  
		Last Modified: Tue, 19 Apr 2022 02:20:24 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d4653a263b26fb72506a97e58bb594026d5b037f2c0d167b249e01707ccff8`  
		Last Modified: Tue, 19 Apr 2022 02:20:31 GMT  
		Size: 9.6 MB (9630099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28465c1cb5852edaa5e9e71010b46b7ee087b9c4f93aa4424122d01f4bf6fcda`  
		Last Modified: Tue, 19 Apr 2022 02:20:24 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef50fdfd287c591014c8294ec6cfc3978b52fb915775b972301be0fdd6fa892`  
		Last Modified: Tue, 19 Apr 2022 02:20:24 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178926b4d625ea0686fd2044b9e126e60c37a7e5aabb55f86ceecdf791f4e9c2`  
		Last Modified: Tue, 19 Apr 2022 02:20:24 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a181e4a34276f4b47dfd23e6aed5031c34fc6c4f289e23265c6f0220651b1962`  
		Last Modified: Tue, 19 Apr 2022 03:20:04 GMT  
		Size: 15.3 MB (15259445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993873e24f6671b4c07b1536ad9e3dcbf3fdb81cd7d2240fe9d7660472296ca1`  
		Last Modified: Tue, 19 Apr 2022 03:19:58 GMT  
		Size: 1.3 MB (1259472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074510ebf6a6f6d43a03f9e5ce83a56553c015bdb7eaeaae67ed3655ca1a25f1`  
		Last Modified: Tue, 19 Apr 2022 03:20:07 GMT  
		Size: 15.7 MB (15701912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53744618a50eb4ffb2630f4a5a4699b83af851179434c6bc4419587a196f9691`  
		Last Modified: Tue, 19 Apr 2022 03:19:55 GMT  
		Size: 644.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5155c435b0013a616f021ec70da61f71e51c95131a371d5f4e16890151eafb7f`  
		Last Modified: Tue, 19 Apr 2022 03:19:55 GMT  
		Size: 544.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aef3cbae0d02c676479582877a3430241e5e3f6731cceb683dcd7d7b2efb68c`  
		Last Modified: Tue, 19 Apr 2022 03:23:27 GMT  
		Size: 54.0 MB (54047378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0474dfcf4e4d5499c14a839069e9d5aad0088cc6a1160426e9b91b467cecc6c`  
		Last Modified: Tue, 19 Apr 2022 03:22:54 GMT  
		Size: 3.0 KB (2953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eaf53c653eecae932164952c0ce488de3f990841b16bc34765898b8ca71e9d0`  
		Last Modified: Tue, 19 Apr 2022 03:22:54 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; arm variant v7

```console
$ docker pull friendica@sha256:843840baab41e66bfcabde79e4adfed47db564842acb4d3ceadd60f0f35eff43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.9 MB (218877568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f1adad3a392a12db46058e437b86c8c3d5f51aaf1dc5efac60c9aaaf2f6b968`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 02:18:34 GMT
ADD file:e1835d1a0c70a0335757f211893e5d12ddf797e489e10434c0982bdf9b234f67 in / 
# Tue, 29 Mar 2022 02:18:36 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 06:49:01 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 06:49:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 06:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 06:49:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 06:49:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 06:55:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 06:55:07 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 06:55:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 06:55:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 06:55:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 06:55:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 06:55:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 06:55:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 08:55:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 08:55:22 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 08:55:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 08:55:23 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 08:55:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 08:55:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:59:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 08:59:30 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:59:32 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 08:59:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 08:59:34 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 08:59:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 08:59:35 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 08:59:35 GMT
EXPOSE 80
# Tue, 29 Mar 2022 08:59:36 GMT
CMD ["apache2-foreground"]
# Tue, 29 Mar 2022 14:38:43 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Tue, 29 Mar 2022 14:38:44 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 14:39:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 14:44:57 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 14:44:58 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 29 Mar 2022 14:44:58 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 29 Mar 2022 14:45:00 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 29 Mar 2022 14:45:00 GMT
VOLUME [/var/www/html]
# Tue, 29 Mar 2022 14:45:02 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 29 Mar 2022 14:45:02 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Tue, 29 Mar 2022 15:02:09 GMT
ENV FRIENDICA_VERSION=2022.03
# Tue, 29 Mar 2022 15:02:09 GMT
ENV FRIENDICA_ADDONS=2022.03
# Tue, 29 Mar 2022 15:02:10 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Tue, 29 Mar 2022 15:02:10 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Tue, 29 Mar 2022 15:02:51 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 15:02:53 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Tue, 29 Mar 2022 15:02:54 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Tue, 29 Mar 2022 15:02:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 15:02:55 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f98812e1a494a683a5b3dea593dd2ef305f5f732193044c147f22e44b00164bc`  
		Last Modified: Tue, 29 Mar 2022 02:34:13 GMT  
		Size: 26.6 MB (26575370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaf6ea3410c58e5dfb18a8d11ed37871fc3403ec1f9d63969c1410dc411fc9e`  
		Last Modified: Tue, 29 Mar 2022 10:29:10 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd96359d7acc6ffe17c6e8a0a4de1c02c133875cb011c7a24fe9ad218b54a4`  
		Last Modified: Tue, 29 Mar 2022 10:29:38 GMT  
		Size: 69.3 MB (69315695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0627cc4eef368ed04b244a169bebdfcf487fab6d4e2eac809d7afb34311391e`  
		Last Modified: Tue, 29 Mar 2022 10:29:10 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d387fd4a423cc7a5d08660b5cbab93b450e830693bae14bd0b5e74dd3ccabc8`  
		Last Modified: Tue, 29 Mar 2022 10:31:04 GMT  
		Size: 18.0 MB (17993444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ad2abc9ddd2e0652b66bca116bf660d0cc0a718ed979975175469fe3ab60fe`  
		Last Modified: Tue, 29 Mar 2022 10:30:57 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4d62c351c39830761e1abfc546b19a7aaae127dfc337b7d13d9711419fad52`  
		Last Modified: Tue, 29 Mar 2022 10:30:57 GMT  
		Size: 517.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7814c46ea906f13c4b0475566f25e0c29defcbd5033834f7db350165d9cefb8a`  
		Last Modified: Tue, 29 Mar 2022 10:46:22 GMT  
		Size: 10.8 MB (10756842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239bf9b793f21f6ff628eb6a6eea9a12c707a6b3a36eed6ab214da2c1a006288`  
		Last Modified: Tue, 29 Mar 2022 10:46:17 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7cfdfea7603ec630bc8676fcbe5bff89061bcdf68180edae1f2e0cf8a8c39c`  
		Last Modified: Tue, 29 Mar 2022 10:46:24 GMT  
		Size: 9.1 MB (9088185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ae0d4a8cc58200510ade7af55f95a5ba3279a393081d1e30813e4ca1b52f91`  
		Last Modified: Tue, 29 Mar 2022 10:46:17 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823e942555ca6ab5781bc2229499d48d161fedb06fa00c1c104a81a63a7cb6cb`  
		Last Modified: Tue, 29 Mar 2022 10:46:17 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2493e6e90e64ab9f15c1af47cc9a3d4435a6d2772d180971b49350695c92e0`  
		Last Modified: Tue, 29 Mar 2022 10:46:17 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d44d31de32493c8095cc9079ee708fa9c2e3869251f726673ce7333481482e5`  
		Last Modified: Tue, 29 Mar 2022 15:08:19 GMT  
		Size: 15.3 MB (15326775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b527c8dc9671bbd0cd4b0545cf352fee0302953f7fa83cfa08bb7377b91e694f`  
		Last Modified: Tue, 29 Mar 2022 15:08:14 GMT  
		Size: 1.3 MB (1252264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e409d4e04bfda1b5a91f5eea1ee152018b9bd9419fa7fb0d2a50e6076d802d01`  
		Last Modified: Tue, 29 Mar 2022 15:08:21 GMT  
		Size: 14.5 MB (14511235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9385d9f3d7ca5a6d167ffcd7d160c0dfeac6fbe8bd7a531318e9583cd59f6138`  
		Last Modified: Tue, 29 Mar 2022 15:08:12 GMT  
		Size: 641.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68716cdc348087bcc9b5e16536aa65f012d9fe9d78935c3bc97f3c7a97a82eda`  
		Last Modified: Tue, 29 Mar 2022 15:08:12 GMT  
		Size: 541.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d646e7fad899e04459a2ababa95fa98b94c62ae7935374dadd2e9c3194d863`  
		Last Modified: Tue, 29 Mar 2022 15:12:36 GMT  
		Size: 54.0 MB (54047113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec7f4e7e069f0a49dff11cdc941520a7885cd454c8df21c3b7f25302682c4b4`  
		Last Modified: Tue, 29 Mar 2022 15:12:03 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe2e007a35493c6b14aa539029e5b9fd777404ac8fcaa721541de6cb8c163d`  
		Last Modified: Tue, 29 Mar 2022 15:12:03 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; arm64 variant v8

```console
$ docker pull friendica@sha256:b0e4b86bee56f644520c50eb31b9e508df3b2ac969bf67f824aea6df86017568
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.7 MB (241684886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dece2305f4e14a32caab98910e4b44eb3971298eb487d80cadec668ba4a5e991`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:49:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:49:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:50:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:50:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:50:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:55:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:55:55 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:56:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:56:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:56:07 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:56:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:56:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:56:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 04:17:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 04:17:37 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 04:17:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 04:17:39 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 04:18:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 04:18:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:20:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 04:20:52 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:20:53 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 04:20:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 04:20:54 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 04:20:56 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:20:56 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 04:20:57 GMT
EXPOSE 80
# Tue, 29 Mar 2022 04:20:58 GMT
CMD ["apache2-foreground"]
# Wed, 30 Mar 2022 16:08:04 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Wed, 30 Mar 2022 16:08:04 GMT
ENV GOSU_VERSION=1.14
# Wed, 30 Mar 2022 16:08:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 30 Mar 2022 16:10:38 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 16:10:39 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 30 Mar 2022 16:10:40 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 30 Mar 2022 16:10:41 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 30 Mar 2022 16:10:42 GMT
VOLUME [/var/www/html]
# Wed, 30 Mar 2022 16:10:43 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 30 Mar 2022 16:10:44 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Wed, 30 Mar 2022 16:16:13 GMT
ENV FRIENDICA_VERSION=2022.03
# Wed, 30 Mar 2022 16:16:14 GMT
ENV FRIENDICA_ADDONS=2022.03
# Wed, 30 Mar 2022 16:16:15 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Wed, 30 Mar 2022 16:16:16 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Wed, 30 Mar 2022 16:16:37 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 16:16:39 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Wed, 30 Mar 2022 16:16:40 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Wed, 30 Mar 2022 16:16:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 16:16:42 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04185688a150624b38e612cca7804e1ceb05264548c47b5e039a5a45060aef8`  
		Last Modified: Tue, 29 Mar 2022 05:29:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facd7dc68db6eed96f10a31d88890a6c08ef4187f51e716d240ae17c0cc9d7cb`  
		Last Modified: Tue, 29 Mar 2022 05:29:15 GMT  
		Size: 86.7 MB (86716093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab6336e386feb8448b58a2dd1a285f186c01d4a3bc00b362b2c626f7a835e31`  
		Last Modified: Tue, 29 Mar 2022 05:29:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b8d351d3b53ca329aa303dff2df30307563b8f986a1addebc6bddfa18e59a1`  
		Last Modified: Tue, 29 Mar 2022 05:30:15 GMT  
		Size: 18.9 MB (18943678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be22cecadde3e793a43747880bb2ddc3a13b59482ec865ef62356a97ae54a4af`  
		Last Modified: Tue, 29 Mar 2022 05:30:13 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d678ae3151a74648b652849c8cc6049def503b181cc68bc77a2a896e5fe30e1`  
		Last Modified: Tue, 29 Mar 2022 05:30:13 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e76af5ce0a95b4dbcfa78783bc26c1db6907eda151ca1d8330f9937d8f4ac9`  
		Last Modified: Tue, 29 Mar 2022 05:41:32 GMT  
		Size: 10.5 MB (10542059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f0521250750e42fb1c32e9bf1feb3aae05301f6e0fb2788ef200afc56ecb56`  
		Last Modified: Tue, 29 Mar 2022 05:41:28 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f8f7d9cbbe242194a02792259ff1d0f1ef36951638b9a97b61a2584dd3c138`  
		Last Modified: Tue, 29 Mar 2022 05:41:30 GMT  
		Size: 10.0 MB (9998982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544b6aa59a7570e01cc799a1751c8346de8e4c3f42c61fe8012f41dd3a46e4ed`  
		Last Modified: Tue, 29 Mar 2022 05:41:28 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6973436120e1fa618f2f7905a4badbe6253d3686e7057d6c48ee5cb483999f81`  
		Last Modified: Tue, 29 Mar 2022 05:41:28 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e359b21249324669779c8244969db9395c4d1804e20db05aaab1f57ac5ac46a`  
		Last Modified: Tue, 29 Mar 2022 05:41:28 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e88b97de051bd7464c9b8420de9cda815be10bb2069c346ccf18ec5519b7ce0`  
		Last Modified: Wed, 30 Mar 2022 16:19:33 GMT  
		Size: 15.1 MB (15133978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4da6dc2c3c8364980407a5b3214e4631a41a1b4e44df30de09f945c72be8a8e`  
		Last Modified: Wed, 30 Mar 2022 16:19:32 GMT  
		Size: 996.2 KB (996244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34a5a94ba1515271ba215d78f7386054ceb5b3bdbfcc442f83c0c2d4420ac62`  
		Last Modified: Wed, 30 Mar 2022 16:19:33 GMT  
		Size: 15.5 MB (15477382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d97c11fe92f1b7bc2e26b6a7d8e63d68a3c7e63cbcd27b8e3a7a5577848a98`  
		Last Modified: Wed, 30 Mar 2022 16:19:30 GMT  
		Size: 608.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b8e3bb44ec1d36f8fbd7bb9d6889dd1eb090b51a098f61371bf0a3a55f1ac3`  
		Last Modified: Wed, 30 Mar 2022 16:19:29 GMT  
		Size: 540.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:416aa160cb6df0056e02a9bdbd47b1d84a704ab94966b0397710b6f739af2ebd`  
		Last Modified: Wed, 30 Mar 2022 16:20:46 GMT  
		Size: 53.8 MB (53801682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4089db5beadd9d4604038bc90dcb885ce418b3809fdcd977208ec2e381f9ef6f`  
		Last Modified: Wed, 30 Mar 2022 16:20:39 GMT  
		Size: 3.0 KB (2951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334b44aad058a0d46ac4ba0caf8045f872a4ff69d68a4416baa603859901dbfc`  
		Last Modified: Wed, 30 Mar 2022 16:20:40 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; 386

```console
$ docker pull friendica@sha256:ed5b4cd506693eb5e09437b0140e10d1dd9a2a702b8d727a13c52e99393ee2b6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **252.9 MB (252901249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:953e6831130b209c414da0ad6655b8c846c523f844b0bc296164b30dd27f9340`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:13:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:13:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:14:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:14:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:14:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:17:26 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:17:26 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:17:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:17:36 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:17:37 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:17:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:17:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:17:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 02:36:38 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 02:36:38 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 02:36:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 02:36:40 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 02:36:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 02:36:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:38:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 02:38:33 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:38:33 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 02:38:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 02:38:35 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 02:38:37 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 02:38:37 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 02:38:38 GMT
EXPOSE 80
# Tue, 29 Mar 2022 02:38:39 GMT
CMD ["apache2-foreground"]
# Tue, 29 Mar 2022 20:40:38 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Tue, 29 Mar 2022 20:40:38 GMT
ENV GOSU_VERSION=1.14
# Tue, 29 Mar 2022 20:40:48 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 29 Mar 2022 20:46:29 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 20:46:29 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 29 Mar 2022 20:46:30 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 29 Mar 2022 20:46:31 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 29 Mar 2022 20:46:32 GMT
VOLUME [/var/www/html]
# Tue, 29 Mar 2022 20:46:33 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 29 Mar 2022 20:46:34 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Tue, 29 Mar 2022 20:48:14 GMT
ENV FRIENDICA_VERSION=2022.03
# Tue, 29 Mar 2022 20:48:15 GMT
ENV FRIENDICA_ADDONS=2022.03
# Tue, 29 Mar 2022 20:48:16 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Tue, 29 Mar 2022 20:48:17 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Tue, 29 Mar 2022 20:48:38 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 20:48:40 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Tue, 29 Mar 2022 20:48:41 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Tue, 29 Mar 2022 20:48:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 20:48:42 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5eef24434e26d7c7efe110e0a514725a245f4a80feef19fde4adf2881c842c6`  
		Last Modified: Tue, 29 Mar 2022 03:19:22 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce29d62a2961a018f305c25e5e41d731c9c0f7ef22ee18a11b27b83c635fd5e`  
		Last Modified: Tue, 29 Mar 2022 03:19:36 GMT  
		Size: 92.5 MB (92510998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a5747ae4f3b12af8c59a4f80eab5e5e8dfd15b8f67d7364e1c226edd82eef1`  
		Last Modified: Tue, 29 Mar 2022 03:19:22 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f03504ae01782d4552efcd88dac5836f7fdb6e628ef6076e536f44bd3726ba`  
		Last Modified: Tue, 29 Mar 2022 03:20:40 GMT  
		Size: 19.5 MB (19501820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:092d9feff8c5c22bf2dfa04dc0622e669df97a9129396f3c60fbbe8c66efafe6`  
		Last Modified: Tue, 29 Mar 2022 03:20:37 GMT  
		Size: 430.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3dd2fa3ed7eaa550087f72d9a21a7cd0385b2967afcd828745e74e0e5c7b67`  
		Last Modified: Tue, 29 Mar 2022 03:20:37 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb24d0f9a354a49651027a736d0565e749a1f13cd16cd30943875c809fa1bfb9`  
		Last Modified: Tue, 29 Mar 2022 03:32:20 GMT  
		Size: 10.5 MB (10542049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836416aae1db2ea61eb03a8ad3f49333d68171e9cec74dc72e3c0a34c4295690`  
		Last Modified: Tue, 29 Mar 2022 03:32:15 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f60ae445e266b6c6dfae9eb6e41af8b6075acb98aecf55d136502085126f0e6`  
		Last Modified: Tue, 29 Mar 2022 03:32:16 GMT  
		Size: 10.4 MB (10441908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45940ebc4ab499421a89f7c528036c870de3fb8b7decdf55ac06e38bd2a6ca7`  
		Last Modified: Tue, 29 Mar 2022 03:32:15 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85b8647a14662032f479ac9a7ddc38c798dc6701baf7bc351ac3756ce2105f0`  
		Last Modified: Tue, 29 Mar 2022 03:32:14 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0e1ec2a42ef97b3d4d612c3f5be513468b54beebdc75d517602ac1c58df939`  
		Last Modified: Tue, 29 Mar 2022 03:32:15 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60acde47017baeccf2f6f5ac9d4fb769981bd19c09a0de4edd8d4b86211c3d8f`  
		Last Modified: Tue, 29 Mar 2022 20:51:57 GMT  
		Size: 15.8 MB (15820795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d424c71343b4a3e196fdb6cdcf8781c3a5b97430cda11f5f37fb054a6be0836c`  
		Last Modified: Tue, 29 Mar 2022 20:51:56 GMT  
		Size: 1.0 MB (1035995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19394b974049f125bab13f07c0911417b31dacef86b9e1fcb77320880ea50809`  
		Last Modified: Tue, 29 Mar 2022 20:51:58 GMT  
		Size: 16.8 MB (16846097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc74db0c556ed066875be4f42f88d26b59872edbb2eeeddfa5353c8deedca26f`  
		Last Modified: Tue, 29 Mar 2022 20:51:53 GMT  
		Size: 609.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a1294dfb3f1fa34b0e9020f44b403eebf59031a27dd3c6967c37d1a52fafb6`  
		Last Modified: Tue, 29 Mar 2022 20:51:53 GMT  
		Size: 537.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d525c2f4281a8bb447ba9c44a5add4d49bf26d25ac27378b8fc8016e015622d`  
		Last Modified: Tue, 29 Mar 2022 20:52:42 GMT  
		Size: 53.8 MB (53801598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61171e58259ea928d3cbca54122e09e91e5fbbf15f59755f9011fef8a0ecd81`  
		Last Modified: Tue, 29 Mar 2022 20:52:35 GMT  
		Size: 3.0 KB (2951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533d4145e6900380d4b025449b4dac83d64facf2e0bb851877c6e6915ecb0f2e`  
		Last Modified: Tue, 29 Mar 2022 20:52:35 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; mips64le

```console
$ docker pull friendica@sha256:b0897965ac45b10f6b28e59a2a63a57fe856aeb30edfa1d179bb7b766c5b5f3a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.7 MB (225685133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c629fea9608c375da64640ae9b9391bd534b6cb47f1f10f17da5f4a2fd2ecba`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 07:42:27 GMT
ADD file:32aa9fd7ee5c64e4bd49459e801e3e5dc50138590bbfca671e336a197aa7fa92 in / 
# Tue, 29 Mar 2022 07:42:31 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 19:03:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 19:03:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 19:05:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 19:05:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 19:05:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 19:19:46 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 19:19:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 19:20:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 19:20:54 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 19:21:01 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 19:21:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 19:21:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 19:21:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 23:04:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 23:04:53 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 23:04:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 23:05:00 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 23:05:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 23:05:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 23:14:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 23:14:39 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 23:14:47 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 23:14:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 23:14:54 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 23:14:57 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 23:15:00 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 23:15:04 GMT
EXPOSE 80
# Tue, 29 Mar 2022 23:15:07 GMT
CMD ["apache2-foreground"]
# Thu, 31 Mar 2022 03:01:13 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Thu, 31 Mar 2022 03:01:16 GMT
ENV GOSU_VERSION=1.14
# Thu, 31 Mar 2022 03:02:04 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Thu, 31 Mar 2022 03:12:38 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 03:12:42 GMT
ENV PHP_MEMORY_LIMIT=512M
# Thu, 31 Mar 2022 03:12:46 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Thu, 31 Mar 2022 03:12:53 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 31 Mar 2022 03:12:57 GMT
VOLUME [/var/www/html]
# Thu, 31 Mar 2022 03:13:04 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Thu, 31 Mar 2022 03:13:08 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Thu, 31 Mar 2022 03:34:25 GMT
ENV FRIENDICA_VERSION=2022.03
# Thu, 31 Mar 2022 03:34:29 GMT
ENV FRIENDICA_ADDONS=2022.03
# Thu, 31 Mar 2022 03:34:33 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Thu, 31 Mar 2022 03:34:37 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Thu, 31 Mar 2022 03:36:02 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 03:36:10 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Thu, 31 Mar 2022 03:36:16 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Thu, 31 Mar 2022 03:36:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 03:36:28 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:5c2a8045f9de06328ab3d0ff505d990892219b7faee393bc9ac342347fc83d04`  
		Last Modified: Tue, 29 Mar 2022 07:52:59 GMT  
		Size: 29.6 MB (29641474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241646a732d87181d18d500ef743d5d3a2d6928dee0e4904828284b8f7781bec`  
		Last Modified: Wed, 30 Mar 2022 00:21:32 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a39d9c931fe7ab8e8a9112a43a8dd9051f2e0c88cb289d2ea4076929ba3514`  
		Last Modified: Wed, 30 Mar 2022 00:22:24 GMT  
		Size: 71.8 MB (71809415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f70f95d116fa6ab27850a082629e46aebd303d2cbbd450d4e07a47b59babf3`  
		Last Modified: Wed, 30 Mar 2022 00:21:32 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a830fdb776609fbc90ff477336538e0d0d197a763fbfa0b4ce4e072e5dc057`  
		Last Modified: Wed, 30 Mar 2022 00:23:31 GMT  
		Size: 18.9 MB (18933435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc6ef92a058387f9d0fc45394ee63826e21f2d5e9d4ee2fd88af074297be6ae`  
		Last Modified: Wed, 30 Mar 2022 00:23:19 GMT  
		Size: 439.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd7427591217cd607d3b02a04ca7db9bd14cafbdc3921e594766014fb6662af`  
		Last Modified: Wed, 30 Mar 2022 00:23:18 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5192a998281980ee351d0e2fb73248256b8861f42aa6129a37a984aa67b9125`  
		Last Modified: Wed, 30 Mar 2022 00:33:34 GMT  
		Size: 10.5 MB (10540675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee6a941257da1432edf7e5507f0d44df29ed3efcb380aa217a9d856b05e1299`  
		Last Modified: Wed, 30 Mar 2022 00:33:29 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b0654c37c985cdd8a89c83954e03baa16c92e0a722b447f6a18c46b276b6ee`  
		Last Modified: Wed, 30 Mar 2022 00:33:37 GMT  
		Size: 9.7 MB (9693395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6174e526694ba7cceafeafad2e22a5a628c8dd455a5bacc2b26e53f352901c0`  
		Last Modified: Wed, 30 Mar 2022 00:33:29 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d514f4450bfb51c117287b436406dbc13a3d8016f89441c47823de412a3eb901`  
		Last Modified: Wed, 30 Mar 2022 00:33:30 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48f0a678799ca10252b27508435e81a3fa9b5f39d0bfb3a3532c9797538a16a8`  
		Last Modified: Wed, 30 Mar 2022 00:33:29 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515c033f5bf2a91f3660e30d8d8d7eb06686cf8d68c72ced49beb909669641f8`  
		Last Modified: Thu, 31 Mar 2022 03:41:25 GMT  
		Size: 14.9 MB (14869765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7070f6b57a7b82d40abcc0aa369563b3bd630bb9daabf65bf4689ab2d385ffb`  
		Last Modified: Thu, 31 Mar 2022 03:41:18 GMT  
		Size: 947.3 KB (947258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfb8123f6d59371c96025ca2c47cdfcb36956a366276f698509d0c280407aa16`  
		Last Modified: Thu, 31 Mar 2022 03:41:28 GMT  
		Size: 15.4 MB (15436325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dae17a152294949838dc77005a6136c6b25558f27c8b1250af07beae6be8843`  
		Last Modified: Thu, 31 Mar 2022 03:41:14 GMT  
		Size: 611.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e331588accf8fa178986c5ee616e7c21be9b249b711fa1801341bde03eb283`  
		Last Modified: Thu, 31 Mar 2022 03:41:14 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78d64fdfa6bb66059e5e4d3f2830159397e1b605a810a28277f818b904ca406`  
		Last Modified: Thu, 31 Mar 2022 03:44:11 GMT  
		Size: 53.8 MB (53802891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2d1ae4a14ce2730e60bca7ac12fcfa8ec5c1f41efbc153b412bd2caeca5899`  
		Last Modified: Thu, 31 Mar 2022 03:43:43 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfa5a75aade35a069e9e01183c55fa795ae57b0fa4d5b6d017bc834ed9bb85f`  
		Last Modified: Thu, 31 Mar 2022 03:43:44 GMT  
		Size: 930.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; ppc64le

```console
$ docker pull friendica@sha256:0220a01ee4d08ebc7513624e25426a8184bc01ce5a6d9acdd0a7d2e54299a4a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.9 MB (251881077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55ea565e3d8db35ef228721fb923a6ab0be8adfd4d5c2138c0e01a15279f3d44`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:08 GMT
ADD file:e7ae113c10f322a9cffc46b62ba12820e270caaadaee3c5b907c801a37e1632c in / 
# Tue, 29 Mar 2022 00:22:11 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 01:19:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 01:19:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 01:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 01:21:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:21:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:27:40 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 01:27:42 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 01:28:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 01:28:35 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 01:28:39 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 01:28:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:28:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:28:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 03:49:02 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 03:49:04 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 03:49:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 03:49:06 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 03:49:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Mar 2022 03:49:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:53:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 03:53:44 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:53:48 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 03:53:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 03:53:52 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Mar 2022 03:53:55 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:53:57 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 03:54:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 03:54:04 GMT
CMD ["apache2-foreground"]
# Wed, 30 Mar 2022 11:33:39 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Wed, 30 Mar 2022 11:33:43 GMT
ENV GOSU_VERSION=1.14
# Wed, 30 Mar 2022 11:34:32 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Wed, 30 Mar 2022 11:43:13 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 11:43:20 GMT
ENV PHP_MEMORY_LIMIT=512M
# Wed, 30 Mar 2022 11:43:24 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Wed, 30 Mar 2022 11:43:34 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Wed, 30 Mar 2022 11:43:36 GMT
VOLUME [/var/www/html]
# Wed, 30 Mar 2022 11:43:43 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Wed, 30 Mar 2022 11:43:46 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Wed, 30 Mar 2022 11:57:28 GMT
ENV FRIENDICA_VERSION=2022.03
# Wed, 30 Mar 2022 11:57:33 GMT
ENV FRIENDICA_ADDONS=2022.03
# Wed, 30 Mar 2022 11:57:38 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Wed, 30 Mar 2022 11:57:43 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Wed, 30 Mar 2022 11:58:59 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 11:59:05 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Wed, 30 Mar 2022 11:59:06 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Wed, 30 Mar 2022 11:59:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 11:59:15 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ecc74bb8af5a048e1123af0e17d88ef3da1d10951ada79e8e1cc9c0a694245d3`  
		Last Modified: Tue, 29 Mar 2022 00:32:57 GMT  
		Size: 35.3 MB (35282506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c087cbc2c7d55cf0725407980efe0470467d5dfd4c5658c2127bd0317fde608`  
		Last Modified: Tue, 29 Mar 2022 05:04:48 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6894e5460431e4ce8d4f063709daa73369a05689921d0cc6896436ea103f76`  
		Last Modified: Tue, 29 Mar 2022 05:05:20 GMT  
		Size: 86.6 MB (86625963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a2eb86a2490b3a6fc39680ea69efc0c28373b420a70b5482adc541e8b8f366`  
		Last Modified: Tue, 29 Mar 2022 05:04:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3efb01d35af6e00fdfb305fa837992b773d71bb3ec8ef8a05af15d85f5cc6b`  
		Last Modified: Tue, 29 Mar 2022 05:06:34 GMT  
		Size: 20.5 MB (20453935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2947ac755e32bf6c4a782e897715296a71cfeb50ec10b45631db62218f0eeb`  
		Last Modified: Tue, 29 Mar 2022 05:06:29 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c4a2e8c312cc99c4e1f371d4bff5828b533bcb94eaf215a5d418a3378aed09`  
		Last Modified: Tue, 29 Mar 2022 05:06:29 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dddd2eb3264f3f5d674f0c7e1316d21da2c482a454bd053c4b010ee26e1cfbf`  
		Last Modified: Tue, 29 Mar 2022 05:20:27 GMT  
		Size: 10.8 MB (10758355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5129dd5fe9f9955e51cfe4a2ec5a1d77cd86f343b718e30958b10247669f7be`  
		Last Modified: Tue, 29 Mar 2022 05:20:23 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36d7bbc11fd954501d445e4cda37d7611a8c92cd7efc858d11601c35bfcca4`  
		Last Modified: Tue, 29 Mar 2022 05:20:26 GMT  
		Size: 10.9 MB (10892988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7902acf32afff5f20b8308b4d25cde38fcfaa1230c3a2b7064c7d87432821a`  
		Last Modified: Tue, 29 Mar 2022 05:20:23 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3543c322e7afb129b5cc4a688de89632c397398675d86eacd3142ddb7cfc706`  
		Last Modified: Tue, 29 Mar 2022 05:20:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b784ee8878df30387cdbc8f98143af1c776305dfa7033517da3d472c457310b7`  
		Last Modified: Tue, 29 Mar 2022 05:20:23 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebffa979315600e016f0b5e7875497e490c852aa7e8ef6c0b6f362dec668aff`  
		Last Modified: Wed, 30 Mar 2022 12:20:48 GMT  
		Size: 15.3 MB (15262164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a21a4b27193cc8d9fe938a4394e3c40d2cb99cf4503ddd91de3b1c6b49fb1574`  
		Last Modified: Wed, 30 Mar 2022 12:20:46 GMT  
		Size: 1.2 MB (1196405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f87b5e6a55d70454877f6e6903f921bf641e39ff8fa2b7d99aade29a195f5f`  
		Last Modified: Wed, 30 Mar 2022 12:20:47 GMT  
		Size: 17.3 MB (17347149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af36a68c8e9272ab0cf65d75de0adcedd9e6995008bc2ce25d74cf1235e69eec`  
		Last Modified: Wed, 30 Mar 2022 12:20:39 GMT  
		Size: 644.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8745c6bd6ae9a3ce6bf50ae235f038e91dd4ad73db7c457912f124fed47bedcf`  
		Last Modified: Wed, 30 Mar 2022 12:20:39 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d447667f37b530a350cbfd9f30f9c0c839acc091ed1deab8db09a33829c7901`  
		Last Modified: Wed, 30 Mar 2022 12:22:20 GMT  
		Size: 54.1 MB (54050952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a83ee0e3a393abafa135323984f40d8c2ef5c4fcae35fadf5d9f8289207828`  
		Last Modified: Wed, 30 Mar 2022 12:22:11 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd6bade38913a9b2ca99528aabcb7a18d51766d14a9250d1ef289578b24bca8`  
		Last Modified: Wed, 30 Mar 2022 12:22:11 GMT  
		Size: 932.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `friendica:latest` - linux; s390x

```console
$ docker pull friendica@sha256:f5b39130b62069c8754a4c2666aa388e55f1453928e0f6fcc7b89d4c3bb84563
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.5 MB (226514689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48154858778008ecd5051077feebf3a4a57371c6c0db15949656eabe26e70031`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:57 GMT
ADD file:39c5e0d7a686abd19448ab3e6237d50955ae2187fc2b64289a08c2549352b8f1 in / 
# Tue, 29 Mar 2022 00:51:58 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 02:21:07 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 29 Mar 2022 02:21:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 29 Mar 2022 02:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 02:21:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 02:21:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 02:24:13 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 29 Mar 2022 02:24:13 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 29 Mar 2022 02:24:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 29 Mar 2022 02:24:21 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 29 Mar 2022 02:24:21 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 29 Mar 2022 02:24:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:24:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:24:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 03:44:11 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Apr 2022 01:03:28 GMT
ENV PHP_VERSION=7.4.29
# Tue, 19 Apr 2022 01:03:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Tue, 19 Apr 2022 01:03:30 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Tue, 19 Apr 2022 01:03:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 19 Apr 2022 01:03:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:05:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Apr 2022 01:05:22 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:05:22 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Apr 2022 01:05:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Apr 2022 01:05:23 GMT
STOPSIGNAL SIGWINCH
# Tue, 19 Apr 2022 01:05:23 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 19 Apr 2022 01:05:23 GMT
WORKDIR /var/www/html
# Tue, 19 Apr 2022 01:05:23 GMT
EXPOSE 80
# Tue, 19 Apr 2022 01:05:23 GMT
CMD ["apache2-foreground"]
# Tue, 19 Apr 2022 03:44:15 GMT
RUN set -ex;         apt-get update;     apt-get install -y --no-install-recommends         rsync         bzip2         msmtp         tini     ;
# Tue, 19 Apr 2022 03:44:16 GMT
ENV GOSU_VERSION=1.14
# Tue, 19 Apr 2022 03:44:33 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates wget; 	if ! command -v gpg; then 		apt-get install -y --no-install-recommends gnupg2 dirmngr; 	elif gpg --version | grep -q '^gpg (GnuPG) 1\.'; then 		apt-get install -y --no-install-recommends gnupg-curl; 	fi; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/gosu.asc; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		chmod +x /usr/local/bin/gosu; 	gosu --version; 	gosu nobody true
# Tue, 19 Apr 2022 03:49:15 GMT
RUN set -ex;         savedAptMark="$(apt-mark showmanual)";         apt-get update;     apt-get install -y --no-install-recommends         mariadb-client         bash         libpng-dev         libjpeg62-turbo-dev         libtool         libmagick++-dev         libmemcached-dev         libgraphicsmagick1-dev         libfreetype6-dev         libwebp-dev         librsvg2-2         libzip-dev         libldap2-dev     ;             debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)";         docker-php-ext-configure gd         --with-freetype         --with-jpeg         --with-webp     ;     docker-php-ext-configure ldap         --with-libdir=lib/$debMultiarch/     ;    docker-php-ext-install -j "$(nproc)"         pdo_mysql         gd         exif         zip         opcache         ctype         pcntl         ldap     ;         pecl install apcu-5.1.21;     pecl install memcached-3.2.0RC1;     pecl install redis-5.3.7;     pecl install imagick-3.7.0;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         apt-mark auto '.*' > /dev/null;     apt-mark manual $savedAptMark;     ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so         | awk '/=>/ { print $3 }'         | sort -u         | xargs -r dpkg-query -S         | cut -d: -f1         | sort -u         | xargs -rt apt-mark manual;         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 03:49:17 GMT
ENV PHP_MEMORY_LIMIT=512M
# Tue, 19 Apr 2022 03:49:18 GMT
ENV PHP_UPLOAD_LIMIT=512M
# Tue, 19 Apr 2022 03:49:19 GMT
RUN set -ex;     {         echo 'opcache.enable=1' ;         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidte_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         {         echo sendmail_path = "/usr/bin/msmtp -t";     } > /usr/local/etc/php/conf.d/sendmail.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > /usr/local/etc/php/conf.d/friendica.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Tue, 19 Apr 2022 03:49:20 GMT
VOLUME [/var/www/html]
# Tue, 19 Apr 2022 03:49:22 GMT
RUN set -ex;    a2enmod rewrite remoteip ;    {     echo RemoteIPHeader X-Real-IP ;     echo RemoteIPTrustedProxy 10.0.0.0/8 ;     echo RemoteIPTrustedProxy 172.16.0.0/12 ;     echo RemoteIPTrustedProxy 192.168.0.0/16 ;    } > /etc/apache2/conf-available/remoteip.conf;    a2enconf remoteip
# Tue, 19 Apr 2022 03:49:22 GMT
ENV FRIENDICA_SYSLOG_FLAGS=39
# Tue, 19 Apr 2022 03:57:22 GMT
ENV FRIENDICA_VERSION=2022.03
# Tue, 19 Apr 2022 03:57:22 GMT
ENV FRIENDICA_ADDONS=2022.03
# Tue, 19 Apr 2022 03:57:23 GMT
ENV FRIENDICA_DOWNLOAD_SHA256=f190dd05bdd2ecff753da108535dbc4e406b0fe291c0764e87f93d9510aae74e
# Tue, 19 Apr 2022 03:57:23 GMT
ENV FRIENDICA_DOWNLOAD_ADDONS_SHA256=d6b95835724b9814aa7c1862f985cdaf8754e7527b41ce80ca58ee5378807936
# Tue, 19 Apr 2022 03:57:55 GMT
RUN set -ex;     fetchDeps="         gnupg     ";     apt-get update;     apt-get install -y --no-install-recommends $fetchDeps;         export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 08656443618E6567A39524083EE197EF3F9E4287;         curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz";     curl -fsSL -o friendica-full-${FRIENDICA_VERSION}.tar.gz.asc         "https://files.friendi.ca/friendica-full-${FRIENDICA_VERSION}.tar.gz.asc";     gpg --batch --verify friendica-full-${FRIENDICA_VERSION}.tar.gz.asc friendica-full-${FRIENDICA_VERSION}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_SHA256} *friendica-full-${FRIENDICA_VERSION}.tar.gz" | sha256sum -c;     tar -xzf friendica-full-${FRIENDICA_VERSION}.tar.gz -C /usr/src/;     rm friendica-full-${FRIENDICA_VERSION}.tar.gz friendica-full-${FRIENDICA_VERSION}.tar.gz.asc;     mv -f /usr/src/friendica-full-${FRIENDICA_VERSION}/ /usr/src/friendica;     chmod 777 /usr/src/friendica/view/smarty3;         curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz";     curl -fsSL -o friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc             "https://files.friendi.ca/friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc";     gpg --batch --verify friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc friendica-addons-${FRIENDICA_ADDONS}.tar.gz;     echo "${FRIENDICA_DOWNLOAD_ADDONS_SHA256} *friendica-addons-${FRIENDICA_ADDONS}.tar.gz" | sha256sum -c;     mkdir -p /usr/src/friendica/proxy;     mkdir -p /usr/src/friendica/addon;     tar -xzf friendica-addons-${FRIENDICA_ADDONS}.tar.gz -C /usr/src/friendica/addon --strip-components=1;     rm friendica-addons-${FRIENDICA_ADDONS}.tar.gz friendica-addons-${FRIENDICA_ADDONS}.tar.gz.asc;         gpgconf --kill all;     rm -rf "$GNUPGHOME";         apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false $fetchDeps;     rm -rf /var/lib/apt/lists/*
# Tue, 19 Apr 2022 03:58:02 GMT
COPY multi:31b45a7507c100b0a9b3decdeeedd3c1880f5c7c482c8e17c6047c00a1ffcb3d in / 
# Tue, 19 Apr 2022 03:58:02 GMT
COPY multi:201dba5df7e408009a8882797a28095a47753a2db673a80c99e898e88501c42e in /usr/src/friendica/config/ 
# Tue, 19 Apr 2022 03:58:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 19 Apr 2022 03:58:03 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:ffb22bcde95509bb75f6dd2d69f3fdb5c7471727e4d720b31d92cd297582865c`  
		Last Modified: Tue, 29 Mar 2022 01:04:43 GMT  
		Size: 29.7 MB (29655426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc646829b4b7797b4933a4313f2ac38c99002eb37cf71d4af56a2cfac7913a`  
		Last Modified: Tue, 29 Mar 2022 04:24:22 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df487a79caa5ca21be0624e6c16cefe85b4350a4a6c39c5f113490ba6ae82a2`  
		Last Modified: Tue, 29 Mar 2022 04:24:31 GMT  
		Size: 71.6 MB (71619822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51d43600a7dc96e3459ca669fa130d53ddd96bd0b420428ab5d6e7f9ba723e8`  
		Last Modified: Tue, 29 Mar 2022 04:24:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a2a1ea2bd50009aff888b17ef0b2beed432e8d5a63a8b882da2cbf9265cea9`  
		Last Modified: Tue, 29 Mar 2022 04:34:26 GMT  
		Size: 19.1 MB (19054463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21e270f6d1aa8cc59b2fde320a29a5b077344626bea8bc99d2812bc601b165ec`  
		Last Modified: Tue, 29 Mar 2022 04:34:20 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef1a1f8227f7c54b9983422c06f616faabea0efae1940602b5b7557bd697254`  
		Last Modified: Tue, 29 Mar 2022 04:34:15 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d7afa850f62f6cbf0a6f4de0056c78681d66a9afd2d7556dbc843666ce29c7`  
		Last Modified: Tue, 19 Apr 2022 02:06:50 GMT  
		Size: 10.8 MB (10757647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b97044a13c41e1593595341465b53b0e61f86e5a9acfca78c5848eff0e7128`  
		Last Modified: Tue, 19 Apr 2022 02:06:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709a7e16b0ed50d3925c64280d2e8f76a33ce74d725113fc6b9ec59374a19367`  
		Last Modified: Tue, 19 Apr 2022 02:06:50 GMT  
		Size: 9.8 MB (9753147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2026da911ee17b103cc5e5d75de2a0867b8a124d0991e8cf7da7ca42006b296`  
		Last Modified: Tue, 19 Apr 2022 02:06:49 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e2fcf8e3f379a7cb369928095e41bf6782e0ae6369d4e407b0a5bfe5f36b3a`  
		Last Modified: Tue, 19 Apr 2022 02:06:48 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad8df31ce561835ed08b7a603608be3e7c65eaece9e78749312e56d3d9beb92`  
		Last Modified: Tue, 19 Apr 2022 02:06:48 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5346beaf83e5b9f150d185e6e40e5930c8339379f05b5d4c3348d06fb0b63df`  
		Last Modified: Tue, 19 Apr 2022 04:00:45 GMT  
		Size: 14.8 MB (14810240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f853d5251ad294b9a22c1b06838e6616e66a5ab5c25b4123c7bb787dbb0f02`  
		Last Modified: Tue, 19 Apr 2022 04:00:44 GMT  
		Size: 1.3 MB (1258139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1886f952f73c7f7958ad04bc1d57159acf1f24696fafb638d56ef0cc8a9c1c1`  
		Last Modified: Tue, 19 Apr 2022 04:00:46 GMT  
		Size: 15.5 MB (15547484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3236c895c140f2e06f720c45445294d9e47f28c60e5060c73711e8dc4a67ba57`  
		Last Modified: Tue, 19 Apr 2022 04:00:42 GMT  
		Size: 639.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600f5bb95fe1694d413dd55a85d7d60ff3ea205b8b2760bdacbd2cb76a770aee`  
		Last Modified: Tue, 19 Apr 2022 04:00:42 GMT  
		Size: 540.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdf4aa6c690f16a9dbfee3ef523df321fe60a183bfe39ae7f6b8c444ef9431b`  
		Last Modified: Tue, 19 Apr 2022 04:01:41 GMT  
		Size: 54.0 MB (54047691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21b099ac9d5d0ca86304a7ded5c9b32e16b4065646ec03c040fc7db6ec3c309`  
		Last Modified: Tue, 19 Apr 2022 04:01:35 GMT  
		Size: 3.0 KB (2952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480b9c600c6679d1c6662d27e368bfedebfa48cc779395f6b0628339c32e0d7a`  
		Last Modified: Tue, 19 Apr 2022 04:01:35 GMT  
		Size: 929.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
